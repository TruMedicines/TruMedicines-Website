# TruMedicines / TelePacks — Website

A static marketing site for TruMedicines' TelePacks Ai-Managed Medication Dispenser.

## Structure

All files live in the root — no subfolders:

```
index.html
style.css
main.js
logo.jpg
device-silver.png
packets.jpg
dr.jpg
nurse.jpg
avatar.jpg
```

No build step — it's plain HTML/CSS/JS.

## Run locally

Just open `index.html` in a browser, or serve it:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000

## Deploy to GitHub Pages

1. Create a new GitHub repo (e.g. `trumedicines-website`) and push these files to the `main` branch.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to "Deploy from a branch," branch `main`, folder `/ (root)`.
4. Save — GitHub will publish at `https://<your-username>.github.io/<repo-name>/`.
5. To use `www.trumedicines.com`, add a `CNAME` file at the repo root containing just `www.trumedicines.com`, and point your domain's DNS (CNAME record) to `<your-username>.github.io`.

## Editing content

- Copy and section content lives in `index.html`.
- Colors, type, and layout tokens are defined at the top of `assets/css/style.css` under `:root`.
- Replace images in `assets/img/` with higher-resolution versions when available — the current photos are the ones provided in the source materials.
