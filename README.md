# Lanza Games website

The home page for Lanza Games, a small studio making pixel games that run in the browser.

Live at **https://lanza-games.netlify.app**

## What's here

| File | What it is |
| --- | --- |
| `index.html` | The home page: logo, a cartridge for each game, screenshots, about section |
| `driftwood-dock.html` | The playable Driftwood Dock game, served at `/driftwood-dock` |
| `lanza-solitaire.html` | The playable Lanza Solitaire game, served at `/lanza-solitaire` |
| `lanza-lines.html` | The playable Lanza Lines game, served at `/lanza-lines` |
| `shot-*.png` | Screenshots used on the home page: each Driftwood Dock fishing area, plus `shot-solitaire.png` and `shot-lines.png` |

Everything is plain HTML, CSS and JavaScript with no build step. Fonts load from Google Fonts.

## Run it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy

The site is hosted on Netlify (project `lanza-games`) and deploys automatically: every push to `main` publishes to https://lanza-games.netlify.app within a minute or so.

```bash
git add -A
git commit -m "Describe the change"
git push
```

Deploy history is at https://app.netlify.com/projects/lanza-games/deploys.

## Adding a game

1. Add the game's page to this folder (for example `my-game.html`).
2. Add a card for it in the `#games` section of `index.html`.
3. Deploy.

Each game's own source lives in its own repo (`driftwood-dock`, `lanza-solitaire`, `lanza-lines`). The copy on this site is the same file plus a small "← Lanza Games" link at the top.
