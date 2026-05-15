# Central IA Soil Temperatures

Live 4″ soil-temperature chart for Central Iowa (BOOI4 — Boone, IA), pulling
daily data from the [Iowa State Soil Moisture Network](https://mesonet.agron.iastate.edu/agclimate/).

The page plots the current season vs. a rolling 10-year average and shows
accumulated Soil Growing Degree Days (base 50 °F) on a secondary axis. The
historical window automatically rolls forward each year — it's always the
10 calendar years before the year currently selected.

## View it

Once GitHub Pages is enabled, the chart is available at:

**https://mckechnieshelena.github.io/CentralIA_Soil_Temps/**

## What's on the chart

- **Blue line** — this year's daily 4″ soil-temperature average
- **Gray dashed** — 10-year daily average (the prior 10 years)
- **Gray band** — min/max envelope across those 10 years
- **Red dotted** — 50 °F (corn-planting threshold)
- **Solid orange** — this year's accumulated Soil GDD (right axis)
- **Dashed orange** — 10-year average Soil GDD (right axis)

## Data source

All values come live from
`https://mesonet.agron.iastate.edu/cgi-bin/request/isusm.py` — no caching,
no backend, no API key. Fetched in the browser using CORS.

Window: March 15 – June 30 each year. Station: `BOOI4`.

## Local development

It's a single static HTML file. Open `index.html` in any modern browser, or
serve the folder with any static server.
