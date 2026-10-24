EDUFEES — INSTALLABLE SCHOOL FEE MANAGEMENT APP
================================================

CONTENTS
- index.html: responsive app interface
- app.js: student, fee, receipt, report and backup logic
- manifest.webmanifest: installable app details
- sw.js: offline app shell
- icons/: app icons

IMPORTANT
This app stores records in local browser storage on one device/browser profile.
It has no cloud sync, authentication, server database or online payment processing.
Do not use real sensitive student data for production without proper security, access
controls, backups, and a suitable database.

HOW TO RUN ON A COMPUTER
1. Extract the ZIP.
2. You need to serve the folder using HTTPS or localhost for PWA install/offline features.
   If you have Python installed, open a terminal in the extracted folder and run:
       python -m http.server 8000
3. Open http://localhost:8000 in your browser.
4. Use your browser's install option if available.

HOW TO INSTALL ON ANDROID
1. Upload/extract this folder to a static hosting service that provides HTTPS
   (for example, a static site host you control).
2. Open the HTTPS website in Chrome on Android.
3. Open the browser menu and tap "Install app" or "Add to Home screen".
   The wording depends on your browser/device.
4. Open EduFees from the home screen.

HOW TO HOST
Upload the contents of the ZIP, keeping the folder structure, to any static hosting
provider that supports HTTPS. The site must be served from the root of the uploaded
folder (or the manifest/service-worker paths must be adjusted for a subfolder).

FEATURES
- Add/edit/delete students
- Student class, roll number and annual fee
- Record payments and calculate balances
- Receipt view and print
- Student/payment CSV exports
- JSON backup and restore
- Dashboard and pending fee reports
- Local persistence and offline app shell after first successful load
- School name and currency settings

DATA BACKUP
Use "Export backup" regularly. Imported backups replace the current local records.
Deleting browser site data may erase app records. CSV exports are for reports and are
not a full restorable backup.
