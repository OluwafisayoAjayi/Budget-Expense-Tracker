# Everyday Budget & Expense Tracker

An independent, mobile-friendly website for household budgeting and daily expense tracking. No county-level data or third-party libraries are needed.

## Features
- Monthly budget calculator with grouped dropdown categories for housing, mortgage, utilities, food, transportation, medical expenses, credit cards, insurance, debt, family, savings, and more. Each category can be used multiple times with a description.
- Budget summary in an expandable section, a single monthly budget doughnut/pie chart, balance and savings coverage.
- Daily spending log with date, category, amount, and note; recent transactions and running daily/monthly totals.
- Monthly budget snapshot history and a daily spending trend.
- Print or save results as PDF using your browser's Print dialog; download a budget CSV, daily expenses CSV, or complete JSON backup. Import a prior JSON backup to restore/merge.
- Local browser storage only. No login, account, remote database or online synchronization.

## Publish as a separate GitHub Pages website
1. On GitHub, create a **new public repository** named `Everyday-Budget-Expense-Tracker` (or another name).
2. Upload `index.html`, `style.css`, `script.js`, and this `README.md` into the new repository root.
3. Under **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. The expected site address will be `https://YOUR-USERNAME.github.io/Everyday-Budget-Expense-Tracker/` if the repo name matches.

Do not place these files inside the old dashboard repository if you want them to be separate websites.

## How it works
- All monthly expenses are summed; monthly balance = entered monthly take-home income minus entered monthly expenses.
- Savings coverage = entered emergency savings / entered monthly expenses; if no expenses are entered, coverage is marked not applicable.
- Budget chart includes entered spending categories and positive remaining balance, but the negative balance is shown in the summary instead of as a pie slice.
- Daily transactions are **not** automatically added to planned expenses; doing that would double count items such as groceries and rent. Daily entries show actual spending, while budget snapshots show the plan.
- Saving a second budget for the same month creates another snapshot; monthly trend charts show the most recently saved snapshot for each month.

## Privacy and persistence
Stored locally using `localStorage`. Browser data deletion, device changes, and private browsing can remove data. Back up JSON regularly. Importing a JSON backup merges records based on their IDs. This is a personal planning aid, not financial advice.
