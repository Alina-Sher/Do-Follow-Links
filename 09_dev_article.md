# Why the Dashboard Number and the Database Number Disagree

| Field | Value |
|---|---|
| Platform | DEV Community (https://dev.to/new) |
| Status | NOT SUBMITTED |
| Suggested title | Why the Dashboard Number and the Database Number Disagree |
| Short description | Common reasons analytics numbers drift from source data, and checks that catch them early. |
| Category | Data engineering |
| Target URL | https://www.techabout.com/services/data-analytics |
| Proposed anchor text | TechAbout's data engineering and analytics services |
| Facts source | content/00_company_facts_verified.md |

**Before submitting:** read DEV's current terms and community guidelines; publish under the real author's profile; add a short disclosure line; use tags such as dataengineering, analytics, sql.

---

Every data team has had this meeting: a leader quotes a figure from a dashboard, someone checks the database, and the numbers differ. Usually nobody is wrong. The pipeline between the two is doing something people did not expect.

## 1. Two definitions of the same word
"Active customer" or "revenue" often means different things in different tools. Write definitions in one place, version them, and make the dashboard use that single definition.

## 2. Time zones and date boundaries
A day in UTC is not a day in local time. Pick one reporting time zone, document it, and convert at one stage only.

## 3. Late and duplicate events
Mobile apps and queues deliver events late or twice. Without de-duplication keys and a rule for late arrivals, counts drift up and totals change after the fact. Decide how long a day stays "open".

## 4. Joins that multiply rows
Joining a one-to-many table before aggregating inflates sums. A simple test is to count rows before and after each join and explain any difference.

## 5. Filters hidden in the tool
Dashboards sometimes apply default filters (a date range, a region, excluded test accounts). Show active filters on the dashboard itself.

## 6. Pipelines that fail quietly
A job that ran but loaded zero rows looks fine. Add checks for row counts, freshness and null rates, and send alerts to a named owner.

## Add reconciliation checks
Pick three headline metrics and compare them automatically against the source system every day, within a tolerance you agree on. When a check fails, stop publishing the affected report instead of shipping a wrong number.

```sql
-- Example: compare yesterday's order count between source and warehouse
SELECT
  (SELECT COUNT(*) FROM source.orders  WHERE order_date = CURRENT_DATE - 1) AS source_count,
  (SELECT COUNT(*) FROM warehouse.fact_orders WHERE order_date = CURRENT_DATE - 1) AS warehouse_count;
```

## Takeaway
Trust in a number comes from a pipeline that can explain itself. Definitions, single time-zone conversion, de-duplication and daily reconciliation catch most disagreements before leadership sees them.

*Author: [AUTHOR NAME], [ROLE] at [TechAbout](https://www.techabout.com/services/data-analytics).*
