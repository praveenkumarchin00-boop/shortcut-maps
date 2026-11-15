# Shortcut Maps — Beta

Mobile-friendly map and road-route comparison for India.

## Features
- OpenStreetMap map with Leaflet
- Search places in India using Nominatim
- Select starting point and destination by searching or tapping the map
- Optional current location
- Compare routes returned by OSRM, sorted by distance
- Responsive interface and basic web app manifest

## Safety and accuracy
**This is an early beta, not a production-ready motorcycle navigation system.** The current router uses a driving profile, not a motorcycle-specific legal-access profile. “Shortest” means shortest among returned alternatives; it does not guarantee the globally shortest legally accessible road route. OpenStreetMap may omit small roads or restrictions. Follow road signs and local traffic laws.

The public Nominatim, OpenStreetMap tile and OSRM demo endpoints are shared services with usage limits and no production availability guarantee. Dedicated infrastructure is required for larger-scale public use.

## Run
With Node.js 20 or later:

```sh
npm start
```

Open http://localhost:3000. Railway provides the PORT environment variable automatically.

## Next milestones
- Validate website availability and route searches on Android
- Replace public demo services with production-capable map/search/routing infrastructure
- Build legal two-wheeler routing with turn restrictions and permitted U-turns
- Benchmark shortest-distance route coverage on mapped Indian roads
- Add complete PWA icons, offline shell, and browser tests

Map data © OpenStreetMap contributors.
