# ForecastIQ — AI Financial Forecasting

Assumptions-driven forecasting with scenario planning, a rolling 3-year plan and revenue levers — driver-based models the finance team can steer live.

Built by **Tiger Analytics** and styled to the Tiger Analytics design system (brand colour
scales and typographic hierarchy). This repository is the standalone build of **ForecastIQ**.

## Demo dataset

The application is client-neutral and runs entirely on synthetic data modelled on a **US
consumer packaged goods / retail group** — roughly **$14B of FY2026 net sales** across six
brand platforms (Hydration & Beverages, Better-for-You Snacks, Packaged Foods, Home Care,
Personal Care, Pet Nutrition) plus a Foodservice & AFH stream. All amounts are **USD**.

The seeded storyline: 77% of the forecast is already committed through customer POs and
joint business plans; a Q3 liquidity trough emerges as the holiday inventory build coincides
with Packaged Foods receivables running behind after a top-3 mass customer moved to 75-day
terms. Every figure recomputes live from the Assumptions sheet and the scenario Equalizer.

## Structure

```
index.html      Landing page
app.html        The ForecastIQ application (self-contained: markup, styles, model, agents)
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

## Design system

Colours come exclusively from the Tiger Analytics scales — Gray (neutral foundation),
Brand Primary orange, and the Success / Warning / Error semantic ramps — declared as CSS
custom properties at the top of `app.html` and referenced by every component. Typography maps
to the h2–h6, subtitle1/2, body1/2, caption and overline hierarchy, exposed both as element
styles and as `.ta-*` utility classes. Spacing follows a standard 4px grid.
