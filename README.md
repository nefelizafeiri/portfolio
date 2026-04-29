# Nefeli Zafeiri — Portfolio

Personal portfolio site. Built with [Quarto](https://quarto.org), styled with
custom SCSS, and auto-deployed to GitHub Pages on every push to `main`.

**Live site:** https://nefelizafeiri.github.io/portfolio/

## What's on the site

- **Hero** — name, MSBA at the University of Miami, contact links
- **Education** — University of Miami Herbert Business School (MSBA, May 2026); University of Central Oklahoma (BBA International Business, May 2025)
- **Experience** — Graduate Assistant, Athletic Department Finance, Research Assistant, Beverage Distribution Operations
- **Projects** — Deloitte capstone (AI wildfire risk monitoring), Chart Reasoner (Phi-3 fine-tune), SQL Agent, Coffee Big Data, Time Series Forecasting, Customer Prediction with XGBoost & SHAP, Monthly Budget App
- **Activities** — Deloitte DIRPA scholar, MSBA cohort representative, NCAA varsity tennis, SAAC, Greek National Tennis Team
- **Skills** — Python, SQL, pandas, scikit-learn, XGBoost, SHAP, PyTorch, Hugging Face, PySpark, statsmodels, Streamlit, Tableau, Power BI, Git

## Repo layout

```
portfolio/
├── nefeli-website/         # Quarto source — see its README for dev instructions
│   ├── _quarto.yml         # Site configuration
│   ├── index.qmd           # Main page (hero, sections, projects)
│   ├── capstone.qmd        # Deloitte capstone detail page
│   ├── styles.css          # Custom SCSS / styling
│   ├── headshot.jpg
│   └── docs/               # Generated output (created by `quarto render`)
└── .github/workflows/      # GitHub Actions — auto-deploy to Pages on push to main
```

## Development

See [`nefeli-website/README.md`](nefeli-website/README.md) for local preview
and deployment notes.

## License

The site's code (Quarto files, SCSS) is personal — feel free to look around for
inspiration. The content (resume, photos, project descriptions) is not licensed
for reuse.
