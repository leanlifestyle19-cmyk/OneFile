# OneFile

Small business tools that live in a single file. No login, no subscription, no cloud — open in any browser, works offline, your data stays on your device.

## Live site

`index.html` is the storefront. Once GitHub Pages is on, the site is at:

```
https://<yourusername>.github.io/<reponame>/
```

## How it's structured

Every file sits at the top level, in one flat folder. The store links to each tool by filename as a sibling, so **don't move the tools into subfolders** — the demo links will break.

## The tools

| File | What it does |
|------|--------------|
| `quote-generator.html` | Type line items, get a clean PDF quote |
| `payment-tracker.html` | Track invoices, see overdue, generate a polite reminder |
| `price-list-maker.html` | A tidy PDF price list in minutes |
| `booking-confirmation.html` | Deposit + balance confirmation slip as a PDF |
| `order-manager.html` | Every order in one place, sorted by collection time |
| `day-sheet.html` | The day's bookings on one printable page |
| `takings-tracker.html` | Log sales and expenses, see today's net, export CSV |
| `session-fee-tracker.html` | Track lessons per student and what's owed |
| `rebooking-reminders.html` | Nudge regulars overdue for a visit |
| `loyalty-card.html` | A digital stamp card for the shop phone |
| `order-page.html` | A shareable "link in bio" shopfront for home bakers |
| `cake-enquiry-form.html` | Turns a vague DM into a tidy order brief |
| `cake-price-calculator.html` | Price custom cakes from real costs |
| `bake-plan.html` | Turn the week's orders into a bake schedule + shopping list |
| `review-collector.html` | Ask for reviews and keep the testimonials |

## Hosting (GitHub Pages)

1. Create a public repo and upload every file to the root.
2. Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
3. Wait ~1–2 minutes, then open the URL above.

## Before going live

- Replace the placeholder checkout buttons in `index.html` (`href="#"`, marked `data-buy`) with your own purchase links.
- Set your own prices.
- Each tool stores data in the browser's `localStorage`, so it's per-device and per-browser — nothing syncs between devices. This is intentional, but tell customers so they're not surprised.

## Tech

Plain HTML, CSS, and vanilla JavaScript. No build step, no dependencies, no external requests. Each file is fully self-contained.