# Screenshot Evidence Checklist

Save only real screenshots from a real browser session. Never edit, mock up or reuse a screenshot for another site.

## Naming (use the workbook ID)
`WS-01_clutch_confirmation.png`, `WS-01_clutch_published.png`, `WS-01_clutch_link_html.png`
Optional: `WS-01_clutch_free_evidence.png`

## For EACH site, capture
- [ ] **Free evidence** - the sign-up/pricing page showing the option you chose is free (no payment step). Browser address bar visible.
- [ ] **Confirmation** - the "submitted / under review" message or confirmation email (hide personal data and passwords).
- [ ] **Published page** - the live page with the full URL visible in the address bar and the text "TechAbout" visible.
- [ ] **Link visible** - the TechAbout link on that page (hover to show the destination in the status bar if possible).
- [ ] **Link HTML** - DevTools open on the `<a>` tag showing href and any `rel=` value.

## Quality rules
- [ ] Text is readable at 100% zoom; crop only to remove clutter, never to hide a rel attribute or a payment prompt.
- [ ] Date/time visible if possible (system clock) or note the date in the tracker.
- [ ] One set of screenshots per site; filenames match the tracker columns.
- [ ] Nothing shows passwords, API keys, private emails or card numbers.

## If a site rejects or needs payment
Screenshot the rejection or the payment prompt, set the tracker status to Rejected or Unavailable, and move on. Do not pay.
