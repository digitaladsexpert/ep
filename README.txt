ElitePips Netlify ZIP
=====================

Contents:
- index.html             -> Main landing page (interactive question + confirm)
- go/redirect.html       -> Intermediate redirect page that logs clicks and then redirects to Telegram
- README.txt             -> This file

How to deploy on Netlify (simple):
1. Unzip and upload this folder as a new site on Netlify (Drag & Drop ZIP or connect repo).
2. Netlify will serve index.html at the root.
3. When users click "Proceed", they are taken to /go/redirect.html which logs and redirects to Telegram.

Optional improvements:
- Add a Netlify Function at /.netlify/functions/logClick to store click logs (see Netlify docs).
- Replace client-side logging in redirect.html with server-side logging or a call to a webhook you control.
- Add Cloudflare Turnstile or hCaptcha to further reduce bot traffic.

Notes:
- The Telegram link in redirect.html and index.html is set to: https://telegram.me/+ZVpxPGfP6LFiZDFl
- If you want me to add a Netlify Function (serverless) for logging clicks, tell me and I will add a sample function file.
