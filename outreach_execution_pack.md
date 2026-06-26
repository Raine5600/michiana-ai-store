# Outreach Execution Pack — Copy, Send, Track
**Grok writes personalized versions. This file is your daily operating system.**

---

## Daily Quota (Non-Negotiable)

| Activity | Min/day | Grok command |
|----------|---------|--------------|
| New cold emails | 5 | `/batch-outreach [trade] 5` |
| Follow-ups | 3 | `/follow-up [day]` |
| FB group post | 1 | Copy from `weekly_content_calendar.md` |
| Fiverr inbox check | 1 | `/fiverr-response [msg]` if needed |

**Time:** 20 minutes if Grok pre-wrote everything the night before.

---

## Lead Tracking Sheet (Copy to Google Sheets)

| Date | Business | Trade | City | Website | Status | Next Action | Grok Command |
|------|----------|-------|------|---------|--------|-------------|--------------|
| | | | | | Sent | Follow up Day 3 | `/follow-up 2` |
| | | | | | Replied | `/prep-call` | |
| | | | | | Demo done | `/proposal` | |
| | | | | | Closed | `/deliver-site` | |
| | | | | | Dead | — | |

**Status values:** `Research` → `Sent` → `Follow-1` → `Follow-2` → `Replied` → `Demo` → `Proposal` → `Closed` → `Dead`

---

## Follow-Up Schedule (Automated via Grok)

| Days since send | Action | Grok |
|-----------------|--------|------|
| 0 | Initial email | `/write-outreach` |
| 3 | Friendly bump | `/follow-up 2` |
| 7 | Value-add (share demo link again) | `/follow-up 2` |
| 14 | Breakup email | `/follow-up 2` |

---

## Master Cold Email Template (Grok personalizes)

**Subject options (rotate):**
- Quick question about [Business Name]'s website
- 24/7 booking for [trade] in [city]?
- Noticed [Business Name] on Google — idea for you
- [First name], missing after-hours calls?

**Body:**
```
Hi [Name / Team at Business],

I came across [Business Name] while looking at [trade] businesses in [city].

[SPECIFIC OBSERVATION — Grok fills: "Your site isn't mobile-friendly" / "Looks like you don't have online booking" / "No website listed on Google"]

I build modern websites + AI assistants for Michiana trades that answer questions and book jobs 24/7 — even when you're on site.

Here's a 60-second live demo (tap the chat button): [DEMO]

Open to a 10-minute look this week? No pressure — happy to just send the link.

Cameron
Michiana AI Solutions
574.274.0643
[STORE]
```

---

## FB DM Template (Short)

```
Hey [Name] — saw [Business] in [group / Google]. I help local [trade] businesses add AI booking to their site (works 24/7). Built a quick demo: [DEMO]. Worth a look if after-hours leads are a thing for you. — Cameron
```

---

## Demo Call Script (10 min)

**Min 0–2:** "Thanks for hopping on. I'll keep this to 10 minutes. Can I share my screen?"

**Min 2–5:** Open demo → show hero → click chat → type leaking sink scenario → show booking flow.

**Min 5–7:** "This is a template — yours would have your logo, services, pricing, and phone. Live in 48 hours."

**Min 7–9:** "Pro package is $799 — full site + chatbot. Pilot this month at $599 if you can give feedback. Which fits better?"

**Min 9–10:** "I'll send a one-pager today. When's good to decide — this week or next?"

**Grok prep:** `/prep-call [Business] [trade]`

---

## Close Email (Send Within 1 Hour of Demo)

**Grok:** `/post-call said yes` or `/proposal [name] Pro`

**Template:**
```
Hi [Name],

Great talking today. As discussed:

→ [Package] — $[price]
→ Delivered within 48 hours
→ Includes: [bullet list]
→ 50% deposit to start: [PayPal/Venmo/Fiverr link]

Reply "GO" and I'll send the intake form (5 questions — Grok can generate).

Cameron
```

---

## Intake Form (Send After "GO")

**Grok command:**
```
/intake-form [Business] [trade]
Create 8 client intake questions for website + chatbot build: business details, services, pricing ranges, service area, hours, brand colors, competitors, special offers.
```

---

## Niche Rotation Schedule

| Week | Trade | Search query for Grok |
|------|-------|----------------------|
| 1 | Plumbers | `plumber South Bend IN` |
| 2 | HVAC | `HVAC Mishawaka IN` |
| 3 | Dentists | `dentist Granger IN` |
| 4 | Electricians | `electrician Niles MI` |
| 5 | Roofers | `roofing Elkhart IN` |

---

## First 10 Outreach — Starter Batch (Customize with Grok)

Run this command to replace placeholders with real businesses:
```
/batch-outreach plumbers 10
Use real Michiana plumber business names from web search. Personalize each email.
```

**Fallback generic (if no search):**

1. **Subject:** South Bend plumber — quick website idea  
   **Angle:** No online booking visible

2. **Subject:** After-hours calls for [Name] Plumbing?  
   **Angle:** Strong Google reviews but dated site

3. **Subject:** Granger area — 48hr AI booking setup  
   **Angle:** Competitor has chat, they don't

4. **Subject:** Mishawaka [trade] — demo inside  
   **Angle:** Mobile site hard to use

5. **Subject:** Free 10-min look at AI receptionist  
   **Angle:** Voicemail-only after hours

6–10: Grok generates with `/batch-outreach`

---

## Integration with Digital Product Funnel

Every outreach email footer (optional, small):
```
P.S. I also sell DIY AI business kits if you know an entrepreneur — [STORE]
```

Every closed client → ask for referral → Grok writes:
```
/referral-request [Client Name]
Write a short email asking happy client for 2 referrals. Offer $50 off maintenance for each intro.
```

---

*Pair with `grok_command_playbook.md` and `automated_sales_marketing_plan.md`*