# n8n-deploy
# n8n Render Deployment

This repo is a minimal setup to deploy n8n on [Render](https://render.com).

## Steps to Deploy

1. Fork this repo to your GitHub account.
2. Go to Render → New + → Web Service → Connect to your fork.
3. Choose **Environment = Docker**.
4. Add Environment Variables:
   - `N8N_BASIC_AUTH_ACTIVE=true`
   - `N8N_BASIC_AUTH_USER=admin`
   - `N8N_BASIC_AUTH_PASSWORD=yourpassword`
   - `WEBHOOK_TUNNEL_URL=https://<your-render-url>/`
5. Click **Deploy** and wait for the build.
6. Open the Render URL → login with your credentials.

## Notes
- Change the default username and password in Render Environment settings.
- You can connect your workflows to Google Sheets, YouTube API, etc.
- Free Render instances sleep after inactivity; upgrade for 24/7 availability.
