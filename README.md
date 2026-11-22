# LEE IT Website

A responsive four-page static website for leeit.me. No build dependencies or backend required.

## Pages
- `index.html` — Home
- `services.html` — Services
- `projects.html` — Project photography
- `contact.html` — Contact (`z@leeit.me`)

## Preview locally

From the repository folder, run `python -m http.server 8000`, then open http://localhost:8000/.

## Publish with GitHub Pages

1. Create a GitHub repository (e.g. `leeit-website`) and upload all contents of this folder to its root, keeping `.nojekyll` and `CNAME`.
2. In GitHub repository **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)`, then save.
3. In **Settings → Pages**, confirm the custom domain is `leeit.me` and enable **Enforce HTTPS** once available.
4. In Porkbun DNS, point the apex `@` GitHub Pages A records to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`. Optionally point `www` CNAME to `<YOUR_GITHUB_USERNAME>.github.io` after replacing the placeholder with your actual user name. Remove conflicting `@` website A/AAAA records before adding new ones.
5. **Important**: retain ALL existing iCloud Custom Email records (MX, SPF/TXT, DKIM CNAME, verification TXT). Changing web hosting should not affect email when mail DNS is preserved.
6. Verify the exact GitHub Pages settings and current DNS records prior to altering Porkbun DNS; allow time for propagation.

## Notes

- Project images were supplied by the site owner and optimized to WebP. Confirm usage/permission and whether any image shows confidential systems, people, badges, or customer identities before publishing.
- Site uses `mailto:` links rather than a web form. No visitor data collection or third-party analytics.
- All service descriptions are intentionally general; do not imply certifications, insurance, or formal client relationships without verification.
