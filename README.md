# Jira Table Modify Tool

A lightweight static web app for converting pasted table data (Excel, Google Sheets, pipe-separated text, or multi-space text) into Jira Wiki Table format.

## Features

- Convert tabular input to Jira Wiki syntax instantly
- Optional first-row header conversion (`||header||` style)
- Auto-convert mode while typing
- One-click copy output to clipboard
- Sample data loader for quick testing

## Run Locally

Because this project is a static site, you can run it directly in a browser:

1. Open `index.html`.

Or serve it with a local static server:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploy To GitHub Pages

This repository includes a GitHub Actions workflow at `.github/workflows/deploy.yml` that deploys the site to GitHub Pages whenever code is pushed to `main`.

### One-time setup

1. Push this repository to GitHub.
2. In GitHub, go to **Settings -> Pages**.
3. Under **Build and deployment**, set **Source** to **GitHub Actions**.
4. Push to `main` (or run the workflow manually from the Actions tab).

After the workflow succeeds, your site will be available at:

`https://<your-username>.github.io/jira-table-modify-tool/`

## Project Structure

- `index.html`: app UI and conversion logic
- `.github/workflows/deploy.yml`: automatic GitHub Pages deployment