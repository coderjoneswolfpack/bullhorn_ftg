# Financial Talent Group Bullhorn Portal (GitHub Pages)

This folder was reconstructed from the live Bullhorn OSCP site assets.

## Publish on GitHub Pages
1. Create a new public GitHub repo, for example `ftg-bullhorn-portal`.
2. Upload all files in this folder to the repo root.
3. In GitHub: **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** `main` and `/ (root)`
5. Save, then wait a minute for Pages to publish.
6. Your site will be available at:
   `https://<github-username>.github.io/ftg-bullhorn-portal/`

## Optional custom domain
If you later want `jobs.financialtalentgroup.com`, add a file named `CNAME` in the repo root with:
`jobs.financialtalentgroup.com`

Then in GitHub Pages settings set the custom domain, and add the DNS record with the domain owner.

## Webflow embed
Point your iframe or button to the GitHub Pages URL first. Example:
```js
const SRC = "https://<github-username>.github.io/ftg-bullhorn-portal/";
```

## Notes
- The portal config is in `app.json`.
- The job search service uses Bullhorn corp token `BGWSW1` on swimlane `43`.
- The old WordPress site was only hosting static assets. This package removes the WordPress dependency.
