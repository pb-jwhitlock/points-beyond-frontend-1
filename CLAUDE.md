# Points Beyond AI — Landing Page Context

## Project Overview
Single-file HTML landing page for Points Beyond AI. No framework — pure HTML/CSS/JS inline.
Deployed via GitHub Pages at **pointsbeyond.ai** with Cloudflare DNS and HTTPS enforced.

---

## Current Status

| Item | Status |
|------|--------|
| Landing page (index.html) | ✅ Live at pointsbeyond.ai |
| Favicons | ✅ All sizes deployed (ico, 16, 32, apple-touch, 192, 512) |
| site.webmanifest | ✅ Configured with brand name and purple theme color |
| GitHub Pages | ✅ Built, CNAME verified, SSL approved |
| Cloudflare DNS | ✅ Connected |
| GHL webhook integration | ⏳ Placeholder only — endpoint not yet configured |
| Form SMS/A2P compliance | ✅ Consent checkbox, STOP/HELP instructions, disclosure |

---

## Last Session Summary

- Built and deployed v2 landing page from scratch — 2 services only (AI Voice Agents, AEO/SEO), 7-day delivery, no Georgetown MPP or $17M+ references
- Wired up all favicon files (from favicon_io folder) including site.webmanifest; logo image now used in nav and footer instead of SVG placeholder
- Iterative copy and design refinements: $399/mo pricing, free 7-day trial on voice agents, updated Privacy Policy/Terms dates to Jan 1 2026, contact email accounts@pointsbeyond.ai, LinkedIn button in blue founder card, session note line repositioned near footer

---

## Next Steps

1. **Configure GHL webhook** — replace the placeholder comment in the form JS submit handler with the actual GoHighLevel webhook endpoint
2. **Test form submission end-to-end** — verify lead data flows into GHL CRM correctly
3. **Add OG image** — `<meta property="og:image">` is missing; create and add a social share image

---

## Design Decisions

- **Font:** Urbanist (Google Fonts) — 400/500/600/700/800/900
- **Brand purple:** `#2e1f7a` (primary), `#4335b8` (light)
- **Accent orange:** `#ea580c`
- **Services:** AI Voice Agents + AEO/SEO only (Custom AI Apps and Workflow Automation excluded by design)
- **Pricing:** $399/mo, free 7-day trial, no setup fee language
- **Credentials shown:** 10+ years enterprise IT strategy, Fairfax County VA — TS/SCI removed by request
- **Stats removed:** Georgetown MPP and $17M+ value — removed by request
- **AI DISPATCH badge:** Removed from nav by request
- **Hero badge:** "AI Agency — Northern VA" with green dot, original purple-on-surface style

---

## Key File Locations

- Landing page: `~/points-beyond-frontend-1/index.html`
- Astro site (separate): `~/points-beyond`
- Favicons source: `~/Library/CloudStorage/Proton Drive/Images/Points-Beyond Logo Files/favicon_io/`
- Custom Claude commands: `~/.claude/commands/`

---

## GHL Integration Notes

Form currently has a placeholder comment block where the webhook URL goes:
```js
// GHL WEBHOOK INTEGRATION
// Replace this comment with:
// fetch('YOUR_GHL_WEBHOOK_URL', { method: 'POST', ... })
```
Search for `GHL WEBHOOK` in index.html to find both the HTML form action placeholder and the JS submit handler.
