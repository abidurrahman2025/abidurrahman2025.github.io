# Abidur Rahman — Portfolio

Personal portfolio for **Abidur Rahman**, a senior Information Science student at the University of South Florida (Data Science & Analysis concentration).

**Live site:** https://abidurrahman2025.github.io

The site showcases data analysis, forecasting and web projects, with case studies, a résumé, and an interactive real estate calculator.

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Home: introduction and featured projects |
| `about.html` | Background, interests and profile links |
| `resume.html` | Education, skills and selected projects (printable) |
| `projects.html` | Overview of all six projects |
| `project.html` | Case study for each project |
| `contact.html` | Contact details |
| `real_estate_calculator.html` | Interactive mortgage, affordability, ROI and rental-yield tool |

## Features

- **Responsive layout:** a sidebar menu on desktop that becomes a top bar on phones.
- **Light and dark themes:** follows the visitor's device setting. No toggle needed.
- **Accessible colors:** text and interface colors meet the WCAG AA contrast target of 4.5:1.
- **Printable résumé:** `resume.html` prints cleanly, without the menu.
- **No build step:** plain HTML and CSS. Nothing to install.

## Project structure

```
.
├── index.html
├── about.html
├── resume.html
├── projects.html
├── project.html
├── contact.html
├── real_estate_calculator.html
├── styles.css
└── .nojekyll
```

`styles.css` holds all shared styles, including the color tokens at the top and the dark-mode overrides at the bottom. `.nojekyll` tells GitHub Pages to serve the files exactly as written.

## Running locally

Open `index.html` in a browser, or run a local server from this folder:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Publishing to GitHub Pages

1. Make sure the repository is named `abidurrahman2025.github.io` and is public.
2. Upload every file in this folder to the root of the repository's default branch.
3. In the repository settings, open **Pages** and confirm the source is the default branch, root folder.
4. Wait a minute or two, then visit https://abidurrahman2025.github.io.

## Real estate calculator

`real_estate_calculator.html` is a standalone single-page app. It contains:

- **Mortgage:** monthly principal and interest, tax, insurance and PMI, with total interest and payoff date.
- **Affordability:** the highest home price that fits a debt-to-income limit, solved directly rather than estimated.
- **Investment ROI:** a year-by-year projection with rent and expense growth, financing, appreciation and selling costs. Returns are annualized (IRR).
- **Rental yield:** gross and net yield, vacancy loss, and cash flow after the mortgage.
- **Loan schedule:** a yearly summary and a monthly CSV download.
- **Share link and print:** every input can be copied into a link, and each results page can be printed.

Assumptions such as tax, insurance, PMI and closing costs are estimates, set in the shared assumptions panel. The calculator is for planning and exploration. It is not financial, tax or lending advice.

The calculator loads Chart.js and Font Awesome from public CDNs, so it needs an internet connection to draw its charts.

## Contact

- Email: abidurrahman@usf.edu
- LinkedIn: https://www.linkedin.com/in/abidur-rahman-b394593a3/
- GitHub: https://github.com/abidurrahman2025
