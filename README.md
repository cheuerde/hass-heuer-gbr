# Haß-Heuer GbR Website Test

Static first version for `hass-heuer-gbr.de`.

Live preview while DNS is pending:

https://cheuerde.github.io/hass-heuer-gbr/

Current production target:

- VM: `95.179.248.249`
- Web server: Caddy Docker stack at `/home/cheuer/family-hub`
- Deployed path on VM: `/home/cheuer/family-hub/hass-heuer`

## Preview

Open `index.html` in a browser, or serve this folder with any static web server.

## Custom domain DNS

When moving `www.hass-heuer-gbr.de` from Squarespace to the VM, keep the Google
Workspace mail records and change only the `www` website record:

- Delete or replace `www` CNAME `ext-sq.squarespace.com`
- Add `www` A `95.179.248.249`

Keep:

- MX `1 smtp.google.com`
- TXT `v=spf1 include:_spf.google.com ~all`

## Before publishing

- Replace `claas@hass-heuer-gbr.de` if the public contact mailbox changes.
- Confirm the Impressum and privacy text before making the site final.
- Remove or adjust the `noindex, nofollow` robots meta tag when the site should be indexed.
