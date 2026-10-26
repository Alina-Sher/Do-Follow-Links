# Beginner Step-by-Step Guide: Submit, Record, Screenshot, Check

Work on ONE website at a time, in the order of the Rank column. Budget about 20-40 minutes per site.

## Before you start (once)
1. Create a free work email alias for submissions (for example marketing@ your company domain) and use the same name, address and phone on every site.
2. Open `content/00_company_facts_verified.md`. Ask management to confirm every [CONFIRM] item.
3. Create a folder on your computer for screenshots and keep it open.

## For each website
**Step 1 - Open the official site.** Use the "Official URL" and "Exact submission URL" in the Website Research sheet. If the exact URL says "to be captured", start from the homepage and find the "Add / List your company" or "Write for us" button, then paste the real URL you land on into the Tracker (Confirmation / draft URL).

**Step 2 - Confirm it is free.** Read the sign-up or pricing page. If any step asks for payment or a paid plan, choose the free/basic option only. If there is no free option, STOP, set Status = Unavailable, screenshot the page, move on.

**Step 3 - Screenshot the free evidence** (address bar visible). Name it `WS-01_clutch_free_evidence.png` using the ID and site name.

**Step 4 - Sign up.** Use the company email alias. Do not reuse an important password. Complete any email verification. If a CAPTCHA appears, solve it yourself.

**Step 5 - Open the draft** in `content/` for that site. Read it, replace every [CONFIRM], [AUTHOR NAME] and [ROLE] with real information, and edit articles into the author's own voice. Only publish articles under the real author's account.

**Step 6 - Fill in the form.** Paste the text. Add https://www.techabout.com/ (or the target URL in the metadata table) as the website. Do not add fake reviews, clients, awards or numbers.

**Step 7 - Submit and screenshot the confirmation.** Save as `WS-01_clutch_confirmation.png`. In the Tracker set Status to Submitted (or Pending Review), enter the date and the confirmation URL.

**Step 8 - Wait for approval.** Many sites take days. Check your email. If rejected, copy the reason into Notes, set Status = Rejected, and move on.

**Step 9 - When it is live, record the real URL.** Open the live page in a fresh browser tab, copy the exact address from the address bar into the Tracker column "Published URL", and set Status = Approved/Live.

**Step 10 - Screenshot the live page.** Show the full address bar and the TechAbout name/link. Save as `WS-01_clutch_published.png`.

**Step 11 - Check the link attribute.**
1. On the live page, right-click the TechAbout link and choose **Inspect** (Chrome/Edge/Firefox).
2. A panel shows the HTML, something like `<a href="https://www.techabout.com/" rel="nofollow">TechAbout</a>`.
3. Look for `rel=`. If it contains `nofollow`, `sponsored` or `ugc`, the link is qualified. If there is no `rel` at all (or other values like `noopener`), enter `none`.
4. If the link is added by script or you cannot inspect it, enter `cannot inspect`.
5. Click the link to confirm it opens https://www.techabout.com/ and set "Link clickable?" = Yes.
6. Screenshot the HTML panel: `WS-01_clutch_link_html.png`.

**Step 12 - Update the Link Verification sheet.** Fill the yellow cells. The "Final classification" column and the Summary sheet update automatically. Only a row with a recorded URL, a clickable link and rel = none becomes "Confirmed do-follow".

## Rules to remember
- Never enter a status you have not actually achieved.
- Never pay, never buy links, never create fake accounts or reviews.
- Never edit screenshots to change what they show.
- A missing rel attribute does not guarantee that search engines will count the link or raise rankings.
- When you finish a batch, tell me the real results and I will prepare the next batch of candidates and content.
