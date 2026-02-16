# MotionTale Pro — landing (waitlist)

Static GitHub Pages landing for **MotionTale Pro** (motion control: photo + reference video → animated output).

## What’s included

- Clean header + CTA
- Upload UI (photo + reference video)
- **Login to generate** → Supabase Google OAuth
- After login: **“We added you to the waitlist”** section
- Avatar in header when available (Google metadata)

## Configure Supabase

This landing expects Supabase keys to be injected as globals. For simple deployment on GitHub Pages, you can edit `index.html` and set:

```js
const SUPABASE_URL = 'https://YOURPROJECT.supabase.co';
const SUPABASE_ANON_KEY = 'YOUR_ANON_KEY';
```

Also make sure in Supabase:

- Authentication → URL Configuration → **Redirect URLs** includes the deployed page URL, e.g.
  - `https://<user>.github.io/motiontale-pro/`

## Deploy to GitHub Pages

- Repo settings → Pages → Deploy from branch → `main` / `/ (root)`

## Notes

This page does **not** upload files to a backend yet. It’s a waitlist MVP.
