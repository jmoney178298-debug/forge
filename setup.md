# Forge — Setup Guide

**Brand:** Forge  
**Tagline:** Find the lead. Build the site. Close the deal.

This is the polished, money-ready version of your agency OS. It runs entirely in the browser (localStorage). No server required to start making money.

---

## 1. Get it live in 10 minutes (recommended path)

### Option A — Netlify Drop (fastest)
1. Go to [https://app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the entire `forge` folder (or just the two HTML files) onto the page.
3. Netlify gives you a live URL like `https://random-name.netlify.app`
4. Optional: rename the site and add a custom domain later in Netlify settings.

### Option B — Cloudflare Pages
1. Create a free account at [https://pages.cloudflare.com](https://pages.cloudflare.com)
2. Create a project → Upload assets → select the `forge` folder.
3. Live in under a minute.

### Option C — Your own domain
Buy a domain (Namecheap, Cloudflare, Google Domains, etc.).  
Point the nameservers or use the Netlify/Cloudflare DNS instructions.  
Example good names: `getforge.app`, `useforge.co`, `forgeagency.com`, `tryforge.io`

---

## 2. First-time configuration (do this before you sell)

1. Open the live Forge app (`app.html`).
2. Go to **Settings**.
3. Fill in:
   - **Agency / brand name** → whatever you want clients to see (e.g. “Forge” or your personal brand).
   - **Stripe payment link** → create a Payment Link in Stripe Dashboard for your default price ($799 or whatever you choose).
   - **Square payment link** → same idea if you prefer Square (or leave blank).
   - **Default price** → $799 is a solid starting point for a 4-page local site.
   - **Monthly care plan** → $39–$79/mo is realistic for hosting + small edits.
   - Optional admin passcode if you want to lock the tool.
4. Click **Save settings**.

Your payment links now appear automatically in:
- Cold email sequences
- Client “your site is ready” emails
- The “After they say yes” ad copy

---

## 3. Daily workflow that makes money

1. **Leads tab** → pick a niche + city (roofers Tampa, plumbers Austin, etc.) → open Google Maps.
2. Look for businesses with no website or only a Facebook page. Score them (4+ = hot).
3. Send hot ones to **Pipeline**.
4. In Pipeline click **Build demo site** → it jumps to Studio with the business pre-filled.
5. Generate the site → download HTML or copy.
6. Send **Cold email sequence** (Email 1 today, Email 2 in 2 days, Email 3 in 5 days).
7. When they say yes → send the payment link → mark **Won**.
8. Go to **Publish** tab → follow the Netlify Drop instructions → give the client the live URL.

Repeat. Track everything in the Revenue tab.

---

## 4. Stripe vs Square

Both work. Just paste the payment link into Settings.

**Stripe**
- Dashboard → Payment Links → Create → set amount → copy link.
- Best if you already use Stripe.

**Square**
- Square Dashboard → Online → Payment Links (or Checkout Links) → create → copy.
- Good if you already take Square payments for other services.

You can fill both. The tool prefers Stripe if both are present, otherwise falls back to Square.

---

## 5. Publishing client sites (the 2-minute method)

1. In Studio, open the finished site → **Download HTML**.
2. Go to [https://app.netlify.com/drop](https://app.netlify.com/drop).
3. Drag the single `.html` file onto the page.
4. Netlify returns a live URL immediately.
5. (Optional) In Netlify → Domain settings → add the client’s domain or keep the free `*.netlify.app` subdomain.
6. Send the live link + your payment link.

You can charge extra for “custom domain setup” if you want.

---

## 6. What is still client-side only

- All data lives in the browser (localStorage key: `forge`).
- Clearing browser data or switching devices loses the data unless you export.
- For multi-device / multi-user later we can add the real backend (the Keystone Stripe + auth code you already have is the starting point).

For now this is intentional: zero hosting cost for the tool itself, instant start, and you can sell sites this weekend.

---

## 7. Next upgrades (when you’re ready)

When you want to go further:
- Real user accounts + cloud sync
- Team seats
- Automatic deploy from inside Forge (Netlify/Cloudflare API token)
- White-label client portal
- Higher-ticket app/website builder (Option B)

Just say the word and we build the next layer.

---

## Files in this package

| File        | Purpose                          |
|-------------|----------------------------------|
| `index.html`| Marketing / landing page         |
| `app.html`  | The full Forge agency OS         |
| `SETUP.md`  | This guide                       |

Open `index.html` first, then click through to the app.

You’re ready. Go close a deal.
