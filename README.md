# ForecastIQ — AI Financial Forecasting

Assumptions-driven forecasting with scenario planning, a rolling 3-year plan and revenue levers — driver-based models the finance team can steer live.

Part of the **DAMAC Finance AI Platform** (Powered by Tiger Analytics). This repository
is the standalone build of **ForecastIQ**, split out from the consolidated Finance
Transformation platform.

## Structure

```
index.html      Landing page
app.html        The ForecastIQ application
```

## Run locally

Any static file server works — the app is self-contained.

```
python -m http.server 3000
```

Then open http://localhost:3000 — the landing page links straight into the app.

## Deploy

Static site. Enable **GitHub Pages → Deploy from branch → `main` / root**; `index.html`
is served as the landing page.
