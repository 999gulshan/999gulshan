# 🚀 Setup Guide — Gulshan's Cyberpunk Profile

Everything lives in this folder. Follow these steps to go live.

## 1. Create the profile repo

Your profile README must live in a repo named **exactly** `999gulshan` (same as your username).

```bash
# on GitHub: create a new PUBLIC repo named 999gulshan (check "Add a README")
git clone https://github.com/999gulshan/999gulshan.git
```

Then copy everything from this folder into it:

```
999gulshan/
├── README.md
├── assets/
│   ├── hero.svg          ← custom animated banner (rain, stars, particles, neon typing)
│   ├── terminal.svg      ← animated hacker terminal
│   └── footer-wave.svg   ← animated wave footer
└── .github/
    └── workflows/
        └── snake.yml     ← neon snake generator
```

```bash
git add .
git commit -m "✦ cyberpunk profile v1"
git push
```

## 2. Enable the neon snake 🐍

1. Go to the repo → **Settings → Actions → General → Workflow permissions** → select **Read and write permissions** → Save.
2. Go to **Actions** tab → select **Generate Neon Snake** → **Run workflow**.
3. It creates an `output` branch with `github-snake-dark.svg`. The README already points at it — nothing else to do. It refreshes every 12 hours automatically.

## 3. Spotify "Now Playing" (optional) 🎧

1. Visit https://spotify-github-profile.kittinanx.com/
2. Log in with Spotify and authorize.
3. It gives you your `uid` — replace `YOUR_SPOTIFY_USER_ID` in README.md.
4. The card auto-updates with whatever you're currently playing (yes, including NewJeans).

If you skip this, just delete the "Now Playing" section from README.md.

## 4. Personalize

- **Email / LinkedIn / Portfolio** links in the Connect section (`mailto:your@email.com` and the `#` placeholders).
- **Skill bar percentages** in the Tech Stack section — set them honestly, they're just text.
- **Featured Projects** — the 4 cards point to your real repos. The LIVE buttons assume GitHub Pages (`999gulshan.github.io/<repo>`); enable Pages on each repo (Settings → Pages → Deploy from branch → main) or swap the links.
- **Hero subtitle** — edit the text `FULL-STACK DEVELOPER ✦ AI ENTHUSIAST` inside `assets/hero.svg` if you want different wording.

## Notes

- All three SVGs are **hand-built, original** — pure SVG + CSS animations, no copied assets. GitHub renders SVG animations natively in READMEs.
- Stats cards (github-readme-stats, streak-stats, activity-graph, trophies) are free public services — they can occasionally be slow or rate-limited; that's normal.
- Theme tokens: background `#050505`, purple `#a855f7`, cyan `#22d3ee`, magenta accent `#e879f9`, green `#4ade80`.
