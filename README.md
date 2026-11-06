# xenlixgames.com

Official website of Xenlix Games. It is plain static HTML and CSS with no build step, no JavaScript, no cookies, no analytics and no external fonts.

| Page | Path | Used for |
|------|------|----------|
| Home | `/` | Studio home |
| Pulse Paths | `/pulse-paths/` | Store "marketing URL" |
| Support | `/support/` | Store "support URL" (FAQ + contact) |
| Privacy Policy | `/privacy/` | Store "privacy policy URL" (required by Google Play and Apple) |
| Terms & Conditions | `/terms/` | EULA / terms of use |
| Licences | `/licenses/` | Godot Engine MIT notice |
| 404 | `/404.html` | GitHub Pages "not found" page |

Contact email used on every page: `support@xenlixgames.com`. This mailbox must exist. To change it, search and replace the address across all `.html` files.

## Publish on GitHub Pages
1. Push this folder's contents to the root of `github.com/adhamqabban37/Xenlixgames.com` (branch `main`).
2. In the repo, go to Settings → Pages → Build and deployment: Source "Deploy from a branch", branch `main`, folder `/ (root)`.
3. Custom domain: once you own `xenlixgames.com`, add these DNS records:
   - `A` records for the apex domain: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153.
   - `CNAME` for `www` → `adhamqabban37.github.io`.

   Then enter `xenlixgames.com` under Settings → Pages → Custom domain and tick "Enforce HTTPS". GitHub writes the `CNAME` file for you. Don't add `CNAME` before the domain is live, or the github.io address will redirect to a domain that doesn't work.
4. The site works at `https://adhamqabban37.github.io/Xenlixgames.com/` before the domain is live. The 404 page uses root links, so it only looks right on the custom domain.

## Images
`assets/img/`:
- `pulse-paths-logo-source.jpg`: the original 1024 px logo.
- `pulse-paths-icon-*.png`: the logo with transparent rounded corners.
- `screen-*.webp`: real gameplay frames (Godot movie writer, 450×800).
- `og-pulse-paths.png`: 1200×630 social preview card.
