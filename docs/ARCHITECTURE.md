# V2 architecture

## Frontend
Vanilla HTML/CSS/JS. No build step and no external runtime dependency.

## Asset boundaries
- `assets/film/` — official/author film content only.
- `assets/profile/` — generated anonymous profile avatars.
- future `assets/world/` — non-canonical system/UI world assets only.

## Backend (next stage)
New Supabase project: `hishchenie-film-v2`.
Backend is intentionally not connected in the foundation build so that layout and interaction bugs can be isolated from network/database bugs.

## Review model planned
- anonymous Supabase auth
- profile keyed to `auth.uid()`
- one review per user
- rating 0–10
- optional text
- realtime subscription
- server-side rate limit
- CAPTCHA / Turnstile gate
- RLS denying cross-user edits
- admin account separated from anonymous users
- admin panel not linked in public navigation
