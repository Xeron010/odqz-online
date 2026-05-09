# ODQZ Studio Website

Independent brand & digital studio. Single-file static deployment for Cloudflare Pages.

## What's on the page (PayFast compliance checklist)

- ✅ **Local contact number:** 0333 151 6444 (in contact section + footer)
- ✅ **Local Pakistani address:** Near Multan Kitab Ghar, Kalma Chowk, Taunsa Sharif, Punjab
- ✅ **9 distinct services** in Section 02 — each presented as its own card with name, description, what's included, and price in PKR
- ✅ **Full pricing catalogue** in Section 03 — 16 priced line items across Brand, Web, Retainers, and One-off services
- ✅ **Privacy Policy** — Section 08
- ✅ **Terms & Conditions** — Section 09
- ✅ **Refund & Cancellation Policy** — Section 10
- ✅ **Service Delivery Policy** — Section 11
- ✅ **PayFast referenced** as authorised payment partner in Privacy, Terms, and Refund policies
- ✅ **JazzCash, Easypaisa, RAAST** all mentioned as accepted payment methods
- ✅ Footer links to all four policy pages and the pricing section

## The 9 featured services (Section 02)

| # | Service | Price |
|---|---------|-------|
| 01 | Logo & Wordmark Design | PKR 35,000 |
| 02 | Brand Identity System | PKR 150,000 |
| 03 | Complete Brand Identity | PKR 350,000 |
| 04 | Landing Page Design | PKR 85,000 |
| 05 | Marketing Website Build | PKR 250,000 |
| 06 | E-commerce Store Build | PKR 450,000 |
| 07 | SEO Retainer | PKR 95,000 / mo |
| 08 | Content & Social Retainer | PKR 75,000 / mo |
| 09 | Brand Audit & Consultation | PKR 35,000 |

That's a clear 9 services on the homepage — well above PayFast's "7 or more services" requirement. The Pricing section below adds 7 more (Brand strategy bundle, Custom web app, Full-service marketing retainer, Premium retainer, Strategy consulting hourly, Logo refresh, Website maintenance) for a total of 16 distinct priced offerings on the site.

## Deploy to Cloudflare Pages

1. Replace the existing `index.html` and `README.md` in your GitHub repo with these new versions.
2. Commit and push. Cloudflare Pages will auto-rebuild within ~30 seconds and deploy the new version.
3. Hard-refresh the live site (Ctrl+Shift+R / Cmd+Shift+R) once the deployment finishes.

## Reply to send back to the PayFast admin

Once the new version is live at odqz.online, reply with something close to this:

> Thank you for the feedback. The website has been updated as requested. The Services section (visible on the homepage) now lists 9 distinct services, each with a clear name, description, what's included, and a starting price in Pakistani Rupees. A full pricing catalogue with additional offerings is also published in the Pricing section directly below it.
>
> Please review at https://odqz.online — the services are immediately visible after scrolling past the hero. Let me know if anything else is needed.

## Hooking up the contact form (when needed)

The form currently shows a success message via JavaScript without sending anywhere.
When you're ready to actually receive submissions, swap the `fetch()` line in the script
at the bottom of `index.html`. Three easy options:

- **Formspree** — free tier, drop-in, no backend
- **Cloudflare Pages Functions** — `/functions/api/contact.js` posting to email
- **Web3Forms** — also free, same pattern

Look for the comment `// Note: in production, replace with actual fetch()` in the script.

## Notes

- All assets are inline (fonts via Google Fonts CDN). No build step.
- Works on the Cloudflare free plan.
- Single file — easy for any reviewer to inspect end-to-end.
