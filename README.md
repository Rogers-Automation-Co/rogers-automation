# Rogers Automation Co. website

Static site for https://rogersautomation.co, served by GitHub Pages from the `main` branch root. Plain HTML and CSS. No build step.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | All page content |
| `styles.css` | All styling and colors (see `:root` at the top) |
| `fonts/` | Self-hosted Saira (variable font, latin subset, woff2) |
| `rogers-logo.svg`, `rogers-logo-white.svg` | Logo for light and dark backgrounds |
| `rogers-gear-icon.svg`, `favicon-*.png`, `apple-touch-icon.png` | Favicons |
| `og-image.png` | 1200x630 social share image |
| `CNAME` | Custom domain for GitHub Pages. Do not delete. |
| `robots.txt`, `sitemap.xml` | Search engine files |

## Editing text

Open `index.html` in any editor. Each section is marked by its `id` (`services`, `about`, `contact`). Change the text between the tags and save. Do not use em dashes in copy.

To set the contact email, search for `EMAIL_PLACEHOLDER` and `[ADD: business email]` and replace both with the real address.

## Previewing

Double-click `index.html` to open it in a browser.

## Redeploying

```
git add -A
git commit -m "Update site text"
git push
```

GitHub Pages rebuilds in about a minute.

## Custom domain

DNS records at the registrar for `rogersautomation.co`:

- Four `A` records on the apex (`@`) pointing to GitHub Pages. Check the current values at https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
- One `CNAME` record for `www` pointing to `<github-username>.github.io`

After DNS resolves, turn on Enforce HTTPS in the repo's Pages settings. Also verify the domain in your GitHub account settings under Pages.
