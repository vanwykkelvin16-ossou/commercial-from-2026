# Commercial Proposal Form — deploy to Vercel

Static site, one file: `index.html` (fully self-contained — fonts, logo and scripts are inlined).

## Option 1 — drag & drop (fastest)
1. Go to https://vercel.com/new
2. Drop this folder onto the page.
3. Vercel returns a live URL, e.g. `https://sa-broking-proposal-form.vercel.app`.

## Option 2 — Git repo (best for updates)
1. Create a repo and commit this folder's contents at the root.
2. Vercel → New Project → import the repo.
3. Framework preset: **Other**. Build command: *(empty)*. Output directory: *(empty / root)*.
4. Deploy — every push redeploys.

## Notes
- No build step, no dependencies, no server needed.
- The form runs entirely in the browser; nothing is submitted anywhere.
- To update, replace `index.html` with the latest export and redeploy.
