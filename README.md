# ODQZ Studio Website

Independent brand & digital studio. Single-file static deployment for Cloudflare Pages.

## What's on the page (PayFast compliance checklist)

- ✅ **Local contact number:** 0333 151 6444 (in contact section + footer)
- ✅ **Local Pakistani address:** Near Multan Kitab Ghar, Kalma Chowk, Taunsa Sharif, Punjab
- ✅ **Complete services with PKR pricing** — Section 03, 16 line items across Brand, Web, Retainers, and One-off
- ✅ **Privacy Policy** — Section 08
- ✅ **Terms & Conditions** — Section 09
- ✅ **Refund & Cancellation Policy** — Section 10
- ✅ **Service Delivery Policy** — Section 11 (covers digital delivery + physical shipping)
- ✅ **PayFast referenced** as authorised payment partner in Privacy, Terms, and Refund policies
- ✅ **JazzCash, Easypaisa, RAAST** all mentioned as payment methods
- ✅ Footer links to all four policy pages and the pricing section

## Deploy to Cloudflare Pages

1. Create a new GitHub repo (public or private both work).
2. Upload `index.html` (and this `README.md`) to the repo root.
3. In Cloudflare dashboard → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**.
4. Pick the repo. Build settings:
   - **Framework preset:** None
   - **Build command:** *(leave empty)*
   - **Build output directory:** `/` (root)
5. Deploy. Then go to **Custom domains** and add `odqz.online`.

## Reply to send back to the PayFast admin

Once the site is live at odqz.online, reply with something close to this:

> Thank you for the review and detailed feedback. I have:
>
> 1. Reviewed the MDR rates and the PKR 20,000 one-time setup fee outlined in your Partner Guide, and confirm my approval to proceed.
> 2. Updated the website with all required policies — Privacy Policy, Terms & Conditions, Refund & Cancellation Policy, and Service Delivery Policy — each accessible from the footer.
> 3. Published the complete service catalogue with pricing in PKR.
> 4. Added the local contact number (0333 151 6444) and local studio address (Near Multan Kitab Ghar, Kalma Chowk, Taunsa Sharif, Punjab).
>
> The site is live at https://odqz.online. Please review and let me know the next steps for the onboarding documentation.

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
