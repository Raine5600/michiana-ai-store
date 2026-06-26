# ConvertKit Setup Checklist — Michiana AI (15 min)

**Storefront:** https://raine5600.github.io/michiana-ai-store/  
**Emails (paste-ready):** `convertkit_emails_ready.md`

---

## Step 1 — Create form (3 min)

1. Go to **https://app.kit.com/forms** → **Create form**
2. Name: **Free AI Launch Checklist**
3. Save form

## Step 2 — Get form ID (1 min)

Open form → **Settings** or **Share** → **HTML embed**

Find this line:
```
action="https://app.convertkit.com/forms/1234567/subscriptions"
```
Copy the number → that's your **FORM_ID**

**Wire it into the storefront:**
```bash
cd ~/Downloads/gumroad-setup
node wire-convertkit-form.mjs FORM_ID
cd ~/Downloads/michiana-ai-store
git add index.html convertkit_emails_ready.md
git commit -m "Connect ConvertKit form"
git push
```

## Step 3 — Tag subscribers (2 min)

Form → **Settings** → **Incentive / After subscribe**:
- Add tag: `launch-kit-lead`

## Step 4 — Create nurture sequence (10 min)

1. **Sequences** → Create **Launch Kit Nurture**
2. Paste each email from `convertkit_emails_ready.md`
3. Set delays: **Day 0**, **+1 day**, **+2 days**, **+2 days**, **+2 days**
4. Enroll new `launch-kit-lead` subscribers automatically

## Step 5 — Test

1. Visit https://raine5600.github.io/michiana-ai-store/#email-capture
2. Submit your email
3. Confirm welcome email arrives + tag applied in Kit

---

## Gumroad links (already in emails)

| Product | URL |
|---------|-----|
| Prompts $47 | https://rainecloud0.gumroad.com/l/xpsfz |
| Website $67 | https://rainecloud0.gumroad.com/l/jdyetn |
| Kit $97 | https://rainecloud0.gumroad.com/l/znalyo |
| Bundle $147 | https://rainecloud0.gumroad.com/l/ucvdgis |

**Subscriber discount code:** `BUNDLE20` (create in Gumroad → Offer codes)