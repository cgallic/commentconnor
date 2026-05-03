# commentconnor.com

Single-page landing page converting TikTok viewers into email subscribers and customers.

## Setup

### 1. Replace placeholders

In `index.html`, replace:
- `PLACEHOLDER_FORM_ID` — your Loops newsletter form ID (get from Loops dashboard → Forms)
- `https://buy.stripe.com/PLACEHOLDER_KIT` — your Stripe Payment Link for the $37 kit
- `https://calendly.com/connorgallic/ai-audit` — your Calendly booking URL

### 2. Deploy

**Vercel (recommended):**
```bash
npm i -g vercel
cd commentconnor
vercel --prod
```
Then add `commentconnor.com` as a custom domain in Vercel dashboard.

**Cloudflare Pages:**
1. Push to GitHub
2. Connect repo in Cloudflare Pages
3. Build command: (none needed)
4. Output directory: `/`
5. Add custom domain

**Manual:**
Upload `index.html` to any static host. It's a single file with zero dependencies.

### 3. Wire up Loops

1. Create a form in Loops dashboard
2. Copy the form ID
3. Replace `PLACEHOLDER_FORM_ID` in index.html
4. Create automation: on form submission → send email with PDF cheat sheet attached

### 4. Wire up Stripe

1. Create a Payment Link in Stripe dashboard for $37
2. Replace the `PLACEHOLDER_KIT` URL
3. Set up Stripe webhook → Loops event to deliver Notion template link on purchase

### 5. Wire up Calendly

1. Create event type "AI Audit — 30 min" at $147
2. Enable Stripe integration in Calendly for payment
3. Update the URL in index.html if different from placeholder

## Files

- `index.html` — the entire site (HTML + CSS + JS, ~12KB)

## Related links

- [MeetKai](https://meetkai.xyz) — the operator layer behind Kai CMO workflows.
- [KaiCalls](https://kaicalls.com) — AI voice agents for small-business phone answering and lead capture.
- [Connor Gallic](https://connorgallic.com) — founder building Kai, KaiCalls, and AI automation systems.
