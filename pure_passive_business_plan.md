# Pure Passive Business Plan — Michiana AI Digital Store
**Target: Revenue with zero cold outreach, zero sales calls, &lt;15 min/day after setup.**

---

## The Model (One Sentence)

Sell digital kits to entrepreneurs on **autopilot**: traffic finds you → email nurtures → Gumroad delivers → Grok creates everything new.

---

## Revenue Stack

```mermaid
flowchart LR
    Traffic[SEO + Social + Pinterest + Gumroad Discover] --> Store[Storefront]
    Store --> Capture[Free checklist email]
    Capture --> Nurture[5-day ConvertKit sequence]
    Nurture --> Sale[Gumroad checkout]
    Sale --> Deliver[Auto file download]
    Deliver --> Upsell[Bundle email Day 7]
```

| Product | Price | Margin | Delivery |
|---------|-------|--------|----------|
| 50 Chatbot Prompts | $47 | ~90% | Gumroad zip |
| Website + Chatbot Starter | $67 | ~90% | Gumroad zip |
| Complete Launch Kit | $97 | ~90% | Gumroad zip |
| Ultimate Bundle | $147 | ~90% | Gumroad zip |
| **Optional add-on** | | | |
| Notion Agency OS | $37 | ~95% | Gumroad |
| Monthly Prompt Drop (subscription) | $19/mo | ~85% | Gumroad membership |

**Month 3 target (realistic passive):** 15–40 sales/mo = **$700–$2,800/mo**  
**Month 1 target:** Infrastructure live + first 3–8 organic sales

---

## What Is Fully Automated (After Setup)

| Step | Tool | Human time |
|------|------|------------|
| Product pages | Gumroad | 0 ongoing |
| Payment + receipt | Gumroad | 0 |
| File delivery | Gumroad | 0 |
| Email capture | ConvertKit form on storefront | 0 |
| Nurture sequence | ConvertKit automation | 0 |
| Sale logging | Zapier → Google Sheet | 0 |
| Support FAQs | Storefront chatbot | ~2 min/day |
| New marketing content | Grok (weekly batch) | 15 min/week paste |

## What Is NOT in Pure Passive Mode

- ❌ Cold email to plumbers
- ❌ Discovery calls
- ❌ Fiverr (inbound = semi-passive; skip for now)
- ❌ Custom client work
- ❌ FB group daily engagement (optional 1 post/week max)

---

## Phase 1: Go Live (Days 1–3) — 4 Hours Total

### Day 1 — Payments + delivery (90 min)
**Grok command:** `Write my 4 Gumroad product listings in full — title, description, tags, cover copy, file list.`

1. Create Gumroad account
2. Create 4 products (see `gumroad_product_listings.md`)
3. Zip kit files per product (Grok can script this)
4. Enable automatic delivery on each product
5. Paste URLs into storefront `CONFIG.gumroadLinks`
6. Set `useSimulatedCheckout: false`

### Day 2 — Email autopilot (90 min)
1. ConvertKit free account
2. Create form: "AI Launch Checklist"
3. Paste 5 emails from `email_nurture_sequence.md`
4. Set delays: 0, 1, 2, 2, 2 days
5. Connect form action to storefront CONFIG
6. Create discount code `BUNDLE20` in Gumroad

### Day 3 — Storefront live (60 min)
**Grok command:** `Deploy ~/Downloads Michiana storefront to Vercel as index.html`

1. Rename storefront → `index.html`
2. Include all kit `.md` files + demo HTML in deploy folder
3. Deploy Vercel → custom domain optional
4. Test: form submit → sequence → test purchase ($0 test product)

---

## Phase 2: Traffic Without Outreach (Days 4–30)

Passive traffic only — no DMs, no cold email.

### Channel A: Gumroad Discover + SEO (free)
- Optimize product titles for search: "AI chatbot prompts local business," "AI agency starter kit 2026"
- Link Gumroad products from storefront (canonical)

### Channel B: Pinterest (high ROI for digital products)
**Grok command:** `/passive-pinterest 10`  
- 10 pins/week: product covers, checklist quotes, demo screenshots  
- Schedule in Pinterest native scheduler or Tailwind  
- Link to storefront email capture or Gumroad

### Channel C: One weekly post (optional, not daily)
- Reddit: r/sidehustle, r/Entrepreneur, r/artificial — **value post**, not spam  
- LinkedIn: 1 post/week from `weekly_content_calendar.md` (digital product angle only)  
- X/Twitter: thread summarizing checklist

**Grok command:** `/passive-content-week` — generates all 4 channels for the week

### Channel D: Affiliate content (slow burn, month 2+)
- 5 SEO articles on storefront blog or free Medium  
- Topics: "how to sell AI chatbots," "chatbot prompts for plumbers"  
- Affiliate links: Chatbase, Framer, Hostinger inside articles  
**Grok command:** `/passive-blog [topic]`

### Channel E: Product Hunt / free directories (one-time)
- Submit Complete Kit once  
- List on SellerShorts, itch.io (digital goods), free AI tool directories

---

## Phase 3: Expand Passive SKUs (Month 2)

Add products without new work — repackage existing kit:

| New product | Price | Source |
|-------------|-------|--------|
| Notion Agency OS | $37 | Grok converts kit to Notion structure |
| "Emails Only" pack | $27 | `email_nurture_sequence.md` + 10 bonus broadcasts |
| Niche prompt packs | $19 each | Split `chatbot_system_prompts.md` by vertical |
| Gumroad membership | $19/mo | 5 new prompts/month (Grok generates) |

**Grok command:** `/new-passive-product [idea]`

---

## Grok Passive Commands (Daily = 0, Weekly = 1 batch)

| When | Command | Output |
|------|---------|--------|
| Weekly Mon | `/passive-content-week` | Pinterest pins, 1 Reddit draft, 1 LinkedIn, 1 X thread |
| Monthly | `/passive-blog [topic]` | SEO article + meta description |
| Monthly | `/new-passive-product` | New Gumroad listing copy |
| On sale alert | `/passive-support [buyer question]` | Support reply template |
| Quarterly | `/passive-review [paste Gumroad stats]` | What to double down on |

**No daily commands required.**

---

## 30-Day Passive Calendar

| Week | Focus | Your time |
|------|-------|-----------|
| 1 | Gumroad + ConvertKit + Vercel live | 4 hrs |
| 2 | 10 Pinterest pins + 1 Reddit value post | 2 hrs |
| 3 | 2 SEO articles (Grok writes) | 1 hr paste/publish |
| 4 | Add 1 new SKU ($19 niche pack) + review stats | 2 hrs |

**Total month 1 hands-on:** ~9 hours, then **~1 hr/week**.

---

## Metrics to Watch (Google Sheet via Zapier)

| Metric | Target month 1 | Target month 3 |
|--------|----------------|----------------|
| Email subscribers | 50–150 | 300–800 |
| Gumroad sales | 3–8 | 15–40 |
| Conversion (email→sale) | 2–5% | 3–7% |
| Revenue | $141–$776 | $700–$2,800 |

---

## Risk & Mitigation

| Risk | Mitigation |
|------|------------|
| No traffic | Pinterest + SEO; patience 30–60 days |
| Gumroad fee (10%) | Acceptable at 90% margin digital |
| Piracy | Price low enough; update bundles quarterly |
| Support emails | Chatbot + FAQ; Grok templates |
| Burnout on content | One weekly Grok batch only |

---

## Files for Pure Passive Mode

| File | Role |
|------|------|
| `pure_passive_business_plan.md` | This doc |
| `gumroad_product_listings.md` | Copy-paste product pages |
| `passive_weekly_playbook.md` | 1-hour weekly routine |
| `email_nurture_sequence.md` | Autopilot emails |
| `lead_magnet_checklist.md` | Lead magnet |
| `AI_Business_Launch_Kit_Storefront.html` | Sales page |
| `grok_command_playbook.md` | Commands |

---

## Start Now (3 Actions)

1. Open `gumroad_product_listings.md` → create 4 products  
2. Paste `email_nurture_sequence.md` into ConvertKit  
3. Tell Grok: `Deploy my passive storefront from ~/Downloads to Vercel`

**Passive mode = no outreach. If you feel tempted to cold email, you're off-plan.**

---

*Michiana AI Digital Store — Pure passive lane | Grok-operated*