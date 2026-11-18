# SpendSense — iPhone-first expense tracker

## Included in this first build
- Add, categorise and view expenses
- Monthly totals, daily average and category breakdown
- Basic insights based on recorded expenses
- Paste a copied Gmail transaction email or SMS, review parsed details, then confirm
- Duplicate check for imported transactions
- CSV export
- Local browser storage; no server calls or bank credentials

## Install on iPhone (no Mac)
This is a Progressive Web App (PWA). It must be served from an HTTPS website for Add to Home Screen and offline caching to work.

1. On your iPhone, open Safari and sign in to GitHub (or use a computer later if convenient).
2. Create a new public or private repository named `spendsense`.
3. Upload the four files in this folder to the repository root: `index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`.
4. In the repository, open Settings → Pages. Choose deploy from branch, select `main` and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish. Open the published HTTPS URL in Safari.
6. Tap Share → Add to Home Screen → Add.

You can also deploy these files to any static HTTPS host. Do not publish transaction data; this project contains only app code.

## Important limitations
- Gmail auto-sync is not implemented in this starter. It needs a Google OAuth consent setup and Gmail read-only API integration. Never put a Google client secret in browser code.
- iOS does not allow a web app to read the iPhone Messages inbox. Copy/paste selected alerts instead.
- Data is stored in Safari's local browser storage on this device. Export CSV backups regularly. Clearing website data may erase it.
- This is a personal tracking tool, not a bank connection or financial-advice product.
