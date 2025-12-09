# EcoComfort Email Flow Templates

This directory contains all HTML email templates for your Klaviyo automation flows.

## Directory Structure

```
emails/
├── README.md (this file)
├── welcome-series/           ✅ 5 emails - COMPLETE
├── abandoned-cart/           ✅ 3 emails - COMPLETE
├── post-purchase/            ⏳ 4 emails - IN PROGRESS
├── browse-abandonment/       📝 2 emails - PENDING
└── winback/                  📝 1 email - PENDING
```

---

## 📧 Email Flow Summary

### 1. Welcome Series Flow (5 emails over 14 days) ✅

**Trigger:** Someone subscribes to email list

| # | Email | Wait Time | Subject Line | File |
|---|-------|-----------|--------------|------|
| 1 | Welcome + 10% Off | Immediate | Welcome to EcoComfort! Here's 10% off 🎁 | `01-welcome-10-percent-off.md` |
| 2 | Education - Chemical Free | Day 2 | What's actually in your current pillow? (It's not good) | `02-education-chemical-free.md` |
| 3 | BOGO Use Cases | Day 5 | Buy 1 Get 1 FREE = Perfect for gifting (or keep both!) | `03-bogo-use-cases.md` |
| 4 | Social Proof | Day 9 | Why 10,000+ Canadians switched to natural bedding | `04-social-proof.md` |
| 5 | Last Chance / Urgency | Day 13 | BOGO ends in 2 days (your 10% code never expires!) | `05-last-chance-urgency.md` |

**Key Codes:** WELCOME10 (10% off, no expiry)

---

### 2. Abandoned Cart Flow (3 emails over 48 hours) ✅

**Trigger:** Cart abandonment (checkout started, not completed)

| # | Email | Wait Time | Subject Line | File |
|---|-------|-----------|--------------|------|
| 1 | Cart Reminder | 1 hour | You left something in your cart | `01-cart-reminder-1-hour.md` |
| 2 | 15% Discount Incentive | 24 hours | Still interested? Here's 15% off | `02-discount-15-percent-24-hours.md` |
| 3 | Last Chance | 48 hours | Your 15% discount expires in 6 hours | `03-last-chance-48-hours.md` |

**Key Codes:** CART15 (15% off, 48-hour validity)

---

### 3. Post-Purchase Flow (4 emails over 90 days) ⏳

**Trigger:** Order placed (purchase completed)

| # | Email | Wait Time | Subject Line | Purpose |
|---|-------|-----------|--------------|---------|
| 1 | Thank You + Tracking | Day 1 | Your order is confirmed! Here's your tracking | Order confirmation + care tips |
| 2 | Check-in + Upsell | Day 7-10 after delivery | How's your new [product]? | Product satisfaction + cross-sell |
| 3 | Review Request | Day 30 | Leave a review, get 20% off your next order | Collect reviews + loyalty discount |
| 4 | Referral Program | Day 60 | Give $20, Get $20 - Refer a friend | Referral incentive |

**Key Codes:** COMFORT10 (10%), REVIEW20 (20% after review)

---

### 4. Browse Abandonment Flow (2 emails) 📝

**Trigger:** Viewed product page, didn't add to cart

| # | Email | Wait Time | Subject Line | Purpose |
|---|-------|-----------|--------------|---------|
| 1 | Product Reminder | 4 hours | Still thinking about [Product]? | Remind about product + offer |
| 2 | Urgency | 24 hours | BOGO ends soon - Buy 1 Get 1 FREE | Create urgency |

---

### 5. Win-Back Flow (1 email) 📝

**Trigger:** No purchase in 90+ days (past customers or engaged subscribers)

| # | Email | Wait Time | Subject Line | Purpose |
|---|-------|-----------|--------------|---------|
| 1 | We Miss You | Day 90 | We miss you! Here's 20% off to come back | Reactivation offer |

**Key Codes:** WELCOME20 (20% off for win-back)

---

## 🎯 Discount Code Summary

| Code | Discount | Usage | Expires |
|------|----------|-------|---------|
| **WELCOME10** | 10% | New subscribers | Never |
| **CART15** | 15% | Abandoned cart recovery | 48 hours |
| **COMFORT10** | 10% | Post-purchase upsell | Never |
| **REVIEW20** | 20% | After leaving review | 30 days |
| **WELCOME20** | 20% | Win-back campaign | 30 days |

**Important:** Create all these codes in Shopify before launching flows!

---

## 🛠️ Setup Instructions

### 1. Create Discount Codes in Shopify

Go to Shopify Admin → Discounts → Create discount code

- **WELCOME10:** 10% off, no expiry, one per customer
- **CART15:** 15% off, no expiry in Shopify (48hr limit in email only), one per customer
- **COMFORT10:** 10% off, no expiry, multiple uses
- **REVIEW20:** 20% off, 30-day expiry, one per customer
- **WELCOME20:** 20% off, 30-day expiry, one per customer

### 2. Import Flows to Klaviyo

For each flow:
1. Klaviyo → Flows → Create Flow → Create from Scratch
2. Set up trigger (e.g., "List - When someone subscribes")
3. Add wait times between emails
4. Copy HTML from `.md` files into email templates
5. Update all variables (domain, unsubscribe link, etc.)
6. Test with test email addresses
7. Set flow to LIVE

### 3. Test Each Flow

**Welcome Series:**
- Subscribe with test email → Check all 5 emails arrive

**Abandoned Cart:**
- Add item to cart → Leave without purchasing → Check 3 emails

**Post-Purchase:**
- Complete test order → Check follow-up emails

---

## ✏️ Customization Checklist

Before launching, update these in ALL emails:

- [ ] Replace `https://ecocomfort.co` with your domain
- [ ] Replace `hello@ecocomfort.co` with your email
- [ ] Update customer testimonials with real reviews
- [ ] Update stats (92%, 87%, etc.) with actual data if available
- [ ] Add `{{unsubscribe_link}}` variable in footers
- [ ] Update BOGO end date from "January 15" as needed
- [ ] Add product images for abandoned cart emails
- [ ] Test all discount codes work at checkout
- [ ] Verify all links work (especially checkout URLs)

---

## 📊 Expected Performance Benchmarks

### Welcome Series
- Open Rate: 35-45% (Email 1), 25-35% (subsequent)
- Click Rate: 5-10%
- Conversion Rate: 3-8%

### Abandoned Cart
- Recovery Rate: 15-25% of carts
- Best performing: Email 2 (with 15% discount)

### Post-Purchase
- Review Collection: 20-30% of customers
- Referral Rate: 5-10% of customers

---

## 🚀 Launch Checklist

- [ ] All discount codes created in Shopify
- [ ] All 5 flows created in Klaviyo
- [ ] All emails customized with your branding
- [ ] Test emails sent and reviewed
- [ ] Unsubscribe links working
- [ ] Mobile responsiveness checked
- [ ] Tracking/UTM parameters added
- [ ] Team trained on responding to email replies

---

## 📁 File Naming Convention

Each file uses this format:
```
[flow-name]/[number]-[description].md
```

Example: `welcome-series/01-welcome-10-percent-off.md`

---

## 🆘 Support

Questions about these templates?
- Check the main execution plan: `/Plan/ECOCOMFORT_HOLIDAY_EXECUTION_PLAN.md`
- Review funnel optimization: `/Plan/FUNNEL_OPTIMIZATION_GUIDE.md`

---

**Total Emails:** 15
**Completed:** 8
**Remaining:** 7

Last Updated: December 2024
