# TechAbout - Do-Follow Links Project (Batch 1)

Status as of 2026-10-26: **research and content preparation only. No submissions have been made, no pages are published, no links have been verified.**

## What is in this folder
| Path | What it is |
|---|---|
| `TechAbout_Backlink_Research_and_Evidence.xlsx` | Workbook: Website Research, Submission Tracker, Link Verification, Summary (formula-driven) |
| `research/100_website_opportunities.csv` | Batch 1 research (25 of 100 candidates; add batches 2-4 here) |
| `research/submission_tracker.csv` | Same tracker as the workbook, for CSV users (statuses all "Not Started") |
| `content/` | Verified company facts + ready-to-edit submission drafts (10 drafts for the top opportunities) |
| `evidence/` | Empty on purpose. Real screenshots go here. See `evidence/screenshot_checklist.md` |
| `reports/final_report_template.md` | Report skeleton to fill with real numbers |
| `reports/verification_summary.csv` | Snapshot of counts at hand-over (all zeros for submissions) |
| `guides/step_by_step_guide.md` | Beginner guide to submitting, recording URLs, screenshots and checking rel attributes |

## Batch 1 results in numbers
- Candidates researched: 25 (target 100; 75 still to research)
- Free submission confirmed on the platform's own page: 11; partly confirmed: 2; third-party report only: 7; not yet verified: 5
- Evidence tier A (platform's own page retrieved): 12 of 25

## How to review
1. Open the workbook, sheet **Website Research**: check the evidence URL and note for each row.
2. Open **content/00_company_facts_verified.md**, then a draft. Every draft has a metadata table (title, description, category, target URL, anchor text).
3. Work through **guides/step_by_step_guide.md** one site at a time.
4. Update the **Submission Tracker** and **Link Verification** sheets with real results; the **Summary** sheet recalculates.

## Honest limitations
- Research used web search and page retrieval. No browser session, accounts, CAPTCHAs, screenshots or live-HTML inspection were available, so none were done.
- Evidence tiers: A = platform's own page retrieved; B = third-party only; C = not verified. Several exact submission URLs are marked "to be captured" because they were not seen on a retrieved page.
- No link is classed as do-follow. Only inspecting the live page's HTML can establish that, and even then a missing rel attribute does not guarantee search engines will count the link or improve rankings.
- Judgement scores (1-5) are the researcher's opinion; the weights are editable in the workbook.
- Directory and platform terms change. Re-read the sign-up page before entering details. Never pick paid options.
