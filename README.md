# Smart Budget System

A browser-based budgeting tool for tracking a spending period, estimating a daily spending allowance, monitoring expenses, and setting aside money toward wishlist goals.

## Features

- **Daily spending estimate:** Recalculates an indicative daily allowance from the remaining budget and days left in the current cycle.
- **Expense tracking:** Record spending and view category-level summaries.
- **Analytics:** Visualize spending patterns with Chart.js.
- **Wishlist goals:** Track savings targets and the funds allocated toward them.
- **Cycle rollover:** Carry eligible balances into a new budgeting period.
- **Data export:** Download data in JSON or CSV formats for backup or further analysis.
- **Browser-based storage:** The current app stores budgeting data in browser `localStorage`.

## Technology

- HTML, CSS, and JavaScript
- Tailwind CSS
- Chart.js
- Phosphor Icons
- Browser LocalStorage API

## Run locally

This is a static web application; no build step is required.

```bash
git clone https://github.com/nksdev/smart-budget-system.git
cd smart-budget-system
```

Open `index.html` in a modern browser, or serve the directory locally:

```bash
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

## How to use

1. Set the budget period, total budget, and applicable fixed costs.
2. Add expenses as they occur.
3. Review the recalculated daily allowance and analytics.
4. Create wishlist goals and track allocations.
5. Export a backup regularly.

The displayed daily limit is a budgeting aid, not financial advice. Verify the calculations against your own requirements before relying on them.

## Data and privacy

Budget data is stored in the browser profile on the device. It is not automatically synced across browsers or devices. Clearing site data or browser storage may remove it, so use the export feature to keep backups. This storage design is not a substitute for encrypted storage on a shared or compromised device.

## Security

The repository includes client-side input handling, but a browser-only app cannot guarantee protection against every injection, browser extension, or device compromise. Do not describe it as “XSS-proof” or use it to store highly sensitive financial information without further review.

## Maintainer

[Naman Kumar Sonker](https://github.com/nksdev)

## License

See [LICENSE](LICENSE).
