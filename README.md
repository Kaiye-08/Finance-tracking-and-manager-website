# ArthaFlow

A lightweight personal finance dashboard built as a single-page HTML app. It helps you plan your monthly budget, track spending, model loan repayments, and assess your financial health without needing a backend or account setup.

## Overview

ArthaFlow is designed for people who want a simple way to:

- set a monthly income
- split spending into needs, wants, and savings
- log real transactions
- compare planned vs actual spending
- model home or business loans
- estimate a basic financial health score

Everything is stored locally in the browser using `localStorage`, so your data stays on your device unless you export or back it up manually.

## Features

### Budget planning
- Fixed salary or irregular income mode
- Assign categories like rent, groceries, transport, and savings
- Switch between percentage-based and fixed-amount budgeting
- Visual summary of how much money is left to allocate

### Spending tracking
- Add transactions by date, category, and description
- See planned vs actual spending for the selected month
- Review recent transaction history
- Compare spending trends across recent months

### Loan modeling
- Add home or business loan entries
- Input principal, rate, and term
- Calculate EMI and total interest paid
- Simulate extra monthly or lump-sum prepayments
- View year-by-year loan schedules

### Financial health score
- Measures savings rate, debt burden, and emergency runway
- Gives simple health feedback and suggested next steps

## Tech stack

This project is intentionally simple and uses:

- HTML
- CSS
- JavaScript

No framework, server, or database is required.

## Project structure

```text
Finance-tracking-and-manager-website/
├── arthaflow.html   # Main app file
├── README.md        # Project documentation
└── .gitignore       # Optional repo hygiene file if added later
```

## Run locally

Because this is a static HTML project, you can open `arthaflow.html` directly in a browser or serve it locally.

### Option 1: Open directly
- Double-click `arthaflow.html` in your file explorer
- Or open it in your browser using File > Open

### Option 2: Run a local server
```bash
cd Finance-tracking-and-manager-website
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000/arthaflow.html
```

## Deploy with GitHub Pages

This repo is ready for GitHub Pages.

### Recommended setup
1. Go to the repository on GitHub
2. Open **Settings**
3. Open **Pages**
4. Select **Deploy from a branch**
5. Choose the `main` branch and the `/root` folder
6. Save

Your site will be available at:

```text
https://<your-username>.github.io/Finance-tracking-and-manager-website/arthaflow.html
```

If you'd like it to open at the root URL instead of the file name, rename `arthaflow.html` to `index.html`.

## Privacy and data notes

- Data is saved in the browser via `localStorage`
- It is not synced to a server
- It is not encrypted
- It is not backed up automatically
- You should export or back up important data if needed

## Disclaimer

ArthaFlow is intended for planning and educational use. It does not replace professional financial or tax advice. Tax notes are general summaries and may not reflect official rules for your country and situation.

## License

This project currently does not include a formal license file. If you plan to share or reuse it publicly, consider adding one such as MIT or Apache-2.0.

## Author

Kaiye-08

## Contributing

Pull requests and suggestions are welcome. If you want to improve the app, consider adding features such as:

- CSV export/import
- recurring budgets
- debt payoff strategies
- multi-currency summaries
- dark mode polish and accessibility enhancements
