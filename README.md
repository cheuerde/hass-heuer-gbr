# Haß-Heuer GbR Website Test

Static first version for `hass-heuer-gbr.de`.

Live preview:

https://cheuerde.github.io/hass-heuer-gbr/

## Preview

Open `index.html` in a browser, or serve this folder with any static web server.

## Custom domain DNS

When moving `hass-heuer-gbr.de` from Squarespace to GitHub Pages, keep the
Google Workspace mail records and change only the website records:

- `@` A `185.199.108.153`
- `@` A `185.199.109.153`
- `@` A `185.199.110.153`
- `@` A `185.199.111.153`
- `www` CNAME `cheuerde.github.io`

Keep:

- MX `1 smtp.google.com`
- TXT `v=spf1 include:_spf.google.com ~all`

## Before publishing

- Replace `claas@hass-heuer-gbr.de` if the public contact mailbox changes.
- Confirm the Impressum and privacy text before making the site final.
- Remove or adjust the `noindex, nofollow` robots meta tag when the site should be indexed.
