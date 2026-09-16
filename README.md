# Health Buddies

Open `index.html` in any modern browser for the interactive demo. It includes the dashboard, fun animal profiles, session-based health check-ins, and appointments.

## Use the Google Sheets database

1. Upload `Health_Buddies_Database.xlsx` to Google Drive, then open it in Google Sheets.
2. Choose **Extensions → Apps Script**, replace the existing project code with `Code.gs`, then create a new deployment version of the same private Web app.
3. Paste the deployment URL into `SCRIPT_URL` near the top of `app.js`.
4. The Appointments tab must remain in this same spreadsheet. Health records and appointments are sent to separate tabs through the same endpoint.
5. Keep the spreadsheet and deployed endpoint shared only with trusted family members.

The app confirms a save only after the Apps Script endpoint responds successfully. If the endpoint is unreachable, it shows an error instead of claiming the record was saved.
