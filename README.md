# example-graph

Static single-page app for tracking exercise progress over time.

## Features

- Runs as a plain GitHub Pages friendly SPA
- Stores exercises and measurements in IndexedDB
- Tracks named exercises such as `Bicep Curl` and `One-armed Row`
- Shows dashboard summaries and per-exercise weight graphs
- Calculates growth rate from the first and latest measurements for each exercise

## Local usage

You can open `index.html` directly in your browser (`file://.../index.html`) with
no local server. The app will use IndexedDB when available and automatically
fall back to localStorage when IndexedDB is unavailable.

If you prefer testing over HTTP:

```bash
cd example-graph
python3 -m http.server 8000
```

Then open `http://127.0.0.1:8000`.

## GitHub Pages

Publish the repository's `githubpages` branch with GitHub Pages and browse the
deployed URL directly without running any server locally. This repository uses
`githubpages` as its configured Pages source branch name.
To update that branch from your working branch, merge or cherry-pick your
changes into `githubpages` and push it before opening the site URL.