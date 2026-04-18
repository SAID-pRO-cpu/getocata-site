# getocata.com — Ocatagroup primary trust page

One-page static site. Plain HTML + Tailwind CDN. No build step.

## Deploy

```bash
vercel --prod
```

Or import via Vercel's GitHub integration: New Project → pick `getocata-site` repo → deploy. Framework preset: **Other** (static).

## Custom domain

1. In Vercel project settings → Domains, add `getocata.com` and `www.getocata.com`.
2. In Namecheap DNS for `getocata.com`, add the records Vercel gives you (usually: A record `@` → `76.76.21.21`, CNAME `www` → `cname.vercel-dns.com`).
3. Wait for DNS propagation (up to 24h, usually 10–60 min). Vercel auto-issues SSL.

## Edit

Everything lives in `index.html`. Sections are commented. To change copy:

- Hero: `<section>` under `<!-- Hero -->`
- About: `<!-- About -->`
- What it does: `<!-- What it does -->`
- Guarantee: `<!-- The Guarantee -->`
- Pricing: `<!-- Pricing -->`
- Fit: `<!-- Who this fits -->`
- FAQ: `<!-- FAQ -->`
- CTA: `<!-- Final CTA -->`

## Links to update before go-live

- Cal.com: `https://cal.com/said-belakbir/discovery` (confirm handle matches what you set up)
- Email: `said@getocata.com` (make sure mailbox is live first)
- LinkedIn: add URL in the About section where noted
