# NervBox Game Data (GitHub Pages)

This repo hosts static game data for the NervBox homepage.

## Endpoints

Published on GitHub Pages root:

- `/featured_worlds.json`
- `/news.json`
- `/version` (plain text, 10-char hash of `featured_worlds.json` + `news.json`)

## Update workflow

1. Edit `featured_worlds.json` and/or `news.json`.
2. Commit and push to `main`.
3. GitHub Actions deploys the new files to Pages and regenerates `/version` from the JSON content hash.

## One-time repo setup

In GitHub repository settings:

1. Open `Settings -> Pages`.
2. Set `Source` to `GitHub Actions`.
