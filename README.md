# Repwise Gym ERP – static site

A single-page, self-contained site (`index.html`). No build step, no server code.
The only external resource is Google Fonts; everything else is inline.

## Deploy

**Netlify:** drag this folder (or the zip) onto app.netlify.com/drop. `netlify.toml` is included.

**Vercel:** `npx vercel` inside this folder, or import it in the dashboard (framework: "Other"). `vercel.json` is included.

**GitHub Pages:** push these files to a repo → Settings → Pages → deploy from branch, root folder.

**cPanel / Hostinger / any Apache host:** upload the contents to `public_html/`. `.htaccess` is included.

**Nginx:** copy to your web root (e.g. `/var/www/repwise`) with `index index.html;`.

## Local preview
`python3 -m http.server 8080` → open http://localhost:8080

## Notes
- Navigation uses URL hashes (`#dashboard`, `#members`, …), so no rewrite rules are needed.
- The data shown is sample/demo data held in the page; nothing is saved to a server.
