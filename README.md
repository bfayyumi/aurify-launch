# Aurify — product website

A static website for Aurify, operated by **Getaurify Inc.** HTML and CSS only; no build step, client JavaScript, external fonts, analytics, or forms.

## Content

- AI front office for home-service businesses, with Claude at the core.
- Clearly labeled product preview using fictional sample data, not a real screenshot.
- Connected lead response, qualification, follow-up, reactivation, booking, and CRM workflow.
- Claude architecture diagram, integration categories, and business-defined approvals.
- Demo requests go by email to hi@getaurify.com; no calendar booking is simulated.
- Dedicated privacy and website/service information pages.

The owner confirmed on October 7, 2026 that the Claude integration is working for a few while being built and updated. The copy says “Built on Claude” without claiming a customer count, named live integrations, results, or endorsement. The interface remains a concept, not product evidence.

## Files and preview

`index.html` is the homepage. `privacy.html` and `terms.html` contain public website policies. `style.css` holds shared responsive styling and reduced-motion rules. `social-card.png` is a 1200×630 social preview. `robots.txt`, `sitemap.xml`, and `CNAME` configure crawling and the domain.

Run `python3 -m http.server 5182 --bind 127.0.0.1` from this directory, then open http://127.0.0.1:5182.

## Hosting

GitHub Pages publishes the root of `main` at https://getaurify.com/. HTTPS is enforced. `.nojekyll` disables Jekyll processing. Pushes to `main` deploy the website.

The domain currently uses these GitHub Pages records. Preserve unrelated email and verification records if changing DNS:

| Type | Name | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | bfayyumi.github.io |

[GitHub Pages custom domain documentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).
