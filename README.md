# Budget Tracker

A simple budget tracker. Switch a bill on when you pay it and the date is filled in for you.
Your budget is saved on your own device. Nothing is sent anywhere.

## What you see

- **Status strip:** budget selector, month, today's date, and a health light. Green means nothing needs attention. Amber means a bill is due within 3 days or everyday spending is over budget. Red means a bill is overdue.
- **Month summary and donuts:** bills paid, money in, and everyday spending at a glance.
- **Schedule:** the month's due dates by week.
- **Planned vs actual spending:** six months ending with the month shown. The actual line fills in as you mark bills paid and enter spending.
- It follows your phone's light or dark setting.

## Put it online with GitHub Pages (free)

1. On github.com, create a new repository (for example `budget-tracker`). Make it **Public**.
2. Upload these files to it: `index.html`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`.
3. Open **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose branch **main** and folder **/ (root)**, then **Save**.
4. After a minute or two the page shows your address, `https://YOUR-USERNAME.github.io/budget-tracker/`.

## Install it on an iPhone

1. Open the address in **Safari**.
2. Tap **Share**, then **Add to Home Screen**.
3. Open it from the new icon.

## Several budgets

Use the selector at the top to switch between budgets. Tap **Manage** to create a new empty budget, rename one, or delete one.
Each budget is a separate set of items and payments. Nothing is shared between them.

**Back up** saves the open budget to its own file, named with the budget (for example `budget-smith-household-2026-11-12.json`).
**Restore…** reads a file and asks where it should go: a new budget, or an existing one.
For an existing budget you can **Replace** everything in it, or **Merge** to add and update items while keeping the rest.
The name inside the file is used to suggest the match, so a file for one budget lands on that budget by default.

## Your own bills

This repository is public, so the app starts empty. Do **not** commit your real budget here.

To load your own items, save your private backup file (for example `my-budget-import.json`) to iCloud Drive or send it to your phone,
then open the app and tap **Restore…**. Tap **Back up** now and then to keep a fresh copy of each budget.

## Notes

- Data lives in the browser on that device and is not encrypted. A different phone or browser starts empty until you Restore a backup.
- Updating the app: edit and re-upload `index.html`. If a change doesn’t appear, close and reopen the app.
