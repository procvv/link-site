# BSKO BUCKNER — Link Site

A lightweight, responsive creator page built with plain HTML, CSS, and JavaScript. It has no build step or dependencies.

## Preview locally

Open `index.html` in a browser.

## Update the page

Edit `index.html` to change the profile name, tagline, social links, card labels, and destinations. The Telegram-style button and the social links currently use placeholder destinations; replace them with the correct profile URLs before sharing the site. The footer email is also a placeholder.

The header's user count is a visual simulation. It changes by a small amount every few seconds and is not connected to real visitor analytics.

## Publish with GitHub Pages

The repository includes a GitHub Actions workflow that publishes the root folder to GitHub Pages whenever a commit is pushed to `main`.

1. Open the repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **GitHub Actions** as the source.
3. Push a change to `main`, or manually run **Deploy to GitHub Pages** from the **Actions** tab.

GitHub Pages is configured to use `bsko.shop`. Add these DNS records at your domain provider:

| Type | Host/name | Value |
| --- | --- | --- |
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| AAAA | `@` | `2606:50c0:8000::153` |
| AAAA | `@` | `2606:50c0:8001::153` |
| AAAA | `@` | `2606:50c0:8002::153` |
| AAAA | `@` | `2606:50c0:8003::153` |
| CNAME | `www` | `procvv.github.io` |

After DNS updates propagate, GitHub will check the domain and issue an HTTPS certificate. DNS changes can take up to 24 hours to propagate. The `www` record is recommended and redirects to the apex domain.
