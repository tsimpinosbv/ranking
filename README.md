# Hosting on GitHub Pages — Weekly Excel Update Guide

No coding or command line needed — everything below is done through the GitHub website.

---

## STEP 1 — Create a GitHub account (skip if you have one)

Go to **github.com** → Sign up → free account.

---

## STEP 2 — Create a new repository

1. Click the **+** icon (top right) → **New repository**
2. Repository name: e.g. `vathmologia-2026`
3. Set it to **Public** (required for free GitHub Pages)
4. Leave everything else default → **Create repository**

---

## STEP 3 — Upload the two files

1. On your new (empty) repository page, click **"uploading an existing file"** (blue link in the middle of the page)
2. Drag in both files from the `netlify_package` folder I gave you:
   - `index.html`
   - `Ranking_2026.xlsx`
3. Scroll down → **Commit changes**

---

## STEP 4 — Turn on GitHub Pages

1. In your repository, go to **Settings** (top tab)
2. Left sidebar → **Pages**
3. Under "Build and deployment" → Source: **Deploy from a branch**
4. Branch: select **main** (or `master`), folder: **/ (root)** → **Save**
5. Wait ~1 minute, refresh the page — you'll see a green box with your live URL:
   `https://your-username.github.io/vathmologia-2026/`

That's the link you send to players.

---

## STEP 5 — Weekly update (the part you'll do every week)

1. Update `Ranking_2026.xlsx` on your computer with the new tournament results (same filename, same column structure as before)
2. Go to your repository on github.com
3. Click on **`Ranking_2026.xlsx`** in the file list
4. Click the **pencil icon (✏️ Edit)** — actually for a binary file like .xlsx, instead do this:
   - Click **Add file → Upload files** (top right of the repo file list)
   - Drag in the new `Ranking_2026.xlsx` — GitHub will detect it has the same name and offer to **replace** the existing one
   - Scroll down → **Commit changes**
5. Done. The live site updates automatically within ~30–60 seconds — no redeploy step needed, GitHub Pages picks it up on its own.

Players just refresh the page (or tap the "Ανανέωση" button inside the app) to see the new totals.

---

## Notes specific to GitHub Pages

- The file must stay named exactly **`Ranking_2026.xlsx`**, in the **same folder** as `index.html` (repository root) — same rule as before.
- GitHub Pages is free forever for public repositories, no time limit, no login required for visitors.
- If you'd rather use git commands instead of the web upload button (faster for frequent updates, but requires installing Git), let me know and I'll give you that workflow instead — but the web upload method above needs zero setup.
- Custom domain (e.g. `vathmologia2026.gr` instead of the `github.io` address) is possible later via Settings → Pages → Custom domain, if you ever want that.

## If GitHub feels like too much

The Netlify Drop method from before is genuinely simpler for pure drag-and-drop weekly updates with no account navigation required beyond the Deploys tab — it's a valid choice too. Both host the exact same `index.html` + `Ranking_2026.xlsx` pair, so you can try either (or both) without changing anything in the app itself.
