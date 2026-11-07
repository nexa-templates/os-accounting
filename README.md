# Accounting

Visual starter; functional accounting/payment workflows remain planned.

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/nexa-templates/os-accounting)

## Run and deploy

Install dependencies using the included lockfile, run `npm run build`, then `npm run deploy`. Wrangler provisions the declared resources. No Nexa account or API key is required for the default configuration.

## Access

Protect the application hostname with Cloudflare Access. Configure `ACCESS_ISSUER`, `ACCESS_AUD` and `APP_ORIGIN`. The Worker also verifies signed tokens and rejects alternate hostnames.

`PREVIEW_MODE=true` is only for an isolated public sample deployment with no customer data or live services. Real installations use `false`.
## Source

Adapted from [accounting](https://github.com/nexa-templates/accounting/tree/9c8d9724c347069ec725a42cde18856e5cc32853) at `9c8d9724c347069ec725a42cde18856e5cc32853`. Original license files are retained. These source files are ordinary Wrangler applications; no Nexa manifest is required.
