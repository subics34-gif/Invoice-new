# Invoice Pro — first working PWA build

## Included
- Mobile-responsive React + TypeScript interface
- Dashboard with calculated local data
- Customer creation and deletion
- Invoice creation/editing, multiple line items, tax and paid amount
- PDF invoice downloads
- Invoice search, status and deletion
- Expense tracking
- Basic cash reports and CSV export
- Business name setting
- Light/dark mode
- JSON backup export/import
- PWA manifest, service worker and icons
- GitHub Actions workflow for GitHub Pages

## Important limitations
This is a local-first MVP. Records are stored in the current browser on the current device. There is no cloud sync, real login, MongoDB backend, online payment processing, subscription activation, email sending, estimates workflow, product catalogue, or production admin panel yet. The plan screen is informational only. No payment is collected.

Export backups regularly. Do not rely on browser local storage as the only copy of important business records.

## Run
Install Node.js 20+, then run:
`npm install`
`npm run dev`

Build:
`npm run build`

## GitHub Pages
1. Create a GitHub repository named `invoice-pro`.
2. Upload all files and push to branch `main`.
3. In GitHub repository Settings → Pages, select GitHub Actions as the source.
4. Wait for the Actions workflow to finish.
5. Open the Pages URL.

If your repository has another name, change `/invoice-pro/` in `vite.config.ts` to `/<your-repository-name>/`.

## iPhone installation
Open the deployed URL in Safari → Share → Add to Home Screen.

## Next production stages
Add an Express backend, MongoDB Atlas, authentication, secure business ownership, cloud file storage, estimate/product/reminder workflows, and server-verified subscription payments. Complete a security and financial-calculation review before commercial launch.
