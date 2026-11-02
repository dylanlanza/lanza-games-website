# Lanza Games website

The home page for Lanza Games, a small studio making pixel games that run in the browser.

Live at **https://lanza-games.netlify.app**

## What's here

| File | What it is |
| --- | --- |
| `index.html` | The home page: logo, featured game, screenshots, about section |
| `driftwood-dock.html` | The playable Driftwood Dock game, served at `/driftwood-dock` |
| `shot-*.png` | Screenshots of each fishing area, used on the home page |

Everything is plain HTML, CSS and JavaScript with no build step. Fonts load from Google Fonts.

## Run it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy

The site is hosted on Netlify (project `lanza-games`). To publish changes from this folder:

```bash
npx netlify-cli deploy --prod --dir . --site 6d9988de-f232-465f-9985-7d7bb858e2d0
```

## Adding a game

1. Add the game's page to this folder (for example `my-game.html`).
2. Add a card for it in the `#games` section of `index.html`.
3. Deploy.

The game's own source lives in its own repo; the Driftwood Dock source is in the `driftwood-dock` repo.
