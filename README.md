# Michi's Rides — Show Tracker

A single-page web app for tracking ride classes and estimating when Michi is up
next at a cutting/ranch show. All state is stored locally in the browser
(`localStorage`), so nothing is sent anywhere and it works offline once loaded.

The whole app lives in [`index.html`](./index.html) — no build step, no
dependencies.

## Hosting on GitHub Pages

This repo deploys to GitHub Pages automatically via the
[`.github/workflows/pages.yml`](./.github/workflows/pages.yml) workflow whenever
the `main` branch changes.

One-time setup (repo owner):

1. Go to **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **GitHub Actions**.

After that, every push to `main` publishes the site. The live URL will be:

```
https://jacktysonss.github.io/show-tracker/
```

You can also trigger a deploy manually from the **Actions** tab
(**Deploy to GitHub Pages → Run workflow**).

## Running locally

Just open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```
