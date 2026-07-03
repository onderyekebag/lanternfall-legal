# Lanternfall — Legal pages (Privacy Policy + Terms)

Static, self-contained HTML. Host free on **GitHub Pages** and paste the URL into Play Console.

## Files
- `index.html` — Privacy Policy (this becomes the URL Play Console needs)
- `terms.html` — Terms of Service (optional but recommended)

## Free hosting — GitHub Pages (5 min)
1. Create a **public** GitHub repo, e.g. `lanternfall-legal`.
2. Upload `index.html` and `terms.html` to it (web UI: "Add file → Upload files", or git push).
3. Repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main` / folder `/root` → Save.
4. Wait ~1 min. Your policy URL is:
   `https://<github-username>.github.io/lanternfall-legal/`
   (Terms: `.../lanternfall-legal/terms.html`)
5. Open it to confirm it loads.

### git push alternative
```bash
cd ~/Desktop/moto/lanternfall-legal
git init && git add . && git commit -m "Lanternfall legal pages"
git branch -M main
git remote add origin https://github.com/<user>/lanternfall-legal.git
git push -u origin main
# then enable Pages in repo Settings
```

## Where the URL goes in Play Console
- **Play Console → your app → Policy → App content → Privacy policy** → paste the `index.html` URL.
- **Store listing** can also link it.

## Before editing
Update the contact email / developer name in both HTML files if needed
(currently: Kyrzma · ykbgonder@gmail.com).

## Other free hosts (if you prefer)
- Netlify / Cloudflare Pages / Vercel — drag-and-drop the folder.
- Google Sites — paste the text into a page.
