# Sentinel map prototype

A clickable prototype of the next Sentinel dashboard map. Open the live page:

**https://widei.github.io/sentinel-map-prototype/**

## What it shows

- Real US state geography on a dark basemap, filled by a five-step scale of alert counts for the week.
- Click a state to open its counties. Alerts appear as proportional circles, coloured by tier, with a white ring at five or more. Hover any circle for the county, count and leading threat category.
- **Tiles** shows the same week on Sentinel's current state tile cartogram, for side-by-side comparison.
- **Globe** switches to a globe projection with the same layers attached.
- The time slider narrows the window from the start of the week. There is no auto-play by design.
- The **Ask Sentinel** panel contains five scripted prompts that move the map. It demonstrates how the Sentinel agent will drive the map in the product. No AI runs in this prototype.

## Data

Sentinel alerts for 27 August to 2 September 2026, aggregated to county level. Counts only; no organisation, user or record details are included.

## Status

Prototype only. Not the production design, not connected to the Sentinel application.
Built with MapLibre GL JS and deck.gl. Basemap © CARTO © OpenStreetMap contributors.

## Shareable links

The address bar follows the view, so any link opens exactly what you were looking at:

- https://widei.github.io/sentinel-map-prototype/#state=KS opens on Kansas
- https://widei.github.io/sentinel-map-prototype/#state=KS&county=20091 zooms to Johnson County, Kansas
- https://widei.github.io/sentinel-map-prototype/#view=tiles opens the tile cartogram
- https://widei.github.io/sentinel-map-prototype/#globe=1 opens the globe
- Add `&days=3` to narrow the window, or `&layer=cat` to colour by top category
