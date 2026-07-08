# 🔥 Wildfire — Free Lead Gen Calculators

A suite of free, no-signup, browser-only calculators for lead generation marketers. Pure static HTML/CSS/JS — no build step, no backend, no dependencies, zero hosting cost.

## The tools

| Tool | Target keyword | File |
|---|---|---|
| Cost Per Lead Calculator | "cost per lead calculator" | `tools/cpl-calculator.html` |
| Lead Value Calculator | "lead value calculator", "how much to pay per lead" | `tools/lead-value-calculator.html` |
| Campaign ROI Calculator | "lead generation roi calculator" | `tools/roi-calculator.html` |
| A/B Test Significance Calculator | "ab test significance calculator" | `tools/ab-test-calculator.html` |
| UTM Link Builder | "utm builder", "utm link generator" | `tools/utm-builder.html` |
| Email Subject Line Tester | "email subject line tester" | `tools/subject-line-tester.html` |

## Deploy (free, ~5 minutes)

1. Push this repo to GitHub.
2. Repo → **Settings → Pages** → Source: *Deploy from a branch* → `main` / root. Done — live at `https://<user>.github.io/wildfire/`.
3. **Recommended:** buy a domain (~$10/yr, the only cost). The site currently uses `wildfiretools.io` as a placeholder — check availability, or pick anything (`.io`, `.tools`, `.marketing`). Then find-and-replace `https://wildfiretools.io` across all `.html` files, `sitemap.xml`, and `robots.txt` with your real domain, and set the custom domain in GitHub Pages settings.
4. Add the site to [Google Search Console](https://search.google.com/search-console), submit `sitemap.xml`.

Cloudflare Pages or Netlify free tiers work identically if you prefer them.

## Monetization (in order of effort)

### 1. Affiliate links (already stubbed in)
Every tool page has a "Tools we recommend" box with `href="#"` placeholders marked `TODO`. Apply to these programs (all free to join) and drop in your links:

| Program | Payout | Fit |
|---|---|---|
| HubSpot Affiliates | 30% recurring up to 1 yr | CPL / ROI / lead value pages |
| Unbounce Partners | 20–35% recurring | CPL / A/B test pages |
| ActiveCampaign | 20–30% recurring | Subject line page |
| ConvertKit (Kit) | 30% recurring, 24 mo | Subject line page |
| OptinMonster | 20% | CPL page |
| Supermetrics | 20% recurring | ROI / UTM pages |
| Semrush (BeRush) | $200/sale | Any page |

Keep the `rel="sponsored nofollow"` attributes and the affiliate disclosure lines — they're required by FTC rules and Google guidelines.

### 2. Email list (form is stubbed in)
Every page has a subscribe form with a `TODO` action. [Buttondown](https://buttondown.email) (free to 100 subs) or Kit (free to 10k subs) — paste the form action URL in. A weekly "one lead gen tactic" email is the retention layer: it turns one-time calculator visitors into a recurring audience you can monetize with the same affiliate links or, later, sponsorships (~$20–50 CPM once you're past ~1k subscribers).

### 3. Later, once there's traffic
- **Embeddable widgets**: let agencies embed the calculators on their own sites with a "Powered by Wildfire" backlink (free tier) or white-label (paid, ~$19/mo). Calculators are lead magnets — your day-job industry buys these.
- **Sponsored placement**: sell the rec-box slots directly to marketing SaaS companies instead of affiliate networks.
- **Programmatic SEO**: spin the CPL benchmark table into per-industry pages ("average cost per lead for SaaS") — each is a long-tail keyword.

## Launch checklist (free distribution)

- [ ] Submit to Product Hunt (tools like this regularly do well as "free tool" launches)
- [ ] Post the CPL calculator to r/PPC, r/marketing, r/Emailmarketing (share as a resource, not an ad)
- [ ] Submit to free-tool directories: SaaSHub, AlternativeTo, Free-for.dev, Indie Hackers
- [ ] Answer "what's a good CPL" questions on Reddit/Quora and link the calculator
- [ ] LinkedIn post walking through the lead value calculator (lead gen audience lives there)
- [ ] Ask marketing newsletters to include it (free tools get picked up easily)

## Development

No build step. Open any `.html` file in a browser, or `python -m http.server` from the repo root. Shared styles live in `styles.css`; each tool page is fully self-contained otherwise.

## TODO markers

Search the codebase for `TODO` to find every spot that needs a real value:
- Affiliate links in each page's `rec-box`
- Email form `action` URLs
- Domain replacement (if not using wildfiretools.io)
