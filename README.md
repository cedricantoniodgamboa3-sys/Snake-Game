# Slitherper.io 🐍

A Slither.io × Paper.io browser game. Steer your snake, loop back home to capture territory, and outlast the bots. One HTML file, no build step, no dependencies.

## Features

- Large circular arena with smooth, curved trails and rounded territory edges
- Territory capture with combos and a frenzy meter
- 14 AI rivals with difficulty levels, plus boss bots
- 8 game modes: Classic, Time Attack, Coin Rush, Battle Royale, Boss Hunt, Survival, Domination, Team Battle
- 7 maps, 28 skins with rarities, base decorations
- Upgrades, 8 equippable skills, power-ups, Golden Rush events
- Daily login, daily spin, quests, weekly missions, monthly season pass, prestige
- Installable app with offline play; keyboard, mouse and touch controls; progress saved in the browser (localStorage)

## Controls

| Input | Action |
| --- | --- |
| Mouse / WASD / arrows | Steer |
| Click / Space / Shift | Boost |
| 1-3 | Use skills |
| P / Esc | Pause |
| F / M / wheel | Fullscreen / mute / zoom |
| Touch | Drag to steer, BOOST button |

## Install as an app

The game is a Progressive Web App, so players can install it with its own icon and play offline.

- **Android / Chrome / Edge (desktop):** tap the **📲 Install app** button on the main menu, or use the browser's install option.
- **iPhone / iPad (Safari):** tap Share, then **Add to Home Screen**.

Needs HTTPS, which GitHub Pages provides. After you deploy an update, bump `CACHE` in `sw.js` (for example `slitherper-v2`) so installed copies refresh.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

## Publish on GitHub Pages

1. Create a new repository on GitHub (for example `slitherper`).
2. Push these files:

   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<your-username>/slitherper.git
   git push -u origin main
   ```

3. In the repo, go to **Settings → Pages**, set **Source** to **GitHub Actions**.
4. The included workflow deploys on every push to `main`. Your game will be live at `https://<your-username>.github.io/slitherper/`.

Prefer no Actions? In **Settings → Pages**, choose **Deploy from a branch**, pick `main` and `/ (root)` instead, and you can delete `.github/`.

## License

MIT. See [LICENSE](LICENSE) and replace `[YOUR NAME]` with yours.
