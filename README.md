# Vietnamese AI Translator

This repository contains the static site for the Vietnamese-focused AI translator.

Quick notes:

- The site is a static front-end that calls the serverless translate function at `/.netlify/functions/translate`.
- Ensure the Netlify site has these environment variables set:
  - `GOOGLE_API_KEY` — Google Cloud Translate API key
  - `SITE_MAIN_TARGET` — `vi` (so the site defaults to translating to Vietnamese)

To deploy / update:

```powershell
Set-Location -Path 'C:\path\to\repo' ;
git add . ;
git commit -m "Prepare Vietnamese site" ;
git push origin main
```

On Netlify, set `SITE_MAIN_TARGET=vi` and `GOOGLE_API_KEY` in Site settings → Build & deploy → Environment.
