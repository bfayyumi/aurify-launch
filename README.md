# Aurify — coming-soon website

A simple, static one-page introduction to Aurify. Plain HTML and CSS, with no build step, JavaScript, external fonts, analytics, or forms. Contact: **hi@getaurify.com**.

The page covers the five planned services, intended Claude API use, human review, upcoming packages, development status, and contact details. Claude features are described as planned, and prices have not been announced. There are no invented client results or testimonials.

## Preview locally

From this directory, run `python3 -m http.server 5182 --bind 127.0.0.1`, then open http://127.0.0.1:5182.

## GitHub Pages

Publish the root of the `main` branch. No build is required; `.nojekyll` disables Jekyll processing. Changes pushed to `main` update the website.

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
