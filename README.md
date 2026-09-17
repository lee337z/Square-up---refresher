# Square Up — Skills Refreshers (Railway deploy)

Static single-page site. Progress saves to the visitor's browser (localStorage).

## Deploy to Railway

1. Create a GitHub repo and upload both files in this folder (`index.html`, `nixpacks.toml`).
2. Railway → **New Project → Deploy from GitHub repo** → select the repo.
3. Railway builds it automatically using `nixpacks.toml`.
4. **Settings → Networking → Generate Domain** → gives you the public `*.up.railway.app` link.

## Alternative: Railway CLI

```
npm i -g @railway/cli
railway login
railway init
railway up
railway domain
```

Run these from inside this folder.

## Note on progress saving

Progress (lessons viewed, quiz scores, badges) saves per browser via localStorage — it does not sync across devices or tie to a user account. To make it per-account, it needs wiring to your existing Supabase auth and a `refresher_progress` table on the main Square Up app.

## Before going live

Course content is drafted but **not SME-reviewed**. The electrical and plumbing calculations need licensed-practitioner sign-off, and the disclaimer wording needs legal review for your states of operation.
