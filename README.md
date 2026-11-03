# MedLeave — Bidiya Hospital

Day-off planner for doctors. Frontend hosted on GitHub Pages, backend on Google Apps Script + Google Sheets.

## Setup
1. Deploy Apps Script as Web App (`Anyone` access).
2. Copy `/exec` URL into `index.html` → `API_URL`.
3. Push to GitHub, enable **Pages** in Settings.

## Notes
- Uses `text/plain` POST to avoid CORS preflight (Apps Script doesn't support OPTIONS).
- Auth is handled server-side: doctor by `staffNo`, admin by `ADMIN` + password from Settings sheet.
