# example-graph

Static single-page app for tracking exercise progress over time.

## Features

- Runs as a plain GitHub Pages friendly SPA
- Stores exercises and measurements in IndexedDB
- Tracks named exercises such as `Bicep Curl` and `One-armed Row`
- Shows dashboard summaries and per-exercise weight graphs
- Calculates growth rate from the first and latest measurements for each exercise

## Local usage

Because the app uses IndexedDB, serve the repository over HTTP instead of opening
the file directly:

```bash
cd example-graph
python3 -m http.server 8000
```

Then open `http://127.0.0.1:8000`.