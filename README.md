# Nasman Finance Hub — Deployment Package

## Recommended hosting
GitHub Pages is the simplest free option for this static HTML/CSS/JavaScript site. GitHub Pages supports HTTPS and custom domains.

Official docs:
https://docs.github.com/en/pages/getting-started-with-github-pages

## Deploy
1. Create a GitHub account.
2. Create a public repository named `nasman-finance-hub`.
3. Upload all files in this folder, with `index.html` at the repository root.
4. Open **Settings → Pages**.
5. Choose the `main` branch and `/ (root)` as the publishing source.
6. Save and open the generated `https://USERNAME.github.io/nasman-finance-hub/` URL.
7. Add your custom domain under Pages settings.
8. After certificate provisioning, enable **Enforce HTTPS**.

## Custom domain
Use `YOURDOMAIN.com` as the placeholder until you own the real domain.

For GitHub Pages apex-domain DNS, GitHub currently documents these A records:
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153

For `www`, use a CNAME to `USERNAME.github.io`.

Verify the domain in GitHub to reduce takeover risk. Do not use wildcard DNS records.

## Security
The site contains no API keys or private secrets. HTTPS/SSL is provided by the hosting platform; HTML alone cannot create a TLS certificate.

## Final checks
HTTPS, no mixed content, CSS/JS/images load, checklist persistence works, monthly reviews work, mobile layout works, internal/external links work, HTTP→HTTPS works after host configuration, www/non-www behavior is consistent, and no secrets are exposed.
