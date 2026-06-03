# watchitnow.today — off-season landing

Single static page shown while the scraper is paused. Lives on GitHub Pages, mapped to `watchitnow.today` via DNS.

## Files
- `index.html` — the landing page (self-contained, no build step)
- `CNAME` — tells GitHub Pages the custom domain is `watchitnow.today`

## Deploy

1. Push this folder to a public GitHub repo (e.g. `watchitnow-offline`)
2. GitHub → Settings → Pages → Source: **Deploy from a branch** → Branch: `main`, Folder: `/ (root)` → Save
3. Wait ~1 minute. Pages will publish at `https://<username>.github.io/<repo>/`
4. Once `CNAME` is detected, set custom domain to `watchitnow.today` (auto-filled from file)
5. Update DNS — see parent `CLAUDE.md` for the apex A records

## Update the message

Edit `index.html` → commit → push. Pages re-deploys in ~30 seconds.
