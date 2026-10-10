# VB Blue Insurance Agency Reporting Site

Static, self-contained performance report hub for VB Blue Insurance Agency, deployed on Vercel.

## Structure

- `index.html` is the report hub linking six reports: campaign overview, Auto and Home campaign pages, SEO audit, and two Virginia research reports
- `VB-Blue-VA-ZIP-Data-10-10-26.csv` is the ZIP-level data behind the research reports
- `vercel.json` — Vercel config: clean URLs, security headers, `noindex` so the report stays out of search engines

## Deploying

No build step. In Vercel, import this repo with:

- **Framework Preset:** Other
- **Build Command:** *(leave empty)*
- **Output Directory:** *(leave empty — serves the repo root)*

Or from the CLI: `vercel --prod`

## Updating the report

Replace `index.html` with the new export and push to `main`; Vercel redeploys automatically.
