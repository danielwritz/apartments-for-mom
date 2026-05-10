# Triangle Apartment Shortlist — GitHub Pages

Self-contained interactive viewer for 14 Raleigh / Cary / Morrisville 2BR/2BA apartments under $1,500/mo. Drop on GitHub Pages and you have a shareable URL.

## Files

- `index.html` — the entire app (HTML + CSS + JS inline). No build step, no dependencies.
- `.nojekyll` — tells GitHub Pages to skip its Jekyll preprocessor (just serve the file as-is).

## Deploy in ~3 minutes

### Option A: GitHub Pages (free, real URL, easy updates)

1. Go to <https://github.com/new> and create a new repo. Name it something like `raleigh-apartments`. Make it **Public** (Pages requires public unless you have a paid account).
2. Skip the "initialize with README" option — you'll upload these files instead.
3. On the new empty repo page, click **uploading an existing file** (the link in the quick setup section).
4. Drag the entire contents of this `github-pages/` folder (`index.html`, `.nojekyll`, and this README) into the upload area. Commit them.
5. Go to **Settings → Pages** in the repo.
6. Under "Build and deployment," set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
7. Wait ~30 seconds. GitHub will show a green "Your site is live at https://YOUR-USERNAME.github.io/raleigh-apartments/" banner.

That URL is what you share. Anyone who opens it sees the page — no install, no login.

### To update the data later

1. Get an updated `index.html` (just edit and save).
2. In the repo on GitHub, click `index.html` → the pencil/edit icon → paste the new content → commit.
3. Wait ~30 seconds, refresh the URL. Your viewers refresh their tab and see the new data.

(Or if you prefer command line: `git clone`, edit, `git push`. Same outcome.)

### Option B: Netlify Drop (no account needed for first deploy)

1. Go to <https://app.netlify.com/drop>.
2. Drag this entire `github-pages/` folder onto the drop zone.
3. You instantly get a URL like `https://random-words-1234.netlify.app/`. Share that.
4. Updating: drag a new folder over to redeploy. The URL stays stable if you create a Netlify account and "claim" the site.

GitHub Pages is better long-term (stable URL, version history). Netlify is faster for "I just need a link in 60 seconds."

## Notes

- The `index.html` is fully self-contained: all CSS and JavaScript are inline. Nothing loads from a CDN. So it'll work offline once downloaded, and there are no broken-link risks over time.
- The "View Listing" buttons link to apartments.com pages, which can change or expire. If a listing 404s, the property has been delisted — call the leasing office or search by name.
