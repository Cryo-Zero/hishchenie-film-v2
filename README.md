# HISHCHENIE FILM V2

Clean rebuild of the official film website.

## Principles
- No inherited P14–P22 DOM/CSS/JS.
- Desktop-first visual system based on the approved 2045 public-system design.
- Global symmetric content grid; only ARCHIVE may leave the grid and use the left browser wall.
- Author film assets are kept separate from profile/world UI assets.
- Reviews/Supabase are intentionally disconnected in this foundation release.

## Local preview
Run any static server from repository root, for example:

```bash
python -m http.server 8080
```

Open `http://localhost:8080`.

## Next stage
1. Visual QA against approved mockup.
2. Freeze desktop layout.
3. Create V2 Supabase schema + RLS + anonymous auth.
4. Add realtime reviews, Turnstile, rate limiting, admin moderation.
5. Mobile adaptation.
