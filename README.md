# Pulse Cloud Sync — Actual Working Build

## GitHub Pages
Upload ONLY `index.html` to the root of your GitHub Pages repository.

## Supabase
1. Create a Supabase project.
2. SQL Editor → New query.
3. Paste all of `supabase_schema.sql`.
4. Run it.
5. In Supabase → Project Settings → API, copy Project URL and Publishable/anon key.
6. Open Pulse → ☁ Cloud Setup.
7. Paste both values → Connect.
8. Create your account or sign in.
9. Use the same account on your phone and laptop.

## Important
Do not use a service_role/secret key in Pulse.

This build uses explicit JavaScript event listeners (no inline onclick handlers), so the buttons work reliably when hosted by GitHub Pages.
