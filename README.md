# Precision Guesswork Technologies — Website

Static company site for PGT LLC. Two pages, no frameworks, no build step.

## Files
- `index.html` — home (hero / about / products / contact)
- `privacy.html` — privacy policy (covers the site + the FireLine app)
- `css/style.css` — all styles
- `README.md` — this file

## Hosting (GitHub Pages)
Deployed from the `main` branch, root folder, of the repo
`chefsquatch/pgt-website`.
- Live (Pages): **https://chefsquatch.github.io/pgt-website/**
- Privacy URL (use for the Play Store): **https://chefsquatch.github.io/pgt-website/privacy.html**

To update the site: edit the files, commit, push to `main`. Pages redeploys in ~1 min.

## FireLine APK download
The "Download APK" button points at the **latest GitHub Release asset** named
`FireLine.apk`:
`https://github.com/chefsquatch/pgt-website/releases/latest/download/FireLine.apk`
To ship a new build: create a new Release (or edit the latest) and upload the new
signed APK as an asset named exactly `FireLine.apk` — the button URL never changes.

## Custom domain (precisionguessworktech.com) — DNS steps
Do this at your domain registrar, then finish in GitHub:
1. **Apex `@` → A records** (GitHub Pages IPs):
   `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
2. **`www` → CNAME** `chefsquatch.github.io`
3. In the repo: **Settings → Pages → Custom domain** → enter `precisionguessworktech.com` → Save
   (this writes a `CNAME` file), then tick **Enforce HTTPS** once the cert issues.
4. After DNS propagates, the site is at **https://precisionguessworktech.com** — then
   update the FireLine Play listing privacy URL to
   `https://precisionguessworktech.com/privacy.html`.
