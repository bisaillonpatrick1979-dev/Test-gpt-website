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


## Mot de passe admin corrigé

Mot de passe actuel:

```
Hailite2026!
```

Après upload dans GitHub, ouvre:

```
/admin.html?v=2
```

Cela force le navigateur à charger la nouvelle version.


## Services + project albums

This version adds:
- brighter service/project images
- clickable service cards with example galleries
- clickable project cards with swipeable albums
- admin supports selecting multiple photos for one project

For a real project album:
1. Open admin.html
2. Choose multiple photos in "Photos du projet / album"
3. Export site-content.json
4. Upload site-content.json to GitHub beside index.html
5. Vercel redeploys


## Real service example photos

The service galleries were updated with product-specific example photos:
- vinyl siding
- soffit & fascia / eaves lining
- Hardie Board / fiber cement style siding
- metal/architectural cladding
- roofing shingles

Most examples are loaded remotely from Wikimedia Commons or public image sources. Replace these with your own project photos later for the most professional final version.

## Admin blur fix

The admin password screen no longer blurs the entire page.  
Password remains:

```
Hailite2026!
```

After replacing files in GitHub, test with:

```
/admin.html?v=3
```
