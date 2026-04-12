# commentconnor.com — Remaining Setup

The landing page is **live** at commentconnor.com. These items need manual setup to complete the funnel.

## Priority 1: Wire the email form (15 min)

The email forms on the page currently point to a placeholder Loops endpoint. Without this, signups go nowhere.

1. Go to [app.loops.so](https://app.loops.so) → Forms
2. Create a new form (or use an existing one) for "AI Cheat Sheet" signups
3. Copy the form ID from the embed code
4. In `index.html`, find `PLACEHOLDER_FORM_ID` (appears once in the script section) and replace it with your actual form ID
5. Commit and push — Vercel auto-deploys

**Email automation**: Set up a Loops automation that sends the cheat sheet PDF when someone subscribes. The cheat sheet content is in `cheat-sheet-content.md` — convert it to PDF (Google Docs, Notion export, or Canva).

## Priority 2: Update Gumroad pricing (5 min)

The "Get the kit" button links to your existing Gumroad product (The Approval Engine). The landing page shows $37 but Gumroad currently lists it at $17.

1. Go to [connorgallic.gumroad.com/l/gnyod](https://connorgallic.gumroad.com/l/gnyod) → Edit
2. Update price from $17 to $37
3. Optionally rename to "The Corporate Survival Kit" to match the landing page

**Alternative**: Create a Stripe payment link at $37 and replace the Gumroad URL in `index.html`. Search for `gumroad.com/l/gnyod` and swap it. Stripe has no platform fee (just processing), vs. Gumroad's 10%.

## Priority 3: Set up Calendly event (10 min)

The "Book a slot" button links to `calendly.com/connorgallic/ai-audit`. This event type may not exist yet.

1. Go to [calendly.com](https://calendly.com) and create event type:
   - Name: "30-Min AI Audit"
   - Duration: 30 minutes
   - URL slug: `ai-audit`
   - Max per week: 5
   - Price: $147 (Calendly can collect payment via Stripe integration)
2. If you use a different slug, update the URL in `index.html`

## Priority 4: Analytics (5 min)

Analytics placeholders are in the HTML head as commented-out script blocks.

1. **GA4**: Uncomment the GA script block and replace `GA_MEASUREMENT_ID` with your GA4 property ID
2. **TikTok Pixel**: Uncomment the TikTok pixel block and replace `YOUR_TIKTOK_PIXEL_ID`
3. Both are already on connorgallic.com — copy the IDs from there

## Priority 5: Create the cheat sheet PDF (30 min)

The content is written in `cheat-sheet-content.md`. Convert to PDF:

1. Paste into Google Docs or Notion
2. Add your branding (logo, colors)
3. Export as PDF
4. Upload to Loops as the automated delivery attachment
5. Or host on Google Drive / Dropbox and include the link in the welcome email

## Priority 6: Email nurture sequence (optional, day 2)

After the cheat sheet signup, set up 3 emails in Loops:

| Day | Subject | Content |
|-----|---------|---------|
| 0 | Here's your AI Cheat Sheet | Deliver PDF + "start with workflow #1" |
| 2 | This one saved someone $4,200 | Insurance denial success story + soft pitch for $37 kit |
| 5 | 4 hours on a performance review? | Kit pitch: "The kit does it in 15 minutes" → $37 CTA |

## Priority 7: OG image for social sharing

When the link is shared on social, it currently has no preview image. Create a 1200x630px image:
- Dark background matching site
- "Comment Connor. Get the hack." in the page fonts
- Upload as `og.png` to the repo root
- Uncomment the og:image meta tag in `index.html` and set to `https://commentconnor.com/og.png`

## Priority 8: Update TikTok bio link

Change TikTok bio link from connorgallic.com/links → commentconnor.com

## What's Live Now

- commentconnor.com — full landing page with 3 product tiers
- Free cheat sheet section with email form (needs Loops form ID)
- $37 Corporate Survival Kit → Gumroad link (needs price update)
- $147 AI Audit Call → Calendly link (needs event creation)
- Mobile sticky CTA bar
- FAQ section
- Testimonials
- Weak vs Operator comparison section
- Second email capture at page bottom
