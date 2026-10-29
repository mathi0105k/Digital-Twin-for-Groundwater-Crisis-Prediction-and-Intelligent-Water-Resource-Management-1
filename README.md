# AquaTwin — Digital Twin for Groundwater Crisis Prediction

An interactive, browser-based prototype for groundwater monitoring, scenario simulation, and water-resource decision support.

## Live demo

After enabling GitHub Pages, your site will be available at:

`https://YOUR-GITHUB-USERNAME.github.io/groundwater-digital-twin/`

Replace `YOUR-GITHUB-USERNAME` with your GitHub username.

## Features

- Groundwater dashboard with illustrative well indicators
- Scenario controls for rainfall, water demand, and recharge intervention
- Forecast visualization and rule-based risk alerts
- Suggested water-conservation actions
- Responsive layout for desktop and mobile
- No build step, package installation, API key, or backend required

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Adjust the scenario controls and select **Run prediction**.

## Deploy with GitHub Pages

1. Create a public repository named `groundwater-digital-twin`.
2. Upload the files and folders in this project to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose branch `main` and folder `/(root)`, then click **Save**.
6. Wait for the deployment to finish and open the URL shown in the Pages section.

## Repository structure

```text
groundwater-digital-twin/
├── index.html
├── README.md
├── .gitignore
├── LICENSE
├── assets/
│   ├── css/
│   ├── js/
│   └── images/
└── docs/
    └── PROJECT_OVERVIEW.md
```

The current prototype is intentionally self-contained: its styling and JavaScript are embedded in `index.html`, so the `assets/css` and `assets/js` folders are reserved for future refactoring.

## Important limitations

This is a demonstration prototype. The readings and monitoring-area visuals are synthetic, and forecasts use simplified scenario calculations. It is **not** a validated hydrological model and must not be used for operational water-management or emergency decisions.

## Future development

- Connect verified groundwater and rainfall datasets
- Add a Python/FastAPI backend and persistent database
- Train and validate a time-series forecasting model
- Add a real monitoring-well map and data provenance
- Report uncertainty alongside forecasts

## Suggested technology stack for future versions

- Frontend: HTML, CSS, JavaScript
- Backend: Python and FastAPI
- Data analysis: pandas, NumPy, scikit-learn
- Database: PostgreSQL or SQLite for a small demo
- Deployment: GitHub Pages for the frontend; a separate backend host if APIs are added
