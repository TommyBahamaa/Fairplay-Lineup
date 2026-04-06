# ⚾ FairPlay Lineup Generator

A free, mobile-friendly lineup generator for youth baseball and softball coaches. Generates fair lineups that rotate batting order and field positions across games so every kid gets equal opportunity.

## Features

- **Fairness Engine** — Automatically balances batting order and field positions across all games played
- **Absence Tracking** — Toggle players in/out for any game (sick, travel, etc.) 
- **Fairness Dashboard** — Visual proof that every player is getting equal treatment
- **Game History** — Full archive of every lineup generated
- **Manual Overrides** — Swap batting order or positions after generating
- **Works Offline** — Install to your phone's home screen as a PWA
- **No Account Needed** — Data stays on your device via localStorage

## How to Use

### Option 1: Use the hosted version
Visit: **https://TommyBahamaa.github.io/Fairplay-Lineup**

### Option 2: Host it yourself
1. Fork this repo
2. Go to Settings → Pages → Source: Deploy from branch → `main` / `root`
3. Your site is live at `https://YOUR-USERNAME.github.io/fairplay-lineup`

### Install on Your Phone
1. Open the link in Safari (iPhone) or Chrome (Android)
2. Tap **Share → Add to Home Screen** (iOS) or the install banner (Android)
3. It now works like a native app, even offline

## How the Fairness Algorithm Works

Each time you generate a lineup, the engine:

1. **Tracks position history** — Counts how many times each player has played each position across all saved games
2. **Assigns positions to minimize imbalance** — Players who've played a position the least get priority for it
3. **Tracks batting order history** — Calculates each player's average batting position
4. **Assigns batting order to equalize** — Players who've batted lower in past games get moved up
5. **Adds controlled randomness** — Small noise prevents predictable patterns while maintaining fairness

## Tech Stack

Pure HTML + React 18 (via CDN) + localStorage. No build step, no server, no dependencies to install.

## License

MIT — Free to use, modify, and share.
