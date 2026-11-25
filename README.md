# River Ride · Prague to Dresden

An English, mobile-friendly cycling journal and dashboard for our group’s five riding days, **12–16 September 2027**.

## Open the app

The app is published at https://prague-dresden-river-ride.ivfisrael.chatgpt.site . Anyone with the link can open it without registering.

## Features

- Fixed five-stage itinerary; switch days to update the dashboard, map and attraction cards.
- Approximately 225 km: Prague → Mělník → Litoměřice → Děčín → Bad Schandau → Dresden.
- Interactive Leaflet map with numbered attraction markers and location links.
- Ten attraction descriptions with photographs, visit durations and access notes.
- Automatic current-day selection using Europe/Prague local time, plus shareable `#day-1` through `#day-5` links.
- Ride completion saved locally to the browser, with undo. No accounts, server or group tracking.
- Photo attribution and route-reference dialogs.

## Run locally

No build or dependency installation is required:

```sh
python3 -m http.server 8000 --directory dist
```

Then open http://localhost:8000 . Serve the `dist` directory on any static host.

## Change content

Edit `dist/data.js` for dates, distances, stage waypoints and attraction descriptions. Styles are in `dist/styles.css`; interactions are in `dist/app.js`. Photos are bundled under `dist/assets/`. All photography licences and creator credits are recorded in `dist/data.js` and accessible from the app footer. Images have been resized/compressed and are displayed cropped; their original Creative Commons licences continue to apply. Leaflet is BSD-2-Clause (see bundled licence).

## Planning limits

Overnight towns are suggested and have not been matched to booked hotels. Distances and riding times are estimates, excluding sightseeing and optional detours. Map lines connect waypoints schematically and are **not navigation tracks**. Use the operator’s confirmed GPX. Some sections share roads. Bastei requires extra walking/climbing and possibly a ferry. Check seasonal opening hours and route conditions nearer departure.

The map uses standard OpenStreetMap tiles without an API key, with visible attribution and normal browser caching. Map tiles and web fonts need internet access; offline support is not implemented. Completion is per browser, not shared between riders.

Route references: https://www.elbe-cycle-route.com/ and https://www.rueckenwind.de/en/destinations/biketours-germany/cycle-tour-prague-dresden . Content prepared November 2026.
