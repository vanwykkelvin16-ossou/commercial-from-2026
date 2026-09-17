# SA Broking Services — Commercial Proposal Form

Static site, ready to deploy. One page, no build step, no dependencies, no server.

Files:
- `index.html` — the complete fillable form (fonts, logo, scripts all inlined)
- `vercel.json` — no-cache headers so clients always get the newest version
- `robots.txt` — keeps the form out of search results (delete if you want it indexed)

## Deploy — drag & drop (fastest)
1. Unzip this folder.
2. Go to https://vercel.com/new
3. Drag the folder onto the page → Deploy.
4. You get a live URL, e.g. `https://sa-broking-proposal-form.vercel.app`.

## Deploy — Git repo (best for updates)
1. Commit these files at the root of a repo.
2. Vercel → Add New → Project → import the repo.
3. Framework preset: **Other**. Build command: *(leave empty)*. Output directory: *(leave empty)*.
4. Deploy. Every push redeploys automatically.

## Custom domain
Vercel → Project → Settings → Domains → add e.g. `proposal.sabroking.co.za`,
then create the CNAME record Vercel shows you at your DNS provider.

## What the form does
- All fields typeable; dropdowns, checkboxes and signature lines work.
- **Add additional premises** / **Remove premises** — extra premises flow onto
  auto-created continuation pages, numbered Premises 2, 3, …
- **+ / X** on previous claims — same continuation behaviour.
- **Download PDF** — writes a true vector PDF (sharp text, embedded logo),
  named after the company entered on the form. No print dialog.
- **Reset form** — clears everything and removes added pages.
- Nothing is submitted anywhere; the form runs entirely in the client's browser.

## Updating
Replace `index.html` with a newer export and redeploy (or push to the repo).
