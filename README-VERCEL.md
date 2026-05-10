# Hailite Xteriors — Vercel static version

Required files at the root of the GitHub repo:
- index.html
- admin.html
- site-content.json

How it works:
1. Vercel serves index.html.
2. admin.html lets you add photos/projects, controlled reviews, and blog cards.
3. admin.html exports site-content.json.
4. Upload site-content.json to GitHub beside index.html.
5. Vercel redeploys automatically.

Important: this admin page is a local editor/exporter, not a secure CMS. It avoids Cloudflare and backend setup.


## Admin password

Default admin password:

```
Hailite2026!
```

To change it, open `admin.html` and search:

```
const ADMIN_PASSWORD = "Hailite2026!";
```

Replace the password inside the quotes.

Important: this is a simple static-site password gate. It is useful to avoid casual access, but it is not a true secure server-side login.


## Admin button removed from public site

The public `index.html` no longer shows an Admin button or link.

The file `admin.html` still exists in the project for private/manual use, but visitors will not see a direct button to it from the website.
