# ElitePips Landing Page (GitHub Pages)

This repo contains a single landing page `index.html` which implements:
- A single-question funnel UI
- Meta pixel integration
- Deep-link to Telegram (tries app first, then web fallback)
- FOMO-style thank-you content

## How to deploy on GitHub Pages (quick)

1. Create a new GitHub repository (e.g. `elitepips-landing`).
2. Add `index.html` to the repository root and commit.
3. Push to GitHub:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Add landing page"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
4. Enable GitHub Pages:
   - Go to the repository > Settings > Pages.
   - Source: `main` branch and `/ (root)` folder.
   - Save — your site will be published at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Notes / Testing
- Test the published URL on mobile (iOS and Android). The "Join" button will attempt `tg://join?...` URI first.
- For Meta Ads use: put the GitHub Pages URL as the landing page in your ad. Meta preview will open the HTML page (not a direct t.me link).
- If you want a custom domain, add `CNAME` file and configure DNS to point to GitHub Pages.

If you want, I can also:
- Create the GitHub repo for you (you'll need to provide access/token)
- Generate a ZIP with these files (ready to upload) — already prepared here.
