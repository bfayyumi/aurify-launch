# Aurify — one-page website

A simple, static one-page introduction to Aurify. Plain HTML and CSS, with no build step, JavaScript, external fonts, analytics, or forms. Contact: **hi@getaurify.com**.

The page introduces AI agents for local businesses, starting with home-service teams: inbound lead responses, qualification, follow-ups, customer reactivation, appointment booking, and CRM context. It explains the Claude-based design, owner review, contact details, and supporting local-growth services. It describes the intended architecture without claiming live deployments or inventing client results or testimonials. Subtle CSS entrance and hover motion respect reduced-motion preferences.

## Preview locally

From this directory, run `python3 -m http.server 5182 --bind 127.0.0.1`, then open http://127.0.0.1:5182.

## GitHub Pages

GitHub Pages publishes the root of the `main` branch at https://getaurify.com/. The custom domain is configured, its DNS points to GitHub Pages, and HTTPS is enforced. No build is required; `.nojekyll` disables Jekyll processing. Changes pushed to `main` update the website.

## Connect getaurify.com

In the domain provider's DNS settings, point the apex domain (`@`) to GitHub Pages using these four A records:

| Type | Name | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | bfayyumi.github.io |

Remove only conflicting website A/AAAA/CNAME records; preserve email MX, SPF, DKIM, DMARC, and other unrelated records. `www` points to the account host, without a repository path.

After the DNS resolves, set the custom domain to `getaurify.com` in repository **Settings → Pages** (a root `CNAME` file contains that hostname). Enable **Enforce HTTPS** once GitHub has issued the certificate. DNS and certificate issuance can take time.

Canonical metadata, the sitemap, and organization structured data already use https://getaurify.com/.

Official setup: [GitHub Pages custom domains](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).
