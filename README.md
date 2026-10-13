# FYPaid

Launch a coin on pump.fun and send its creator fees to any TikTok @handle.

This repo is the front-end: a single static page (`index.html`) plus the clips and coin icons in `media/`. No build step.

## Run it

Open `index.html` in a browser, or serve the folder:

```
npx serve .
```

## Deploy with GitHub Pages

Settings → Pages → Source: "Deploy from a branch" → `main` / root. The site will be live at `https://<user>.github.io/<repo>/`.

## What's simulated

Launches, the payout ticker, stats, the leaderboard and creator profiles use example data. Wallet connect uses Phantom when it's installed and falls back to a demo wallet. To make it real you need a backend that:

- creates the token through PumpPortal with a fee vault set as creator
- collects creator fees per coin
- verifies the TikTok handle (bio code check or TikTok Login)
- runs payouts to verified creators and the $FYP buyback and burn

FYPaid is independent and not affiliated with TikTok or ByteDance.
