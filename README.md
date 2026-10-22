# Everyday Budget & Expense Tracker — expanded edition

An independent, accessible, responsive static budgeting website with no build dependencies. The application works with GitHub Pages.

## Features

- Monthly take-home budget calculator with customizable expense rows, including car-free transportation (bus, train, transit pass, bike share, rideshare).
- Optional **gross** household income for a housing-cost assessment using 30% and 50% descriptive thresholds. Calculation combines entered housing and utility costs as an approximation; it is **not** an official determination, eligibility assessment, or eviction prediction.
- Monthly pie/doughnut chart, expandable input summary, CSV downloads and browser print-to-PDF.
- Daily expense logging, quick category buttons, editing amounts, deleting entries, and CSV export.
- Monthly budget and daily spending history, locally saved in browser, with export/import of a JSON backup.
- Recurring bill calendar-style upcoming reminders (only shown when page is opened; no notifications).
- Personal savings goal, progress bar, and hypothetical what-if analysis.
- State-selected support finder for all 50 states plus Washington, D.C. based on official national directories and 211, with select additional state-level links. **Does not assert that local programs are funded or accepting applications.**

## Publish

1. Extract the ZIP and upload **index.html**, **style.css**, **script.js**, **README.md** to the root of your GitHub repository. (Do not upload the outer folder unless you want it to be part of the URL.)
2. In GitHub **Settings → Pages**, set source to **Deploy from branch**, branch **main**, folder **/(root)**.
3. Open `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/` after deployment completes.

## Privacy and limitations

Data is stored in browser `localStorage`. It is not shared with a server, and will not automatically transfer between browsers, devices, or private sessions. Download JSON backups regularly. Results should be checked with professionals for financial/legal decisions. State and local program eligibility, funding, and application windows change and must be verified directly on the linked provider's website. No live state assistance database is connected. This site is not financial, legal, or benefits advice.

## Assistance directory maintenance (important)

The public `assistance-programs.json` file is a **static curated directory**, not a live service. Resources shown as “Official source reviewed” had their linked official page reviewed on October 22, 2026; this does **not** verify that an assistance application is currently accepting submissions, that funds remain, or that a household qualifies. Entries not individually reviewed remain labeled “Not verified”. The state selector covers all 50 states plus DC through the national LIHEAP, HUD, SNAP and 211 directories; state-specific curated entries are currently limited to MA, ME, NY, CA, and TX. Do not misrepresent national directory links as individual state program confirmations.

To update: inspect official program pages, confirm URLs and latest rules directly, add or update the entries in `assistance-programs.json`, record the actual review date and source verification status, and publish a new commit. For **current application status**, check a dated agency notice, and avoid asserting an open window from a general program page. A static GitHub Pages site cannot monitor closures or intake changes automatically.

The directory searches locally in the browser and never transmits a user's budget or ZIP input to any of the linked providers.


## ZIP-based local assistance search
Enter a state and optional five-digit ZIP code. The page opens area-specific searches on partner/referral sites, including 211, Findhelp, HUD, LIHEAP, and food-bank locators. **It does not retrieve a verified list of nearby agencies into the page or verify applications are open**, because those provider systems do not offer a public cross-directory live API for this static site. Nearby listings and availability must be checked directly on provider sites. No financial data is transmitted by this website.

All fields on the monthly calculator are optional; blank expense lines are ignored. For a meaningful balance add take-home income; for housing burden add gross income and housing expense(s). Previous browser data is retained using the same localStorage key.
