# PolicyMitra Complete Website

Files are arranged for Node.js hosting:
- `server.js` — web server + lead API
- `public/index.html` — customer website
- `public/admin.html` — protected lead dashboard
- `public/advisor-photo.png` — supplied advisor photo
- `leads.json` — local development storage
- `.env.example` — admin secret configuration

## Deploy
Use Node.js 18+. Start command: `npm start`.
Set a strong `ADMIN_TOKEN` environment variable on the hosting platform.

## Important
For production customer leads, replace local JSON storage with a managed database and add rate limiting/backups. Keep secrets out of GitHub. Do not collect Aadhaar, PAN, bank credentials or other sensitive documents through this basic enquiry form. Final privacy/consent and insurer/agency compliance wording should be reviewed before launch.

## Notifications
This package stores leads and provides an admin dashboard. Email and WhatsApp notifications should be connected using your own approved provider accounts and secrets on the hosting platform; never place API keys in frontend files or GitHub.
