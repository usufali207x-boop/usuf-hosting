# USUF HOSTING — Publish Ready

## Before going live
1. Change the admin password in `users.json` from `CHANGE_THIS_ADMIN_PASSWORD`.
2. Set a strong `SECRET_KEY` environment variable.
3. Do not commit real passwords, tokens, or bot files to a public Git repository.

## Render
- Create a new Web Service.
- Connect the repository.
- Build: `pip install -r requirements.txt`
- Start: `gunicorn app:app`

## Search engines
After deployment, open:
- `/robots.txt`
- `/sitemap.xml`

Then add the public domain to Google Search Console and submit `/sitemap.xml`.
Google indexing can take time and is not guaranteed immediately.
