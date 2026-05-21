# MenuMines Marketing Site

## What This Is

Static marketing site for MenuMines, a macOS menu bar Minesweeper app. Single `index.html` file deployed on GitHub Pages.

## Tech Stack

- Plain HTML, no framework
- Tailwind CSS v4 via `@tailwindcss/cli`
- JetBrains Mono font via Google Fonts
- Build: `npm run build:css` (or `npm run dev` for watch mode)

## Architecture

Everything lives in `index.html`. The page sections in order:

1. Hero - ASCII art logo + tagline
2. App preview - Interactive-looking game grid mockup + download CTAs
3. Features - Three cards (daily puzzle, stats/streaks, accessibility)
4. Screenshots - Four game state mockups (fresh, victory, game over, stats)
5. Controls - Keyboard shortcut reference
6. FAQ - Four Q&A items
7. Final CTA - Download buttons
8. Footer - Links to privacy policy, support, press kit

## Styling Conventions

- Dark background gradient: `#1a1a2e` -> `#16213e` -> `#0f3460`
- Primary buttons: purple gradient `#667eea` -> `#764ba2`
- Glass-morphism cards: `rgba(255,255,255,0.05)` with `backdrop-blur`
- All text uses JetBrains Mono
- Custom component styles live in `src/styles.css` alongside the Tailwind import
- Standard Tailwind utility classes are used in `index.html`
- Built CSS output goes to `dist/styles.css` (committed for GitHub Pages)

## Development

```sh
npm install
npm run dev
```

Open `index.html` directly or use any static file server. The `dev` script watches for changes and rebuilds `dist/styles.css`.

## Deployment

GitHub Pages from the `main` branch. Push to `main` to deploy.
