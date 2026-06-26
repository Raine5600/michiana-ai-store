# Michiana AI Solutions — Set & Forget Automation Playbook
**Go live in one afternoon. Run on autopilot after setup.**

**Related files (sales & marketing — mostly Grok-executable):**
- `automated_sales_marketing_plan.md` — master plan + daily routine
- `grok_command_playbook.md` — paste these commands into Grok daily
- `email_nurture_sequence.md` — ConvertKit emails (ready to paste)
- `weekly_content_calendar.md` — 4 weeks of social posts
- `outreach_execution_pack.md` — cold email system + tracking
- `lead_magnet_checklist.md` — free checklist for email gate

---

## Stack Overview

| Layer | Tool | Cost | What it automates |
|-------|------|------|-------------------|
| Storefront | `AI_Business_Launch_Kit_Storefront.html` (host on Vercel) | Free | Product display, email capture UI, sales chatbot |
| Payments | Gumroad (recommended) or Lemon Squeezy | 10% fee | Checkout, receipts, tax |
| Delivery | Gumroad auto-delivery OR Zapier + Google Drive | Free–$20/mo | Instant file delivery after purchase |
| Email capture | ConvertKit or MailerLite | Free tier | Lead magnets, nurture sequences |
| Upsells | Gumroad offer codes + checkout bump | Included | Bundle discounts, post-purchase offers |
| Service leads | Zapier → Google Sheets + email alert | Free tier | Fiverr/DM leads logged automatically |

---

## Step 1: Host the Storefront (15 min)

1. Create folder `michiana-ai-store` with these files:
   - `AI_Business_Launch_Kit_Storefront.html` → rename to `index.html`
   - `sample_plumber_website_demo.html`
   - `chatbot_system_prompts.md`
   - `Michiana_AI_Solutions_Business_Plan.md`
   - `fiverr_gig_and_outreach_kit.md`
2. Push to GitHub → connect Vercel → deploy.
3. In `index.html`, update `CONFIG` at the top of the script:
   - `gumroadLinks` — paste your Gumroad product URLs
   - `convertKitFormAction` — paste ConvertKit form endpoint
   - `deliveryFolderUrl` — Google Drive shared folder link for buyers

---

## Step 2: Gumroad Products (30 min)

Create 4 Gumroad products matching the storefront:

| Product | Price | Files to attach |
|---------|-------|-----------------|
| Complete Launch Kit 2026 | $97 | All 5 kit files (zip) |
| 50 Chatbot Prompts Pack | $47 | `chatbot_system_prompts.md` |
| Website + Chatbot Starter | $67 | `sample_plumber_website_demo.html` + prompts |
| Ultimate Bundle (all 3) | $147 | Full zip + bonus automation playbook |

**Per product settings:**
- Enable "I want to offer this as a pay-what-you-want" → OFF
- Content tab → upload files OR link to Google Drive
- After purchase → Gumroad sends download email automatically
- Create offer code `BUNDLE20` for email subscribers (20% off bundle)

Copy each product URL into the storefront `CONFIG.gumroadLinks` object.

---

## Step 3: Email Capture + Nurture (45 min)

### ConvertKit setup

1. Create form: "Free AI Launch Checklist" (lead magnet = link to demo HTML).
2. Create 5-email sequence (schedule: Day 0, 1, 3, 5, 7):

**Email 1 (instant):** Deliver free checklist + link to plumber demo. CTA: Browse kits at your storefront URL.

**Email 2:** "3 local businesses making $2k/mo with AI chatbots" — social proof story. CTA: Chatbot Prompts Pack ($47).

**Email 3:** Case study format — walk through the demo site. CTA: Website Starter Pack ($67).

**Email 4:** Objection handling — "I don't know how to sell this." Include Fiverr gig text snippet. CTA: Complete Kit ($97).

**Email 5:** Urgency — bundle offer $147 (save $64). Include `BUNDLE20` code for subscribers.

3. Paste ConvertKit form action URL into storefront `CONFIG.convertKitFormAction`.

### MailerLite alternative
Same flow — use automation workflow triggered on form submit.

---

## Step 4: Zapier Automations (30 min)

### Zap A: New Gumroad sale → delivery log
- Trigger: Gumroad — New Sale
- Action: Google Sheets — Add Row (date, email, product, amount)
- Action: Gmail — Send personal thank-you (optional, Gumroad already sends receipt)

### Zap B: ConvertKit subscriber → welcome tag
- Trigger: ConvertKit — New Subscriber
- Action: ConvertKit — Add Tag "launch-kit-lead"
- Action: Slack/Email — Notify you of new lead

### Zap C: Fiverr order (manual) → client folder
- Trigger: Email — New email matching "Fiverr order"
- Action: Google Drive — Create folder `[Client Name] - [Date]`
- Action: Google Sheets — Log service client

### Make.com alternative
Same logic — Gumroad webhook → router → multiple actions.

---

## Step 5: One-Click Upsell Paths

Built into the storefront checkout flow:

1. **Cart bump:** After selecting any single product, modal offers bundle upgrade ($147 vs $211 separate).
2. **Post-purchase:** Success screen shows "Add Chatbot Prompts for $27" (create Gumroad upsell link).
3. **Email Day 3:** Link directly to bundle with pre-filled discount code.
4. **Chatbot:** When user asks about pricing, bot recommends bundle and offers to email the link.

Gumroad upsell: Settings → Upsells → link lower-tier buyers to bundle at discounted price.

---

## Step 6: AI Support Chatbot (Production)

Replace demo chat logic with Chatbase or Grok API:

1. Copy system prompt from `chatbot_system_prompts.md` — adapt for **Michiana AI Solutions sales** (products, pricing, automation, Fiverr services).
2. Deploy on Chatbase.co → embed script in storefront (replace built-in widget).
3. Connect Chatbase → Zapier → email you when someone asks about custom services ($499+ packages).

**Sales bot must know:**
- 3 digital products + bundle pricing
- Fiverr service packages ($499–$999)
- Link to live demo
- Email capture offer (free checklist)

---

## Step 7: Set & Forget Checklist

- [ ] Storefront live on custom domain (optional: `michianaai.com`)
- [ ] 4 Gumroad products with auto-delivery files attached
- [ ] ConvertKit form connected + 5-email sequence active
- [ ] Zap A + B running (test with $0 Gumroad product)
- [ ] Fiverr gig posted (copy from `fiverr_gig_and_outreach_kit.md`)
- [ ] Chatbase bot live (or Grok API connected)
- [ ] Google Sheet tracking sales + leads
- [ ] Weekly 15-min review: check sheet, refine chatbot from logs

**Expected hands-on time after setup:** ~30 min/week (review sales, respond to service inquiries only).

---

## Revenue Paths (Automated vs Manual)

| Path | Automation level | Your involvement |
|------|------------------|------------------|
| Digital product sales | 95% automated | None unless support email |
| Email nurture → purchase | 90% automated | Write/refine emails once |
| Fiverr service orders | 50% automated | Deliver using kit templates |
| Local cold outreach | 20% automated | Send emails, take calls |

---

*Michiana AI Solutions | Built with Grok | June 2026*