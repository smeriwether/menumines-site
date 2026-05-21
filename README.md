# MenuMines Marketing Site

Marketing website for [MenuMines](https://menumines.com), a macOS menu bar app for daily Minesweeper puzzles.

## Overview

MenuMines gives you one Minesweeper puzzle every day, right in your menu bar. The same board is generated for everyone on Earth, so you can compare times with friends.

This repo contains the static marketing site, currently deployed on **GitHub Pages**. MenuMines is available on the [Mac App Store](https://apps.apple.com/us/app/menumines/id6769579671).

## Tech Stack

- Plain HTML (single `index.html`)
- [Tailwind CSS](https://tailwindcss.com) v4 (built via CLI)
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/) font via Google Fonts

## Local Development

```sh
npm install
npm run build:css
open index.html
```

To rebuild CSS on changes:

```sh
npm run dev
```

## Deployment

The site is deployed via [GitHub Pages](https://pages.github.com/) from the `main` branch. Pushing to `main` triggers a deploy automatically.

`dist/styles.css` is committed to the repo so GitHub Pages can serve it directly.

## Project Structure

```
.
├── src/
│   └── styles.css    # Source CSS (Tailwind + custom styles)
├── dist/
│   └── styles.css    # Generated output (committed for GitHub Pages)
├── app-store-badge.svg # Official App Store download badge
├── index.html        # The marketing page
├── package.json
└── README.md
```
