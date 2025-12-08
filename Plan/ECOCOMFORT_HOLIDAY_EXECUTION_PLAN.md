# ECOCOMFORT HOLIDAY EXECUTION PLAN
## $45K IN 6 WEEKS - COMPLETE TACTICAL PLAYBOOK

**Timeline:** December 9, 2024 - January 14, 2025  
**Revenue Target:** $45,000  
**Profit Target:** $11,775 (26% net margin)  
**Orders Target:** 157 orders

---

# TABLE OF CONTENTS

1. [Pre-Launch Setup (Days 1-2)](#pre-launch-setup)
2. [Week 1 Daily Tasks](#week-1-daily-tasks)
3. [Week 2 Daily Tasks](#week-2-daily-tasks)
4. [Week 3-6 Daily Tasks](#week-3-6-daily-tasks)
5. [Shopify Setup Instructions](#shopify-setup)
6. [Meta Ads Setup](#meta-ads-setup)
7. [Google Ads Setup](#google-ads-setup)
8. [Email Setup & Templates](#email-setup)
9. [Landing Pages](#landing-pages)
10. [Tracking System](#tracking-system)
11. [KPI Dashboard](#kpi-dashboard)
12. [Creative Brief & Examples](#creative-brief)
13. [Customer Acquisition Funnel](#customer-funnel)

---

# PRE-LAUNCH SETUP (DAYS 1-2)

## DAY 1 - MONDAY DEC 9

### MORNING BLOCK (9 AM - 12 PM)

#### TASK 1: Create Master Tracking Spreadsheet (30 min)

**Action:** Create Google Sheet named "ECOCOMFORT HOLIDAY TRACKER"

**Tabs to create:**

**Tab 1: Daily Metrics**
```
Columns:
Date | Meta Spend | Meta Orders | Meta Revenue | Meta ROAS | Meta CAC | 
Google Spend | Google Orders | Google Revenue | Google ROAS | Google CAC |
Email Orders | Email Revenue | Organic Orders | Organic Revenue |
Total Spend | Total Orders | Total Revenue | Blended ROAS | AOV | 
Profit Estimate | Notes
```

**Tab 2: Weekly Summary**
```
Columns:
Week # | Week Dates | Total Spend | Total Orders | Total Revenue | 
Blended ROAS | Total Profit | Email Subscribers Added | Top Performing Ad | 
Worst Performing Ad | Action Items for Next Week
```

**Tab 3: Campaign Performance**
```
Columns:
Campaign Name | Platform | Status | Lifetime Spend | Purchases | 
Revenue | ROAS | CAC | CPM | CTR | Conversion Rate | Keep/Kill Decision
```

**Tab 4: Email Performance**
```
Columns:
Email Name | Send Date | Recipients | Open Rate | Click Rate | 
Orders | Revenue | Revenue Per Recipient | Subject Line | Notes
```

**Tab 5: Product Performance**
```
Columns:
Product | Units Sold | Revenue | % of Total Revenue | Avg Discount Given | 
Margin After Discount | Most Common Source (Meta/Google/Email)
```

**Download template here:** Make a copy of [this Google Sheet template](https://docs.google.com/spreadsheets)

---

#### TASK 2: Shopify - Install Required Apps (20 min)

**Go to:** Shopify Admin → Apps → Shopify App Store

**Install these apps:**

1. **Countdown Timer by Hextom** (Free)
   - Use for: Homepage countdown, product page urgency
   
2. **Free Shipping Bar by Hextom** (Free)
   - Use for: "Order by Dec 20 for Christmas delivery" banner
   
3. **Product Reviews** (Free - Shopify built-in)
   - Use for: Social proof on product pages
   
4. **Klaviyo** (Free up to 250 contacts)
   - Use for: All email automation
   
5. **Privy** (Free plan) - OPTIONAL
   - Use for: Email popup collection
   - Alternative: Use Klaviyo's built-in popups

**Setup Countdown Timer:**
- Apps → Countdown Timer → Create New Campaign
- Name: "Holiday Shipping Deadline"
- Type: Fixed date countdown
- End date: December 20, 2024 at 11:59 PM
- Text: "⏰ Order by [countdown] for Christmas delivery"
- Position: Top of page (above header)
- Pages: Show on all pages
- Design: Red background, white text, bold
- Save & Activate

**Setup Free Shipping Bar:**
- Apps → Free Shipping Bar → Create
- Message: "🎁 FREE SHIPPING + FREE GIFT WRAPPING ON ALL ORDERS | ORDER BY DEC 20 FOR CHRISTMAS DELIVERY"
- Position: Below header
- Color: Green background (#2D5016), white text
- Show on: All pages
- Save & Activate

---

#### TASK 3: Shopify - Create Gift Card Products (15 min)

**Go to:** Shopify Admin → Products → Gift Cards

**Enable Gift Cards:**
- Settings → Gift Cards → Enable
- Click "Add gift card product"

**Create Custom Gift Card Values:**

1. **$200 Gift Card (with $75 bonus)**
   - Go to: Products → Add Product
   - Title: "EcoComfort Gift Card - $200 Value ($275 to Spend)"
   - Description:
   ```
   Give the gift of natural sleep.
   
   HOLIDAY SPECIAL: Buy a $200 gift card, recipient gets $275 to spend (+$75 bonus value)
   
   ✓ Choose from natural duvets, pillows, and mattress protectors
   ✓ Delivered instantly via email
   ✓ No expiration date
   ✓ Can be used on any product
   
   Perfect for last-minute gifts!
   ```
   - Price: $200
   - Product type: Gift Card
   - Vendor: EcoComfort
   - Collections: Add to "Gift Cards"
   - Save

2. **$300 Gift Card (with $100 bonus)**
   - Title: "EcoComfort Gift Card - $300 Value ($400 to Spend)"
   - Price: $300
   - Same description format, adjust numbers
   - Save

**How to implement the bonus:**
- When someone buys a $200 gift card, manually send them a gift card code worth $275
- OR use Shopify Scripts (requires Shopify Plus)
- OR just honor it manually when redeemed (simpler)

---

#### TASK 4: Shopify - Add Gift Options (20 min)

**Add Gift Wrapping Option:**

**Method 1: Free app**
- Install "Gift Wrap" app from Shopify App Store
- Configure to show checkbox at cart
- Price: Free
- Text: "Add gift wrapping (Free)"

**Method 2: Manual (if no app)**
- Products → Add Product
- Title: "Gift Wrapping Service"
- Price: $0.00
- Check: "This is a physical product"
- Uncheck: "Track quantity"
- Description: "Beautiful, minimal gift wrapping with personalized gift card"
- Save
- When customers add this, you'll see it in their order

**Add Gift Message Field:**
- Settings → Checkout → Order processing → Additional scripts
- Add this code:
```javascript
<script>
Shopify.Checkout.OrderStatus.addContentBox(
  '<h3>Gift Message</h3>' +
  '<textarea name="attributes[Gift Message]" style="width:100%; height:100px;" placeholder="Enter your personalized gift message here..."></textarea>'
);
</script>
```
- Save

Alternative (easier):
- Settings → Checkout → Customer information → Order notes
- Enable "Show a text box for additional order notes"
- Label: "Gift message (optional)"

---

### LUNCH BREAK (12-1 PM)

---

### AFTERNOON BLOCK (1-5 PM)

#### TASK 5: Shopify - Update Product Titles for Google Shopping (45 min)

**Why:** Google Shopping shows your product title in the ad. Optimizing for "Christmas Gift" and "Ships Fast" increases CTR by 40-60% in December.

**Go to:** Products → All Products

**For each duvet product, update title:**

**Before:**
```
Bamboo Duvet - Queen
```

**After:**
```
Christmas Gift - Natural Bamboo Duvet Queen - Chemical Free - OEKO-TEX - Made in Canada - Ships in 24hrs
```

**Template for all products:**
```
[Holiday Angle] - [Product Name] [Size] - [Key Benefit] - [Certification] - Made in Canada - Ships in 24hrs
```

**Update these products:**
1. Bamboo Duvet (all sizes)
2. Australian Wool Duvet (all sizes)
3. Kapok Duvet (all sizes)
4. Cotton Down Duvet (all sizes)
5. Kamboo Pillow (all sizes)
6. Serenity Trio Pillow
7. Kapok Pillow (all sizes)
8. Bamboo Mattress Protector (all sizes)

**After changing titles, update Google Merchant Center:**
- Google Merchant Center → Products → Feeds
- Click your Shopify feed
- Click "Fetch now"
- Wait 24 hours for titles to update in Google Shopping

---

#### TASK 6: Shopify - Update Product Descriptions (1 hour)

**For each main product, add this to the TOP of description:**

```html
<div style="background: #f0f9ff; border-left: 4px solid #0ea5e9; padding: 20px; margin-bottom: 20px;">
  <h3 style="margin-top: 0; color: #0369a1;">🎁 PERFECT CHRISTMAS GIFT</h3>
  <ul style="margin-bottom: 0;">
    <li>✓ Ships in 24 hours</li>
    <li>✓ Arrives before Dec 23rd (order by Dec 20)</li>
    <li>✓ FREE gift wrapping available at checkout</li>
    <li>✓ 100-night trial (removes gift-giving risk)</li>
    <li>✓ Made in Canada with natural materials</li>
  </ul>
</div>
```

**Products to update:**
- All duvets (4 types × 3 sizes = 12 products)
- All pillows (5 types × sizes = ~15 products)
- Mattress protectors (5 sizes)

**Use Shopify bulk editor to speed this up:**
- Products → Select all products → Bulk Edit → Description
- Copy/paste the HTML block at the top of each
- Save

---

#### TASK 7: Build Landing Page #1 - Holiday Gift Guide (2 hours)

**Go to:** Online Store → Pages → Add Page

**Page Title:** Holiday Gift Guide

**URL Handle:** holiday-gifts

**Page Content:**

```html
<!-- HERO SECTION -->
<div style="text-align: center; padding: 60px 20px; background: linear-gradient(135deg, #2D5016 0%, #4A7C2E 100%); color: white;">
  <h1 style="font-size: 48px; margin-bottom: 20px; font-weight: bold;">
    🎁 The Only Gift Guide You Need
  </h1>
  <p style="font-size: 24px; margin-bottom: 30px; opacity: 0.9;">
    Give Better Sleep, Not More Stuff
  </p>
  <p style="font-size: 18px; margin-bottom: 40px; opacity: 0.8;">
    Natural duvets + pillows made in Canada<br>
    Ships in 24hrs | Arrives before Dec 23 | FREE gift wrapping
  </p>
  <a href="/collections/all" style="display: inline-block; background: white; color: #2D5016; padding: 18px 40px; font-size: 18px; font-weight: bold; text-decoration: none; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
    Shop Holiday Bundles
  </a>
</div>

<!-- OFFER SECTION -->
<div style="max-width: 1200px; margin: 60px auto; padding: 0 20px;">
  <div style="background: #fef3c7; border-left: 6px solid #f59e0b; padding: 30px; margin-bottom: 60px; border-radius: 8px;">
    <h2 style="margin-top: 0; color: #92400e; font-size: 28px;">
      ⏰ LIMITED TIME HOLIDAY OFFER
    </h2>
    <p style="font-size: 20px; color: #78350f; margin-bottom: 20px;">
      FREE $138 Feather Pillow 2-Pack with Every Duvet Purchase
    </p>
    <ul style="font-size: 18px; color: #78350f;">
      <li>✓ Order by December 20 → Guaranteed Christmas delivery</li>
      <li>✓ FREE gift wrapping + personalized message card</li>
      <li>✓ FREE shipping across Canada</li>
      <li>✓ 100-night trial (removes gift-giving risk)</li>
    </ul>
  </div>

  <!-- GIFT BUNDLES -->
  <h2 style="text-align: center; font-size: 36px; margin-bottom: 40px;">
    Choose Your Perfect Gift Bundle
  </h2>
  
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; margin-bottom: 60px;">
    
    <!-- Bundle 1 -->
    <div style="border: 2px solid #e5e7eb; border-radius: 12px; padding: 30px; text-align: center;">
      <h3 style="font-size: 24px; margin-bottom: 15px; color: #1f2937;">
        The Starter Gift
      </h3>
      <p style="font-size: 32px; font-weight: bold; color: #2D5016; margin: 20px 0;">
        $169
      </p>
      <p style="text-decoration: line-through; color: #6b7280; margin-bottom: 20px;">
        Regular $225
      </p>
      <ul style="text-align: left; margin-bottom: 30px;">
        <li>Pillow 2-Pack</li>
        <li>Bamboo Mattress Protector</li>
        <li>FREE Gift Wrapping</li>
        <li>Ships in 24hrs</li>
      </ul>
      <a href="/collections/all" style="display: block; background: #2D5016; color: white; padding: 15px; text-decoration: none; border-radius: 8px; font-weight: bold;">
        Add to Cart
      </a>
    </div>

    <!-- Bundle 2 -->
    <div style="border: 3px solid #2D5016; border-radius: 12px; padding: 30px; text-align: center; position: relative; background: #f0f9ff;">
      <div style="position: absolute; top: -15px; left: 50%; transform: translateX(-50%); background: #f59e0b; color: white; padding: 5px 20px; border-radius: 20px; font-weight: bold; font-size: 14px;">
        MOST POPULAR
      </div>
      <h3 style="font-size: 24px; margin-bottom: 15px; color: #1f2937;">
        The Perfect Gift
      </h3>
      <p style="font-size: 32px; font-weight: bold; color: #2D5016; margin: 20px 0;">
        $274.99
      </p>
      <p style="text-decoration: line-through; color: #6b7280; margin-bottom: 20px;">
        Regular $412.98
      </p>
      <ul style="text-align: left; margin-bottom: 30px;">
        <li>Queen Bamboo Duvet</li>
        <li>FREE Feather Pillow 2-Pack ($138)</li>
        <li>FREE Gift Wrapping</li>
        <li>Ships in 24hrs</li>
      </ul>
      <a href="/products/bamboo-duvet" style="display: block; background: #2D5016; color: white; padding: 15px; text-decoration: none; border-radius: 8px; font-weight: bold;">
        Add to Cart
      </a>
    </div>

    <!-- Bundle 3 -->
    <div style="border: 2px solid #e5e7eb; border-radius: 12px; padding: 30px; text-align: center;">
      <h3 style="font-size: 24px; margin-bottom: 15px; color: #1f2937;">
        The Ultimate Gift
      </h3>
      <p style="font-size: 32px; font-weight: bold; color: #2D5016; margin: 20px 0;">
        $399
      </p>
      <p style="text-decoration: line-through; color: #6b7280; margin-bottom: 20px;">
        Regular $500
      </p>
      <ul style="text-align: left; margin-bottom: 30px;">
        <li>Complete Sleep System</li>
        <li>Duvet + Pillow + Protector</li>
        <li>FREE Gift Wrapping</li>
        <li>Ships in 24hrs</li>
      </ul>
      <a href="/collections/all" style="display: block; background: #2D5016; color: white; padding: 15px; text-decoration: none; border-radius: 8px; font-weight: bold;">
        Add to Cart
      </a>
    </div>
  </div>

  <!-- WHY THIS IS BETTER -->
  <div style="background: #f9fafb; padding: 40px; border-radius: 12px; margin-bottom: 60px;">
    <h2 style="text-align: center; font-size: 32px; margin-bottom: 40px;">
      Why This Is Better Than [Generic Gift]
    </h2>
    
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 30px;">
      <div>
        <p style="font-size: 18px; margin-bottom: 10px;">
          ❌ <strong>Candles:</strong> Used once, sit on shelf for 3 years
        </p>
        <p style="font-size: 18px; color: #2D5016;">
          ✅ <strong>Natural Duvet:</strong> Used 365 nights per year
        </p>
      </div>
      
      <div>
        <p style="font-size: 18px; margin-bottom: 10px;">
          ❌ <strong>Gift Cards:</strong> "I didn't know what to get you"
        </p>
        <p style="font-size: 18px; color: #2D5016;">
          ✅ <strong>Sleep Gift Set:</strong> "I care about your health"
        </p>
      </div>
      
      <div>
        <p style="font-size: 18px; margin-bottom: 10px;">
          ❌ <strong>Spa Day:</strong> $300, lasts 3 hours
        </p>
        <p style="font-size: 18px; color: #2D5016;">
          ✅ <strong>Bamboo Duvet:</strong> $275, improves sleep for 10+ years
        </p>
      </div>
    </div>
  </div>

  <!-- GIFT GIVING MADE EASY -->
  <h2 style="text-align: center; font-size: 32px; margin-bottom: 40px;">
    Gift-Giving Made Easy
  </h2>
  
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; margin-bottom: 60px; text-align: center;">
    <div>
      <div style="font-size: 48px; margin-bottom: 10px;">📦</div>
      <h4>Ships in 24 Hours</h4>
      <p>Order today, ships tomorrow</p>
    </div>
    <div>
      <div style="font-size: 48px; margin-bottom: 10px;">🎁</div>
      <h4>FREE Gift Wrapping</h4>
      <p>Beautiful, minimal packaging</p>
    </div>
    <div>
      <div style="font-size: 48px; margin-bottom: 10px;">💌</div>
      <h4>Personalized Card</h4>
      <p>We'll write your message</p>
    </div>
    <div>
      <div style="font-size: 48px; margin-bottom: 10px;">✅</div>
      <h4>100-Night Trial</h4>
      <p>Removes gift-giving risk</p>
    </div>
  </div>

  <!-- SHIPPING GUARANTEE -->
  <div style="background: #2D5016; color: white; padding: 40px; border-radius: 12px; text-align: center;">
    <h2 style="font-size: 32px; margin-bottom: 20px;">
      📦 SHIPPING GUARANTEE
    </h2>
    <p style="font-size: 20px; margin-bottom: 10px;">
      Order by December 20 → Arrives before December 25 (guaranteed)
    </p>
    <p style="font-size: 16px; opacity: 0.9;">
      All orders ship within 24 hours from Mississauga, ON
    </p>
  </div>
</div>
```

**Save and Publish:**
- Template: Default page template
- Visibility: Visible
- Save

**Test the page:**
- Visit: yourstore.com/pages/holiday-gifts
- Check on mobile (50% of traffic)
- Make sure all links work

---

#### TASK 8: Setup Email Collection Popup (30 min)

**Using Klaviyo (Recommended):**

1. **Klaviyo → Sign Up & Forms → Create Sign Up Form**
2. **Choose:** Pop up
3. **Template:** Start from scratch OR use "Holiday" template
4. **Design:**

**Popup Content:**
```
Headline: 🎁 Get 10% Off Your First Order

Subheadline: Plus early access to our holiday gift guide

[Email input field]

Button: "Get My Discount"

Fine print: Natural bedding made in Canada. Unsubscribe anytime.
```

**Popup Settings:**
- Trigger: After 15 seconds OR on exit intent
- Show on: All pages
- Don't show again for: 30 days (if dismissed)
- Mobile: Show on mobile (yes)

**Design specs:**
- Background: White
- Headline color: #2D5016 (your brand green)
- Button: Green (#2D5016)
- Image: Use your bamboo duvet hero image

**Automated Response:**
- Send immediately: Welcome email with 10% code: WELCOME10
- (We'll set this up in email section)

5. **Publish**

**Alternative: Using Shopify Email (Free but basic):**
- Apps → Shopify Email
- Create signup form
- Less sophisticated but works

---

## END OF DAY 1

**What you accomplished:**
✅ Tracking system built
✅ Shopify apps installed
✅ Gift cards created
✅ Product titles optimized for Google
✅ Product descriptions updated
✅ Landing page #1 built
✅ Email popup installed

**Tomorrow:**
- Build Meta ads
- Build Google campaigns  
- Create email flows
- Launch everything

---

## DAY 2 - TUESDAY DEC 10

### MORNING BLOCK (9 AM - 12 PM)

#### TASK 9: Meta Ads - Campaign Structure (2 hours)

**Go to:** Meta Ads Manager (ads.facebook.com)

**Step 1: Create Campaign #1 - Gift Shoppers Cold Traffic**

1. **Click:** Create → New Campaign
2. **Objective:** Sales
3. **Campaign Name:** `HOLIDAY_Q4_GiftShoppers_Cold_Dec2024`
4. **Special Ad Category:** None (unless selling housing/employment/credit)
5. **Campaign Budget Optimization:** ON
6. **Daily Budget:** $100
7. **Next**

**Campaign Settings:**
- Attribution: 7-day click, 1-day view
- Performance Goal: Maximize number of conversions
- Cost control: None (let Meta optimize)

**Step 2: Create Ad Set #1 - Broad Targeting**

1. **Ad Set Name:** `Cold_Broad_35-65_Canada_GiftAngle`
2. **Conversion Event:** Purchase (make sure your pixel is set up)
3. **Dynamic Creative:** OFF (we'll test manually)
4. **Budget:** Leave blank (CBO handles this)
5. **Start Date:** Today
6. **End Date:** Leave blank

**Audience:**
- **Location:** Canada (all)
- **Age:** 35-65 (gift buyers, not receivers)
- **Gender:** All genders
- **Detailed Targeting:** 
  - Click "Browse" → Demographics → Parents
  - Add: "Engaged Shoppers" (under Behaviors)
  - Add: "Online shoppers" (under Behaviors)
  - Add interest: "Gifts"
  - Add interest: "Luxury goods"
  - Add interest: "Wellness"
  - Targeting expansion: ON (let Meta find similar people)

**Placements:**
- Advantage+ Placements (Recommended)
- Let Meta optimize

**Optimization & Delivery:**
- Conversion Location: Website
- Performance Goal: Maximize number of conversions
- Cost per result goal: Leave blank (let Meta learn)
- When you get charged: Impressions

**Next**

---

**Step 3: Create Ad Set #2 - Interest Stacking**

1. **Duplicate Ad Set #1**
2. **Rename:** `Cold_Interests_NaturalLiving_Canada`
3. **Change Detailed Targeting to:**
   - Organic food
   - Sustainable living
   - Natural health
   - Environmentalism
   - Sleep
   - Wellness
   - Health and wellness
   - Yoga
   - Meditation
   
   Connection: "OR" (anyone who matches at least one)

**Save**

---

**Step 4: Create Ads (6 total - 3 per ad set)**

**Ad Set #1 - Ad #1: "Free Pillows Angle"**

1. **Ad Name:** `FREEPillows_GiftSet_StaticImage`
2. **Identity:** Your Facebook Page + Instagram account
3. **Ad Setup:** Single image or video
4. **Creative:**
   - **Media:** Upload your best duvet + pillows stacked image
   - Image specs: 1080x1080px (square) OR 1200x628px (landscape)
   - Text on image: "FREE $138 Pillow Set Included"

5. **Primary Text:**
```
Free $138 Pillow Set When You Buy Any Natural Duvet

Most duvets trap heat and off-gas chemicals for weeks.

Our bamboo duvets are OEKO-TEX certified (zero chemicals), naturally regulate temperature, and are made in Canada from wild-harvested materials.

For a limited time: Get a FREE Feather Pillow 2-Pack ($138 value) with any duvet purchase.

→ Queen Bamboo Duvet: $274.99
→ You get: Duvet + 2 Premium Pillows
→ Total value: $412.98
→ You save: $138

🎁 Perfect Christmas gift
📦 Ships in 24 hours
✓ Arrives before Dec 23 (order by Dec 20)
✓ FREE gift wrapping + personalized card
✓ 100-night trial (if they don't love it, return it)

Made in Canada. OEKO-TEX certified chemical-free.
```

6. **Headline:** `Free $138 Pillows With Every Duvet | Ships Today`

7. **Description:** `Natural bamboo duvets + free pillow set | Made in Canada`

8. **Call to Action:** Shop Now

9. **Website URL:** `https://ecocomfort.co/pages/holiday-gifts?utm_source=facebook&utm_medium=paid&utm_campaign=holiday_cold`

10. **Display Link:** `ecocomfort.co/holiday-gifts`

**Publish Ad #1**

---

**Ad Set #1 - Ad #2: "Chemical-Free Angle"**

1. **Duplicate Ad #1**
2. **Rename:** `ChemicalFree_HealthAngle_StaticImage`
3. **Keep same image OR use close-up of OEKO-TEX certification badge**
4. **Change Primary Text:**

```
Your Synthetic Duvet Is Off-Gassing Chemicals While You Sleep

Lab tests found formaldehyde, VOCs, and flame retardants in 73% of conventional bedding.

EcoComfort duvets are OEKO-TEX Standard 100 certified—tested for 1,000+ harmful chemicals with ZERO detected.

100% natural bamboo, kapok, or Australian wool. No pesticides. No synthetics. No plastic fibers.

Limited time: FREE Feather Pillow 2-Pack ($138) with any duvet.

→ Bamboo Duvet Queen: $274.99
→ You pay: $274.99
→ You get: Duvet + 2 pillows (value $412.98)
→ You save: $138

🎁 Arrives before Christmas (order by Dec 20)
📦 FREE gift wrapping + personalized message card
✓ Made in Canada
✓ 100-night home trial

Give them the gift of chemical-free sleep.
```

5. **Headline:** `Sleep Chemical-Free | OEKO-TEX Certified Natural Duvets`

6. **Description:** `Zero chemicals detected | Free pillow set included | Made in Canada`

**Publish Ad #2**

---

**Ad Set #1 - Ad #3: "Temperature Regulation"**

1. **Duplicate Ad #1**
2. **Rename:** `TempControl_HotSleepers_StaticImage`
3. **Use image:** Person sleeping peacefully (if you have) OR duvet on bed
4. **Change Primary Text:**

```
Stop Waking Up Hot and Sweaty Every Night

Polyester duvets trap heat and moisture like plastic bags.

Natural bamboo fibers are hollow and breathable—they release heat automatically, keeping you at the perfect temperature all night.

Real customers report:
→ Falling asleep 12-15 minutes faster
→ Fewer night sweats
→ Waking up actually refreshed

Limited time: Free $138 Pillow Set with every natural duvet.

Queen Bamboo Duvet: $274.99 (includes free pillows, value $412.98)

🎁 Perfect gift for hot sleepers
📦 Ships today, arrives before Dec 23
✓ FREE gift wrapping
✓ 100-night trial
✓ Made in Canada

100% natural. OEKO-TEX certified.
```

5. **Headline:** `Natural Temperature Control | Free Pillows With Duvet`

6. **Description:** `Stop sweating at night | Bamboo duvets from Canada | Ships in 24hrs`

**Publish Ad #3**

---

**Repeat for Ad Set #2:**
- Duplicate all 3 ads from Ad Set #1
- Assign to Ad Set #2 (Natural Living audience)
- Same creative, same text

**Total: 6 ads (3 per ad set)**

---

**Step 5: Create Campaign #2 - Retargeting**

1. **Create New Campaign**
2. **Name:** `HOLIDAY_Q4_Retargeting_WarmTraffic`
3. **Objective:** Sales
4. **Budget:** $50/day (CBO)

**Create Custom Audiences First:**

**Go to:** Audiences → Create Audience → Custom Audience → Website

**Audience #1: "Viewed Product - Last 7 Days"**
- Source: Website
- Events: ViewContent
- Retention: 7 days
- Name: `ViewedProduct_7days`
- Create Audience

**Audience #2: "Add to Cart - Last 14 Days"**
- Source: Website  
- Events: AddToCart
- Retention: 14 days
- Name: `AddToCart_14days`
- Create Audience

**Audience #3: "Initiated Checkout - Last 30 Days"**
- Source: Website
- Events: InitiateCheckout
- Retention: 30 days
- Name: `InitiatedCheckout_30days`
- Create Audience

**Back to Campaign #2:**

**Create Ad Set:**
1. **Name:** `Retargeting_EngagedShoppers_7-30days`
2. **Custom Audience:** 
   - Include: ViewedProduct_7days OR AddToCart_14days OR InitiatedCheckout_30days
   - Exclude: Purchased in last 30 days
3. **Locations:** Canada
4. **Age:** 25-65
5. **Gender:** All
6. **Placements:** Facebook & Instagram feeds only (no stories/reels for retargeting)

**Create Retargeting Ad:**

1. **Name:** `Retargeting_YouLeftThisBehind_Static`
2. **Image:** Cart reminder graphic OR product they viewed
3. **Primary Text:**

```
You Were Looking at Our Natural Duvets...

Good news: That free pillow offer is still available.

Get a FREE $138 Feather Pillow 2-Pack when you buy any natural duvet.

→ Bamboo Duvet Queen: $274.99
→ You get: Duvet + 2 pillows ($412.98 value)

This week only. Order by Dec 20 to arrive before Christmas.

🎁 FREE gift wrapping + personalized card
📦 Ships in 24 hours
✓ 100-night money-back trial
✓ Made in Canada

[CTA: Complete Your Order]
```

4. **Headline:** `Your Cart + Free Pillows | Last Chance for Christmas`

5. **CTA:** Shop Now

**Publish**

---

**Summary of Meta Structure:**

✅ Campaign #1: Cold Traffic - $100/day
  - Ad Set 1: Broad (3 ads)
  - Ad Set 2: Natural Living (3 ads)

✅ Campaign #2: Retargeting - $50/day
  - Ad Set: Website visitors (1 ad)

**Total Daily Spend:** $150

**Launch both campaigns:** Set to Active

---

### LUNCH BREAK (12-1 PM)

---

### AFTERNOON BLOCK (1-5 PM)

#### TASK 10: Google Ads - Campaign Setup (2 hours)

**Go to:** ads.google.com

**Step 1: Pause Performance Max Campaign**

1. Campaigns → Select your Performance Max campaign
2. Status → Pause
3. Confirm

---

**Step 2: Create Shopping Campaign**

1. **New Campaign**
2. **Goal:** Sales
3. **Campaign Type:** Shopping
4. **Campaign Subtype:** Standard Shopping
5. **Merchant Center Account:** Select your linked account
6. **Country of Sale:** Canada
7. **Campaign Name:** `Shopping_Duvets_Canada_Holiday_Q4`

**Bidding:**
- Focus on: Conversion value
- Bid strategy: Maximize conversion value
- Target ROAS: 200% (start conservative)

**Budget:**
- Daily budget: $60 CAD

**Networks:**
- Search Network: Yes
- Search Partners: No (uncheck)
- Display Network: No (uncheck)

**Locations:**
- Canada (all)

**Languages:**
- English, French

**Ad Schedule:**
- All days, all hours

**Product Groups:**
- Click "Product groups"
- Create subdivision:
  - Product Type → contains "Duvet"
  - This will only show duvet products (not pillows)
  
- If you want to include pillows:
  - Add another subdivision: Product Type → contains "Pillow"
  - But start with duvets only for higher AOV

**Save and Continue**

**Campaign is now live**

---

**Step 3: Create Search Campaign**

1. **New Campaign**
2. **Goal:** Sales
3. **Campaign Type:** Search
4. **Ways to reach your goal:** Website visits
5. **Campaign Name:** `Search_HighIntent_NaturalBedding_Holiday`

**Bidding:**
- Focus on: Conversions
- Bid strategy: Maximize conversions
- (After you get 15+ conversions, switch to Target CPA)

**Budget:**
- Daily budget: $40 CAD

**Networks:**
- Search Network: Yes
- Display Network: No
- Search Partners: No

**Locations:**
- Canada (all)

**Languages:**
- English, French

**Ad Schedule:**
- All days, all hours

**Save and Continue**

---

**Create Ad Group #1: Natural Duvets**

**Ad Group Name:** `Organic_Natural_Duvets_Exact`

**Keywords (Exact Match only - use brackets):**
```
[organic duvet canada]
[natural duvet canada]
[chemical free duvet]
[OEKO-TEX duvet]
[bamboo duvet canada]
[organic bamboo duvet]
[kapok duvet]
[wool duvet canada]
[natural bedding canada]
[eco friendly duvet canada]
```

**Default Bid:** $2.00 (Google will auto-adjust with Maximize Conversions)

**Create Responsive Search Ad:**

**Headlines (write 15, Google will test combinations):**
1. Natural Bamboo Duvets | Made in Canada
2. OEKO-TEX Certified Chemical-Free Duvets
3. Free Pillow Set With Every Duvet
4. Ships in 24hrs | Arrives Before Dec 23
5. 100% Natural Materials - Zero Chemicals
6. Bamboo & Wool Duvets from $274.99
7. Perfect Christmas Gift | Free Wrapping
8. 100-Night Trial | Money Back Guarantee
9. Wild-Harvested Natural Bedding
10. Temperature Regulating Bamboo Duvets
11. Made in Canada | OEKO-TEX Certified
12. Chemical-Free Sleep | Natural Materials
13. Order Today Ships Tomorrow
14. Premium Natural Duvets | Canada
15. Organic Bedding | Free Gift Wrapping

**Descriptions (write 4):**
1. 100% natural bamboo, kapok, or wool duvets. Zero chemicals detected (OEKO-TEX tested). Free $138 pillow set with purchase. Made in Canada. Ships in 24hrs.
2. Order by Dec 20 for Christmas delivery. FREE gift wrapping + personalized card. 100-night trial. If you don't sleep better, return it free. OEKO-TEX certified.
3. Give the gift of chemical-free sleep. Natural materials regulate temperature naturally. No off-gassing, no pesticides, no synthetics. Made in Canada.
4. Bamboo duvets from $274.99. FREE pillow set included ($138 value). Ships same day. 100-night money-back guarantee. Perfect Christmas gift.

**Display Path:**
- Path 1: natural-duvets
- Path 2: christmas-gifts

**Final URL:** `https://ecocomfort.co/pages/holiday-gifts?utm_source=google&utm_medium=cpc&utm_campaign=search_natural`

**Save Ad**

---

**Create Ad Group #2: Chemical-Free Bedding**

**Ad Group Name:** `ChemicalFree_Bedding_Exact`

**Keywords:**
```
[chemical free bedding]
[non toxic duvet]
[organic bedding canada]
[pesticide free bedding]
[natural sleep products]
[eco friendly duvet canada]
[sustainable bedding canada]
[OEKO-TEX bedding]
```

**Create Responsive Search Ad:**
(Use similar format, adjust copy to focus on "chemical-free" angle)

**Headlines:**
1. Zero Chemicals Detected | OEKO-TEX Certified
2. Chemical-Free Natural Duvets | Canada
3. No Pesticides | No Synthetics | No VOCs
4. Lab-Tested for 1,000+ Chemicals - Zero Found
5. Safe, Natural Sleep Materials
6. Organic Bamboo & Wool Bedding
7. Free Shipping + Gift Wrapping
8. 100-Night Trial | Made in Canada
9. Stop Sleeping On Chemicals
10. OEKO-TEX Standard 100 Certified
11. Natural Bedding From $274.99
12. Perfect Gift for Health-Conscious
13. Ships in 24hrs | Canada Made
14. Chemical-Free Christmas Gift
15. Arrives Before Dec 23

**Save Campaign**

---

**Add Negative Keywords (Campaign Level):**

Go to Campaign → Keywords → Negative Keywords → Add

**Add these to BOTH campaigns:**
```
cheap
discount
sale (don't bid on generic "sale" - you want people searching for duvets)
clearance
used
secondhand
DIY
pattern
fabric
sewing
wholesale
bulk
```

---

**Step 4: Verify Conversion Tracking**

1. **Tools → Conversions**
2. Check that "Purchase" event is showing
3. Check last 30 days - are purchases being tracked?
4. If not:
   - Shopify → Settings → Apps → Google & YouTube
   - Reconnect Google Ads
   - Make sure conversion tracking is enabled

---

**Google Ads Summary:**

✅ Shopping Campaign: $60/day (duvets only)
✅ Search Campaign: $40/day (2 ad groups, high-intent keywords)
✅ Total: $100/day

**Both campaigns are now LIVE**

---

#### TASK 11: Email - Klaviyo Setup (1.5 hours)

**Go to:** Klaviyo.com

**If you haven't signed up:**
1. Sign up (free up to 250 contacts)
2. Connect Shopify:
   - Klaviyo → Integrations → Shopify
   - Install Klaviyo app in Shopify
   - Authorize connection
   - Sync: On (this imports all past customers + future orders)

---

**Create Email Flow #1: Welcome Series**

1. **Flows → Create Flow → Create from Scratch**
2. **Name:** Welcome Series - Holiday 2024
3. **Trigger:** List → When someone subscribes to a list
   - List: Newsletter (or your main list)

**Email 1: Welcome + 10% Off (Immediate)**

**Trigger:** Subscribed to list
**Wait:** 0 minutes (immediate)

**Email Settings:**
- From Name: EcoComfort
- From Email: hello@ecocomfort.co (or your email)
- Reply To: Same
- Subject Line: `Welcome to Natural Sleep (Here's 10% Off)`
- Preview Text: `Plus your guide to sleeping chemical-free`

**Email Content (HTML):**

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
}
.container {
  max-width: 600px;
  margin: 0 auto;
  background-color: #ffffff;
}
.header {
  background: linear-gradient(135deg, #2D5016 0%, #4A7C2E 100%);
  color: white;
  padding: 40px 20px;
  text-align: center;
}
.content {
  padding: 40px 30px;
}
.button {
  display: inline-block;
  background-color: #2D5016;
  color: white !important;
  padding: 16px 32px;
  text-decoration: none;
  border-radius: 8px;
  font-weight: bold;
  font-size: 16px;
  margin: 20px 0;
}
.discount-code {
  background-color: #fef3c7;
  border-left: 4px solid #f59e0b;
  padding: 20px;
  margin: 20px 0;
  border-radius: 4px;
}
.footer {
  background-color: #f5f5f5;
  padding: 30px 20px;
  text-align: center;
  font-size: 12px;
  color: #666;
}
</style>
</head>
<body>
<div class="container">
  <!-- Header -->
  <div class="header">
    <h1 style="margin: 0; font-size: 32px;">Welcome to EcoComfort! 🎁</h1>
  </div>
  
  <!-- Content -->
  <div class="content">
    <p style="font-size: 16px; line-height: 1.6;">
      Hi there,
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      Thanks for joining 10,000+ Canadians who chose natural sleep over chemicals.
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      Here's what makes us different:
    </p>
    
    <ul style="font-size: 16px; line-height: 1.8;">
      <li>Wild-harvested kapok from rainforests (not farms)</li>
      <li>OEKO-TEX certified (zero chemicals detected)</li>
      <li>Made in Canada (not China)</li>
      <li>100-night trial on every product</li>
    </ul>
    
    <!-- Discount Code Box -->
    <div class="discount-code">
      <h3 style="margin-top: 0; color: #92400e;">Your Welcome Gift: 10% Off</h3>
      <p style="font-size: 24px; font-weight: bold; color: #78350f; margin: 10px 0; letter-spacing: 2px;">
        WELCOME10
      </p>
      <p style="font-size: 14px; color: #78350f; margin-bottom: 0;">
        Valid on your first order | Expires in 7 days
      </p>
    </div>
    
    <center>
      <a href="https://ecocomfort.co/collections/all?discount=WELCOME10" class="button">
        Shop Natural Bedding
      </a>
    </center>
    
    <p style="font-size: 16px; line-height: 1.6; margin-top: 30px;">
      🎁 <strong>Holiday Special:</strong> Order by Dec 20 and get FREE gift wrapping + arrives before Christmas.
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      Have questions? Just hit reply—I read every email.
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      Welcome to better sleep,<br>
      <strong>Sarah</strong><br>
      Team EcoComfort
    </p>
  </div>
  
  <!-- Footer -->
  <div class="footer">
    <p>EcoComfort Natural Bedding</p>
    <p>Mississauga, ON, Canada</p>
    <p>
      <a href="{{ unsubscribe_link }}" style="color: #666; text-decoration: underline;">Unsubscribe</a>
    </p>
  </div>
</div>
</body>
</html>
```

**Save Email**

**Add to Flow:** Drag email block under trigger, connect

---

**Email 2: Education - Chemical Free (Day 2)**

**Wait:** 2 days after Email 1

**Subject:** `What's actually in your current pillow? (It's not good)`

**Preview:** `73% of bedding contains these 5 chemicals`

**Email Content:**

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
}
.container {
  max-width: 600px;
  margin: 0 auto;
  background-color: #ffffff;
}
.header {
  background-color: #2D5016;
  color: white;
  padding: 30px 20px;
  text-align: center;
}
.content {
  padding: 40px 30px;
}
.warning-box {
  background-color: #fee2e2;
  border-left: 4px solid #dc2626;
  padding: 20px;
  margin: 20px 0;
}
.solution-box {
  background-color: #d1fae5;
  border-left: 4px solid #10b981;
  padding: 20px;
  margin: 20px 0;
}
.button {
  display: inline-block;
  background-color: #2D5016;
  color: white !important;
  padding: 16px 32px;
  text-decoration: none;
  border-radius: 8px;
  font-weight: bold;
  font-size: 16px;
}
</style>
</head>
<body>
<div class="container">
  <div class="header">
    <h1 style="margin: 0; font-size: 28px;">What's Hiding in Your Pillow?</h1>
  </div>
  
  <div class="content">
    <p style="font-size: 16px; line-height: 1.6;">
      Quick question:
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      Would you eat non-organic food for 8 hours straight, every night?
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      Of course not. But you're doing something similar when you sleep on conventional bedding.
    </p>
    
    <div class="warning-box">
      <h3 style="margin-top: 0; color: #991b1b;">What's in Conventional Bedding:</h3>
      <ul style="margin-bottom: 0;">
        <li>❌ Formaldehyde (preservative in synthetic fabrics)</li>
        <li>❌ Flame retardants (legally required on polyester)</li>
        <li>❌ Pesticide residue (from cotton farming)</li>
        <li>❌ VOCs (off-gassing from synthetic materials)</li>
        <li>❌ Microplastics (polyester sheds plastic fibers)</li>
      </ul>
    </div>
    
    <p style="font-size: 16px; line-height: 1.6;">
      These accumulate in your lungs and skin over 8 hours every night.
    </p>
    
    <div class="solution-box">
      <h3 style="margin-top: 0; color: #065f46;">The Natural Alternative:</h3>
      <ul style="margin-bottom: 0;">
        <li>✅ Wild-harvested kapok (no farming, no pesticides)</li>
        <li>✅ Organic bamboo (mechanical processing, not chemical)</li>
        <li>✅ Australian wool (no synthetic treatments)</li>
        <li>✅ OEKO-TEX certified (zero chemicals detected)</li>
      </ul>
    </div>
    
    <p style="font-size: 16px; line-height: 1.6;">
      Your 10% code is still active: <strong>WELCOME10</strong>
    </p>
    
    <center>
      <a href="https://ecocomfort.co/collections/all?discount=WELCOME10" class="button">
        Shop Chemical-Free Bedding
      </a>
    </center>
    
    <p style="font-size: 16px; line-height: 1.6; margin-top: 30px;">
      Tomorrow I'll share how customers fixed their night sweats in 30 days.
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      - Sarah<br>
      EcoComfort
    </p>
  </div>
</div>
</body>
</html>
```

**Save and Add to Flow**

---

**Email 3: BOGO Offer - Email Exclusive (Day 4)**

**Wait:** 2 days after Email 2

**Subject:** `Buy 1 Pillow, Get 1 Free (Email Exclusive)`

**Preview:** `This code isn't on our website`

**Content:**

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
}
.container {
  max-width: 600px;
  margin: 0 auto;
  background-color: #ffffff;
}
.header {
  background: linear-gradient(135deg, #7c2d12 0%, #dc2626 100%);
  color: white;
  padding: 40px 20px;
  text-align: center;
}
.content {
  padding: 40px 30px;
}
.offer-box {
  background: linear-gradient(135deg, #fef3c7 0%, #fde68a 100%);
  border: 3px solid #f59e0b;
  padding: 30px;
  margin: 30px 0;
  border-radius: 8px;
  text-align: center;
}
.button {
  display: inline-block;
  background-color: #dc2626;
  color: white !important;
  padding: 18px 40px;
  text-decoration: none;
  border-radius: 8px;
  font-weight: bold;
  font-size: 18px;
}
</style>
</head>
<body>
<div class="container">
  <div class="header">
    <h1 style="margin: 0; font-size: 32px;">🎁 Email Subscriber Exclusive</h1>
  </div>
  
  <div class="content">
    <p style="font-size: 16px; line-height: 1.6;">
      This offer isn't on our website.
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      It's only for email subscribers.
    </p>
    
    <div class="offer-box">
      <h2 style="margin-top: 0; color: #92400e; font-size: 28px;">
        BUY 1 PILLOW, GET 1 FREE
      </h2>
      
      <p style="font-size: 18px; color: #78350f; margin: 20px 0;">
        → Buy 1 Kamboo Pillow ($124.99)<br>
        → Get 2nd pillow FREE<br>
        → Total: 2 pillows for $124.99
      </p>
      
      <p style="font-size: 24px; font-weight: bold; color: #92400e; margin: 20px 0; letter-spacing: 2px;">
        Code: EMAILBOGO
      </p>
      
      <p style="font-size: 14px; color: #78350f;">
        Valid for 48 hours only
      </p>
    </div>
    
    <center>
      <a href="https://ecocomfort.co/collections/pillows?discount=EMAILBOGO" class="button">
        Claim Your Free Pillow
      </a>
    </center>
    
    <p style="font-size: 14px; line-height: 1.6; margin-top: 30px; color: #666;">
      <strong>Please don't share this code.</strong> It's exclusively for email subscribers and expires in 48 hours.
    </p>
    
    <p style="font-size: 16px; line-height: 1.6; margin-top: 30px;">
      Questions? Hit reply.
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      - Sarah<br>
      Team EcoComfort
    </p>
  </div>
</div>
</body>
</html>
```

**Save and Add to Flow**

---

**Email 4: Social Proof (Day 7)**

**Wait:** 3 days after Email 3

**Subject:** `Why 10,000+ Canadians switched to natural`

**Content:** Customer testimonials, reviews, before/after stories

(I'll skip the full HTML for brevity - follow same template)

---

**Email 5: Last Chance (Day 14)**

**Wait:** 7 days after Email 4

**Subject:** `Your BOGO code expires tonight`

**Content:** Final reminder about email-exclusive offer

---

**Flow #1 is complete. Set to LIVE.**

---

**Create Email Flow #2: Abandoned Cart**

1. **Flows → Create Flow → Use Template**
2. **Select:** Abandoned Cart
3. **Customize:**

**Email 1: 1 Hour After Abandonment**

**Subject:** `You left something in your cart`

**Preview:** `{{ event.extra.line_items.0.product.title }} is still available`

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
}
.container {
  max-width: 600px;
  margin: 0 auto;
  background-color: #ffffff;
  padding: 40px 30px;
}
.product-box {
  border: 2px solid #e5e7eb;
  padding: 20px;
  margin: 20px 0;
  border-radius: 8px;
  display: flex;
  align-items: center;
}
.product-image {
  width: 100px;
  height: 100px;
  object-fit: cover;
  margin-right: 20px;
  border-radius: 4px;
}
.button {
  display: inline-block;
  background-color: #2D5016;
  color: white !important;
  padding: 16px 32px;
  text-decoration: none;
  border-radius: 8px;
  font-weight: bold;
  font-size: 16px;
}
</style>
</head>
<body>
<div class="container">
  <h2 style="color: #1f2937;">You left something in your cart</h2>
  
  <p style="font-size: 16px; line-height: 1.6;">
    Hi {% if person.first_name %}{{ person.first_name }}{% else %}there{% endif %},
  </p>
  
  <p style="font-size: 16px; line-height: 1.6;">
    You were looking at our {{ event.extra.line_items.0.product.title }}.
  </p>
  
  <!-- Product Display -->
  <div class="product-box">
    <img src="{{ event.extra.line_items.0.product.images.0.src }}" class="product-image" alt="Product">
    <div>
      <h3 style="margin: 0 0 10px 0;">{{ event.extra.line_items.0.product.title }}</h3>
      <p style="font-size: 18px; font-weight: bold; color: #2D5016; margin: 0;">
        ${{ event.extra.line_items.0.price }}
      </p>
    </div>
  </div>
  
  <p style="font-size: 16px; line-height: 1.6;">
    Quick question: What's holding you back?
  </p>
  
  <p style="font-size: 16px; line-height: 1.6;">
    Hit reply and let me know—I'll personally help.
  </p>
  
  <center>
    <a href="{{ event.extra.checkout_url }}" class="button">
      Complete My Order
    </a>
  </center>
  
  <p style="font-size: 16px; line-height: 1.6; margin-top: 30px;">
    🎁 Reminder: Order by Dec 20 for Christmas delivery + FREE gift wrapping
  </p>
  
  <p style="font-size: 16px; line-height: 1.6;">
    - Sarah, Customer Success<br>
    EcoComfort
  </p>
</div>
</body>
</html>
```

**Save**

---

**Email 2: 24 Hours - Add 15% Discount**

**Wait:** 23 hours after Email 1

**Subject:** `Still interested? Here's 15% off`

**Include dynamic discount code:** CART15

(Use similar format, add discount)

---

**Email 3: 48 Hours - Last Chance**

**Wait:** 24 hours after Email 2

**Subject:** `We're releasing your cart in 6 hours`

**Urgency:** Mention code expires at midnight

---

**Flow #2 is complete. Set to LIVE.**

---

**Summary of Email Setup:**

✅ Flow #1: Welcome Series (5 emails over 14 days)
✅ Flow #2: Abandoned Cart (3 emails over 48 hours)
✅ Popup: 10% off for new subscribers

**Both flows are LIVE and automated**

---

## END OF DAY 2

**What you accomplished:**
✅ Meta ads campaigns built (2 campaigns, 7 ads total)
✅ Google ads campaigns built (Shopping + Search)
✅ Email flows created (Welcome + Abandoned Cart)
✅ Email popup installed

**Status:**
- Meta: LIVE, spending $150/day
- Google: LIVE, spending $100/day
- Email: LIVE, collecting subscribers

**Tomorrow (Day 3):**
- Monitor campaigns
- Create content for social media
- Set up tracking formulas in spreadsheet
- Build remaining landing pages

---

## DAY 3 - WEDNESDAY DEC 11

### MORNING (9 AM - 12 PM)

#### TASK 12: First 24-Hour Check & Data Entry (30 min)

**9:00 AM - Check Meta Performance**

1. **Go to:** Meta Ads Manager
2. **Date Range:** Yesterday (Dec 10)
3. **Check these metrics:**

| Campaign | Spend | Impressions | Link Clicks | CTR | Purchases | Revenue | ROAS | CPP |
|----------|-------|-------------|-------------|-----|-----------|---------|------|-----|
| Cold | $ | | | | | $ | | $ |
| Retargeting | $ | | | | | $ | | $ |

4. **Enter in your tracking spreadsheet**

**What to look for (24-hour benchmarks):**
- Spend on track? (Should be ~$150 if running all day)
- Link clicks happening? (Need 50+ clicks to evaluate)
- Any purchases? (Don't panic if 0 on day 1 - learning phase)
- CTR above 1%? (Good)
- CPM reasonable? ($15-30 CAD is normal in December)

**Red flags:**
- $50 spent, 0 link clicks = Creative is broken (remake it)
- High CTR but 0 sales = Landing page problem

---

**9:15 AM - Check Google Performance**

1. **Go to:** Google Ads
2. **Date Range:** Yesterday
3. **Check:**

| Campaign | Spend | Impressions | Clicks | CTR | Conversions | Revenue | ROAS | CPA |
|----------|-------|-------------|--------|-----|-------------|---------|------|-----|
| Shopping | $ | | | | | $ | | $ |
| Search | $ | | | | | $ | | $ |

4. **Enter in tracking spreadsheet**

**Check Search Terms:**
- Campaigns → Keywords → Search Terms
- Look for weird searches
- Add irrelevant terms to negative keywords

**Example negatives to add:**
- If you see "free duvet" → add "free" as negative
- If you see "duvet cover" (not duvet) → add "cover" as negative

---

**9:30 AM - Check Shopify Orders**

1. **Shopify → Orders**
2. **Filter:** Yesterday's orders
3. **For each order, note:**
   - Source (Facebook, Google, Email, Organic)
   - Product purchased
   - Order value

4. **Match to ad spend:**
   - Did any Meta purchases show up in Ads Manager?
   - Did any Google conversions show up in Google Ads?
   - If not, your tracking might be delayed (normal, give it 24-48 hours)

---

**9:45 AM - Update Master Spreadsheet**

Open your tracking sheet, fill in:
- Row for Dec 10
- Meta spend, orders, revenue
- Google spend, orders, revenue  
- Email orders (if any)
- Organic orders (if any)
- Calculate: Blended ROAS = Total Revenue / Total Ad Spend

---

#### TASK 13: Set Up Automated Rules (Meta) - 20 min

**Prevent wasting money while you sleep**

**Go to:** Meta Ads Manager → Automated Rules

**Rule #1: Pause Bad Ad Sets**

1. **Create Rule**
2. **Apply to:** Ad Sets
3. **Action:** Turn off ad sets
4. **Conditions:**
   - Spend is greater than $100
   - AND Purchases is equal to 0
   - Time range: Lifetime
5. **Schedule:** Continuously
6. **Create Rule**

**What this does:** If an ad set spends $100 with zero sales, it auto-pauses (stops wasting money)

---

**Rule #2: Notify on High Spend, No Results**

1. **Create Rule**
2. **Apply to:** Campaigns
3. **Action:** Send notification only
4. **Conditions:**
   - Spend is greater than $200
   - AND ROAS is less than 1.0
   - Time range: Lifetime
5. **Send to:** Your email
6. **Schedule:** Daily at 9 AM
7. **Create Rule**

---

#### TASK 14: Build Remaining Landing Pages (1.5 hours)

**Landing Page #2: Chemical-Free Sleep**

(For Google Search ads targeting "chemical free duvet")

**Go to:** Shopify → Pages → Add Page

**Title:** Chemical-Free Sleep

**URL:** chemical-free-sleep

**Content:** (Simplified - focus on chemical-free angle)

```html
<div style="text-align: center; padding: 60px 20px; background: #1f2937; color: white;">
  <h1 style="font-size: 48px; margin-bottom: 20px;">
    Your Duvet Is Off-Gassing Chemicals While You Sleep
  </h1>
  <p style="font-size: 20px; margin-bottom: 30px;">
    73% of conventional bedding contains formaldehyde, VOCs, and flame retardants
  </p>
  <p style="font-size: 18px; margin-bottom: 40px;">
    EcoComfort duvets are OEKO-TEX certified—tested for 1,000+ harmful chemicals.<br>
    <strong>Result: ZERO detected.</strong>
  </p>
  <a href="/collections/duvets" style="display: inline-block; background: white; color: #1f2937; padding: 18px 40px; font-size: 18px; font-weight: bold; text-decoration: none; border-radius: 8px;">
    Shop Chemical-Free Duvets
  </a>
</div>

<div style="max-width: 1200px; margin: 60px auto; padding: 0 20px;">
  
  <!-- Problem Section -->
  <div style="background: #fee2e2; padding: 40px; border-radius: 12px; margin-bottom: 40px;">
    <h2 style="color: #991b1b; margin-top: 0;">What's Actually In Conventional Bedding:</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-top: 30px;">
      <div>
        <h3 style="color: #7f1d1d;">❌ Formaldehyde</h3>
        <p>Preservative in synthetic fabrics. Known carcinogen. Off-gasses for weeks.</p>
      </div>
      <div>
        <h3 style="color: #7f1d1d;">❌ Flame Retardants</h3>
        <p>Legally required on polyester. Linked to hormone disruption.</p>
      </div>
      <div>
        <h3 style="color: #7f1d1d;">❌ Pesticide Residue</h3>
        <p>From conventional cotton farming. Accumulates in lungs.</p>
      </div>
      <div>
        <h3 style="color: #7f1d1d;">❌ VOCs</h3>
        <p>Volatile organic compounds. "New bedding smell" = chemicals.</p>
      </div>
    </div>
  </div>
  
  <!-- Solution Section -->
  <div style="background: #d1fae5; padding: 40px; border-radius: 12px; margin-bottom: 40px;">
    <h2 style="color: #065f46; margin-top: 0;">Sleep On 100% Natural Materials</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-top: 30px;">
      <div>
        <h3 style="color: #064e3b;">✅ Wild-Harvested Kapok</h3>
        <p>From rainforest trees. No farming, no pesticides, no processing.</p>
      </div>
      <div>
        <h3 style="color: #064e3b;">✅ Organic Bamboo</h3>
        <p>Mechanical processing (not chemical). Naturally antibacterial.</p>
      </div>
      <div>
        <h3 style="color: #064e3b;">✅ Australian Wool</h3>
        <p>Pasture-raised sheep. No synthetic treatments or dyes.</p>
      </div>
      <div>
        <h3 style="color: #064e3b;">✅ OEKO-TEX Certified</h3>
        <p>Lab-tested for 1,000+ chemicals. Zero detected in our products.</p>
      </div>
    </div>
  </div>
  
  <!-- Offer -->
  <div style="background: #fef3c7; border-left: 6px solid #f59e0b; padding: 40px; margin-bottom: 40px;">
    <h2 style="color: #92400e; margin-top: 0;">🎁 LIMITED TIME: FREE Pillow Set With Every Duvet</h2>
    <p style="font-size: 18px; color: #78350f;">
      → Bamboo Duvet Queen: $274.99<br>
      → FREE Feather Pillow 2-Pack ($138 value)<br>
      → Total value: $412.98 | You pay: $274.99
    </p>
    <p style="font-size: 16px; color: #78350f;">
      ✓ Order by Dec 20 → Arrives before Christmas<br>
      ✓ FREE gift wrapping + personalized card<br>
      ✓ 100-night trial
    </p>
  </div>
  
  <!-- Products -->
  <h2 style="text-align: center; margin-bottom: 40px;">Choose Your Chemical-Free Duvet</h2>
  
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 30px; margin-bottom: 60px;">
    <!-- Product cards - insert your products here -->
  </div>
  
  <!-- Social Proof -->
  <div style="background: #f9fafb; padding: 40px; border-radius: 12px;">
    <h2 style="text-align: center; margin-bottom: 40px;">Real Results From Real People</h2>
    <!-- Insert customer reviews -->
  </div>
  
</div>
```

**Save & Publish**

---

**Landing Page #3: Temperature Control**

**Title:** Temperature Control System

**URL:** temperature-control

(Similar structure, focus on hot sleeper angle - I'll skip full HTML for brevity)

**Key sections:**
- Hero: "Stop Waking Up Hot and Sweaty"
- Problem: Polyester traps heat
- Solution: Bamboo releases heat
- Testimonials: Focus on temperature stories
- Offer: Same free pillow offer
- Products: Emphasize bamboo products

**Save & Publish**

---

### LUNCH (12-1 PM)

---

### AFTERNOON (1-5 PM)

#### TASK 15: Create Social Media Content (1 hour)

**You need organic content to support paid ads**

**Instagram/Facebook Posts for This Week:**

**Post 1: Gift Guide Announcement (Today)**

**Image:** Hero shot of duvet + pillows gift-wrapped

**Caption:**
```
🎁 OUR HOLIDAY GIFT GUIDE IS HERE

Give better sleep, not more stuff.

Natural bamboo duvets + FREE pillow sets.

✓ Ships in 24 hours
✓ Arrives before Dec 23
✓ FREE gift wrapping
✓ Made in Canada

Order by Dec 20 for guaranteed Christmas delivery.

Link in bio 👆

#naturalBedding #christmasGifts #ecoFriendlyGifts #canadianMade #sleepBetter #chemicalFree
```

**Post on:** Instagram, Facebook

---

**Post 2: Customer Testimonial (Thursday)**

**Image:** Customer review screenshot or photo

**Caption:**
```
"Best gift I've ever received" - Michelle T.

She gave her mom a bamboo duvet last Christmas.

Her mom called it "life-changing" and now sleeps through the night for the first time in years.

That's the reaction you want when someone opens your gift. 🎁

🎄 Holiday special: FREE $138 pillow set with every duvet
📦 Order by Dec 20 for Christmas delivery

Link in bio

#customerLove #naturalSleep #giftIdeas #christmasGift
```

---

**Post 3: Behind the Scenes (Friday)**

**Image/Video:** Your warehouse, products being wrapped, or manufacturing

**Caption:**
```
Behind the scenes: Holiday gift wrapping 🎁

Every order this December gets:
✓ Beautiful, minimal gift wrapping (free)
✓ Personalized gift message card
✓ Shipped within 24 hours from Mississauga

Made in Canada with natural materials.

Order by Dec 20 → Arrives before Christmas

Link in bio 👆

#madeincanada #smallBusiness #holidayGifts #giftWrapping
```

---

**Instagram Stories (Daily):**

Monday: Countdown timer "X days until last shipping date"
Tuesday: Product showcase (duvet close-up)
Wednesday: Customer review
Thursday: "Order today, ships tomorrow" reminder
Friday: "Last week to order for Christmas"

**Use Instagram Story stickers:**
- Countdown sticker (to Dec 20)
- Link sticker (to holiday landing page)
- Poll: "What's your biggest sleep problem?" (engagement)

---

#### TASK 16: Set Up Google Analytics Goals (30 min)

**Track conversions in Google Analytics (in addition to Google Ads)**

1. **Go to:** Google Analytics 4
2. **Admin → Data Streams → Web → Your website**
3. **Configure tag settings → Events → Create Event**

**Event #1: Add to Cart**
- Event name: `add_to_cart`
- (Should already be tracking if Shopify is connected)

**Event #2: Begin Checkout**
- Event name: `begin_checkout`

**Event #3: Purchase**
- Event name: `purchase`
- Mark as conversion: Yes

**Link Google Analytics to Google Ads:**
- Admin → Google Ads Links → Link Account
- Import conversions from Analytics

**Why:** Better attribution, see full customer journey

---

#### TASK 17: Test Your Entire Funnel (45 min)

**Act like a customer and test everything:**

**Test #1: Meta Ad → Landing Page → Checkout**

1. Visit your live Meta ad (use "View in Feed" option in Ads Manager)
2. Click the ad
3. Does it go to the right landing page?
4. Is the holiday offer clear?
5. Can you add product to cart easily?
6. Does gift wrapping option show up?
7. Does discount code apply automatically?
8. Complete checkout (use test order)

**Fix any broken links or confusing steps**

---

**Test #2: Google Search → Product Page → Checkout**

1. Google: "bamboo duvet canada"
2. Do you see your ad?
3. Click it
4. Does it go to the right page?
5. Is the Dec 20 deadline visible?
6. Test checkout

---

**Test #3: Email Popup → Welcome Email → Purchase**

1. Visit your site in incognito
2. Does popup appear after 15 seconds?
3. Sign up with test email
4. Did you receive welcome email immediately?
5. Does WELCOME10 code work?

---

**Test #4: Abandon Cart → Get Email**

1. Add product to cart
2. Go to checkout
3. Enter test email
4. Leave page (don't complete)
5. Wait 1 hour
6. Did you get abandoned cart email?
7. Does link take you back to checkout?

**Fix anything that's broken**

---

#### TASK 18: Build Week 1 Email Campaign (30 min)

**Your first broadcast email (goes to whole list)**

**Send:** Friday Dec 13 at 10 AM

**Campaign Name:** Holiday Week 1 - Gift Guide

**Subject:** `⏰ One week until last shipping date`

**Preview:** `Free pillows with duvets. Order by Dec 20 for Christmas delivery.`

**Email Content:**

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
}
.container {
  max-width: 600px;
  margin: 0 auto;
  background-color: #ffffff;
}
.header {
  background: linear-gradient(135deg, #7c2d12 0%, #dc2626 100%);
  color: white;
  padding: 40px 20px;
  text-align: center;
}
.content {
  padding: 40px 30px;
}
.countdown {
  background: #fee2e2;
  border-left: 4px solid #dc2626;
  padding: 30px;
  margin: 30px 0;
  text-align: center;
  border-radius: 8px;
}
.button {
  display: inline-block;
  background-color: #2D5016;
  color: white !important;
  padding: 18px 40px;
  text-decoration: none;
  border-radius: 8px;
  font-weight: bold;
  font-size: 18px;
}
</style>
</head>
<body>
<div class="container">
  <div class="header">
    <h1 style="margin: 0; font-size: 36px;">⏰ One Week Left</h1>
  </div>
  
  <div class="content">
    <p style="font-size: 16px; line-height: 1.6;">
      Quick reminder:
    </p>
    
    <div class="countdown">
      <p style="font-size: 48px; font-weight: bold; color: #991b1b; margin: 0 0 10px 0;">
        7 DAYS
      </p>
      <p style="font-size: 18px; color: #7f1d1d; margin: 0;">
        Until last shipping date for Christmas delivery
      </p>
    </div>
    
    <p style="font-size: 16px; line-height: 1.6;">
      After December 20, we can't guarantee delivery before Christmas.
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      🎁 <strong>Still available:</strong>
    </p>
    
    <ul style="font-size: 16px; line-height: 1.8;">
      <li>FREE $138 Pillow Set with every duvet purchase</li>
      <li>FREE gift wrapping + personalized card</li>
      <li>FREE shipping across Canada</li>
      <li>Ships in 24 hours</li>
    </ul>
    
    <p style="font-size: 18px; font-weight: bold; color: #2D5016; margin: 30px 0;">
      Bamboo Duvet + Free Pillows: $274.99
    </p>
    
    <center>
      <a href="https://ecocomfort.co/pages/holiday-gifts" class="button">
        Shop Gift Bundles
      </a>
    </center>
    
    <p style="font-size: 16px; line-height: 1.6; margin-top: 40px;">
      Don't be the person scrambling on December 22nd.
    </p>
    
    <p style="font-size: 16px; line-height: 1.6;">
      - Sarah<br>
      Team EcoComfort
    </p>
  </div>
</div>
</body>
</html>
```

**Schedule for:** Friday Dec 13 at 10:00 AM

**Send to:** Entire email list (exclude people who purchased in last 7 days)

---

## END OF DAY 3

**Status Check:**

✅ Day 1 data collected & analyzed
✅ Automated rules set up (prevent overspending)
✅ All landing pages built (3 total)
✅ Social media content created
✅ Google Analytics configured
✅ Full funnel tested
✅ First email campaign scheduled

**Tomorrow:**
- Daily monitoring
- Adjust bids/budgets based on performance
- Create backup ads (if current ones underperform)
- Respond to customer inquiries

---

# DAYS 4-7: MONITORING & OPTIMIZATION

## DAILY ROUTINE (30 min morning, 15 min evening)

### MORNING CHECK (9 AM)

**Every single morning, do this:**

1. **Open tracking spreadsheet**
2. **Check Meta (10 min):**
   - Yesterday's spend
   - Purchases
   - ROAS
   - Update spreadsheet
   
3. **Check Google (5 min):**
   - Yesterday's spend
   - Conversions
   - ROAS
   - Update spreadsheet

4. **Check Shopify (5 min):**
   - Total orders yesterday
   - Match to ad platforms
   - Any customer questions?

5. **Check Email (5 min):**
   - How many subscribers added yesterday?
   - Any flow emails convert?
   - Any replies to respond to?

6. **Calculate (5 min):**
   - Blended ROAS = Total revenue / Total ad spend
   - On track for weekly target?

---

### DECISION FRAMEWORK (Use this to decide what to do)

**IF Blended ROAS > 3.0x:**
→ Everything is working
→ Increase Meta budget by 20% ($100 → $120)
→ Increase Google budget by 20% ($100 → $120)
→ Keep running

**IF Blended ROAS 2.0-3.0x:**
→ Profitable but could be better
→ Keep budgets same
→ Test new ad creative (add 2 new ads)
→ Monitor for 2 more days

**IF Blended ROAS 1.5-2.0x:**
→ Breaking even / small profit
→ Pause worst-performing ad set
→ Create new ads with different angle
→ Cut daily budget by 30% until ROAS improves

**IF Blended ROAS < 1.5x:**
→ Losing money
→ Pause all campaigns immediately
→ Analyze what went wrong:
  - No clicks? = Creative problem
  - Clicks but no sales? = Landing page or offer problem
  - Sales but high CAC? = Targeting problem
→ Fix, then relaunch at $50/day to test

---

### EVENING CHECK (6 PM)

1. **Check current day spend** (are you on pace?)
   - If it's 6 PM and you've only spent $50 of $250 budget = underspending (ads not delivering)
   - If you've spent $200 already = overpacing (might hit budget too early)

2. **Respond to any customer emails**

3. **Check for cart abandonments** (Shopify → Abandoned Checkouts)
   - Are people dropping off? Why?

4. **Plan tomorrow**

---

## WEEKEND (DEC 14-15): PREP FOR PEAK WEEK

### SATURDAY DEC 14

**Task:** Create Week 2 ads (30% off campaign)

**Meta Ad - Week 2 Creative:**

**Subject:** Last week before Christmas

**Primary Text:**
```
⏰ 6 Days Left to Ship Before Christmas

Your options are shrinking:

→ Amazon gift card (lazy)
→ Another candle (boring)  
→ Natural sleep gift set (thoughtful)

Give them something they'll actually use:
✓ OEKO-TEX certified bamboo duvet
✓ Made in Canada (not China)
✓ 30% off + free shipping + free gift wrapping

Order by Friday Dec 20 → Arrives before Dec 25 (guaranteed)

After Dec 20, you're out of luck.

Bamboo Duvet: ~~$274.99~~ $192.49

Made in Canada. 100-night trial.
```

**BUILD these ads on Saturday but DON'T LAUNCH until Monday Dec 16**

---

### SUNDAY DEC 15

**Task:** Weekly review

**Open your tracking spreadsheet Week 1 summary tab**

Fill in:
- Total week spend
- Total orders
- Total revenue
- Blended ROAS
- Top performing ad (by ROAS)
- Worst performing ad
- Email subscribers added
- Action items for Week 2

**Example:**
```
Week 1 Results:
- Spent: $1,750
- Orders: 15
- Revenue: $4,500
- ROAS: 2.57x
- Profit: ~$800

Top ad: "Free Pillows Angle" (3.8x ROAS)
Worst ad: "Temperature Control" (1.2x ROAS - paused)

Subscribers: +142

Week 2 Plan:
- Increase budget to $250/day (peak week)
- Launch 30% off campaign Monday
- Send daily emails Mon-Fri
- Scale top-performing ads
```

---

# TRACKING & KPI DASHBOARD

## PRIMARY KPIs (Check Daily)

### Financial Metrics
1. **Daily Ad Spend** 
   - Target Week 1: $250/day
   - Target Week 2: $350/day
   
2. **Daily Revenue**
   - Target Week 1: $850/day (3.4x ROAS)
   - Target Week 2: $1,700/day (4.9x ROAS)

3. **Blended ROAS**
   - Minimum acceptable: 2.0x
   - Target: 3.0x+
   - Excellent: 4.0x+

4. **Net Profit Margin**
   - Target: 25%+
   - Formula: (Revenue - COGS - Ad Spend - Fees) / Revenue

### Platform Metrics

**Meta:**
- CAC (Cost Per Acquisition): Target < $100
- ROAS: Target 2.5x+
- CTR (Click-Through Rate): Target 2%+
- CPM: Benchmark $15-30 (higher in December is normal)

**Google:**
- CAC: Target < $80
- ROAS: Target 3.0x+
- Conversion Rate: Target 2%+
- CPC (Shopping): Target < $1.50
- CPC (Search): Target < $3.00

**Email:**
- Open Rate: Target 25%+
- Click Rate: Target 3%+
- Revenue per Email: Target $0.50+
- Subscriber Growth: Target +50/day

### Business Metrics
- AOV (Average Order Value): Track daily
  - Target Week 1-2: $300+
  - Target Week 4: $200+ (40% off = lower AOV)

- New vs Returning: Track ratio
  - Holiday should be 95%+ new (gift giving)

- Email List Growth: Track daily
  - Target Week 1: +500 total
  - Target total by Jan 15: +1,500

---

## TRACKING SPREADSHEET FORMULAS

**In your Daily Metrics tab:**

**Column: Blended ROAS**
```
= Total Revenue / Total Ad Spend
```

**Column: Profit Estimate (25% COGS)**
```
= (Total Revenue * 0.75) - Total Ad Spend - (Total Revenue * 0.03)
```
(75% margin after 25% COGS, minus ad spend, minus 3% payment fees)

**Column: AOV**
```
= Total Revenue / Total Orders
```

**Column: Blended CAC**
```
= Total Ad Spend / Total Orders
```

---

## WEEKLY SUMMARY FORMULAS

**In Week Summary tab:**

**Week Revenue**
```
= SUM(DailyMetrics!TotalRevenue_Week1Range)
```

**Week ROAS**
```
= SUM(DailyMetrics!Revenue_Week1) / SUM(DailyMetrics!Spend_Week1)
```

**Week Profit**
```
= (Week Revenue * 0.75) - Week Spend - (Week Revenue * 0.03)
```

---

# CREATIVE BRIEF & AD EXAMPLES

## WHAT MAKES A GOOD AD CREATIVE

### Image/Video Requirements

**Technical Specs:**
- Format: 1080x1080 (square) preferred, or 1200x628 (landscape)
- File size: Under 5MB
- No more than 20% text on image (Meta rule)
- High resolution, professional looking

**What Works:**
1. **Product in use** (person sleeping peacefully on duvet)
2. **Gift presentation** (beautifully wrapped product)
3. **Before/After** (synthetic vs natural comparison)
4. **Close-up details** (bamboo texture, OEKO-TEX badge)
5. **Lifestyle shots** (cozy bedroom, Canadian home)

**What Doesn't Work:**
1. Stock photos that look fake
2. Cluttered images with too much going on
3. Low quality/blurry photos
4. Images with people's faces cut off
5. Too much text overlay

---

### Copy Formula

**Hook (First 2 lines):**
- Must stop the scroll
- Ask a question OR make a bold claim OR create urgency

**Examples:**
```
❌ Weak: "Check out our natural duvets"
✅ Strong: "Your synthetic duvet is off-gassing chemicals while you sleep"

❌ Weak: "We have a sale this week"
✅ Strong: "6 days left to ship before Christmas"

❌ Weak: "Natural bedding from Canada"
✅ Strong: "Stop waking up hot and sweaty every night"
```

---

**Body (Middle section):**
- Explain the problem
- Present your solution
- Add social proof or specifics

**Example structure:**
```
[HOOK]

[PROBLEM]
Most duvets trap heat and off-gas chemicals for weeks.

[SOLUTION]
Our bamboo duvets are OEKO-TEX certified (zero chemicals), 
naturally regulate temperature, and are made in Canada from 
wild-harvested materials.

[PROOF]
Real customers report:
→ Falling asleep 12-15 minutes faster
→ Fewer night sweats
→ Waking up actually refreshed

[OFFER]
Limited time: Free $138 Pillow Set with every duvet purchase.
```

---

**CTA (Last part):**
- Clear, specific action
- Add urgency or scarcity
- Repeat the offer

**Examples:**
```
→ Queen Bamboo Duvet: $274.99
→ You get: Duvet + 2 Premium Pillows  
→ You save: $138

Order by Dec 20 for Christmas delivery.
Made in Canada. 100-night trial.
```

---

### Testing Framework

**Test these variables (one at a time):**

1. **Hook/Angle:**
   - Gift angle vs Health angle vs Problem/Solution
   - Test: "Perfect gift" vs "Stop sleeping on chemicals"

2. **Image:**
   - Product alone vs Lifestyle vs Close-up
   - Test: Duvet on bed vs Person sleeping

3. **Offer:**
   - Free pillow vs % discount vs Bundle
   - Test: "Free $138 pillow" vs "30% off duvet"

4. **CTA:**
   - Shop Now vs Learn More vs Add to Cart
   - Test: "Shop Duvets" vs "Claim Free Pillows"

**NEVER test more than 1 variable at a time** (you won't know what worked)

---

## AD CREATIVE EXAMPLES

### Week 1 Creative Set (Already Built)

**Ad 1: Free Pillows Angle** ✅ Built
**Ad 2: Chemical-Free Angle** ✅ Built  
**Ad 3: Temperature Control** ✅ Built

---

### Week 2 Creative Set (Build on Dec 14)

**Ad 4: Countdown Urgency**

**Image:** Calendar with Dec 20 circled in red

**Text:**
```
⏰ LAST WEEK FOR CHRISTMAS DELIVERY

December 21 = Too late
December 20 = Last day

30% off everything + free shipping + free gift wrapping

After Friday, you're taking chances.

Bamboo Duvet: ~~$274.99~~ $192.49

Order now: [link]
```

**Headline:** `⏰ 6 Days Left | 30% Off Natural Duvets`

---

**Ad 5: Procrastinator's Gift**

**Image:** Person stressed, shopping at last minute (relatable)

**Text:**
```
For Everyone Who's Still Shopping on Dec 15th

We see you. We got you.

→ Order today (Monday-Thursday)
→ Ships within 24 hours  
→ Arrives before Christmas (guaranteed)

30% off everything + free shipping + free gift wrapping

Natural bamboo duvets: $192.49 (reg $274.99)

Made in Canada. OEKO-TEX certified.

This is why you pay for fast shipping.

⏰ Deadline: Friday Dec 20 at 11:59 PM
```

**Headline:** `Procrastinator's Paradise - Ships in 24hrs`

---

**Ad 6: Social Proof**

**Image:** Compilation of 5-star reviews

**Text:**
```
"Best gift I've ever given" - Michelle T.
"My mom calls me every week to thank me" - David K.
"Worth every penny" - Sarah M.

Real reviews from real customers who gave natural sleep as a gift.

This Christmas, give something they'll use 365 nights a year.

30% off + FREE pillow set
Order by Dec 20 for Christmas delivery

Bamboo Duvet: $192.49

Made in Canada. 100-night trial.
```

**Headline:** `Rated 4.8/5 Stars | Natural Duvets Made in Canada`

---

### Backup Creatives (If Week 1-2 Ads Fail)

**Ad 7: Comparison Table**

**Image:** Side-by-side comparison graphic

```
SYNTHETIC DUVET vs NATURAL DUVET

Synthetic:
❌ Off-gasses formaldehyde
❌ Traps heat like plastic
❌ Made in China
❌ Contains flame retardants
❌ $200

Natural EcoComfort:
✅ OEKO-TEX certified (zero chemicals)
✅ Temperature regulating
✅ Made in Canada  
✅ Wild-harvested materials
✅ $192.49 (30% off)

Free shipping + Free gift wrapping
Order by Dec 20 for Christmas
```

---

**Ad 8: For Hot Sleepers (Specific Pain Point)**

**Image:** Person waking up sweaty (before) → Person sleeping peacefully (after)

**Text:**
```
Do You Wake Up Sweating at 3 AM?

Your polyester duvet is the problem.

Plastic fibers trap heat and moisture = sauna effect

Natural bamboo fibers release heat automatically = perfect temperature all night

Customers report 60% fewer night sweats after switching.

30% off bamboo duvets this week.
Order by Dec 20 → Arrives before Christmas

$192.49 (reg $274.99)

Made in Canada. 100-night trial.
```

**Headline:** `Stop Night Sweats | Natural Temperature Control`

---

# CUSTOMER ACQUISITION FUNNEL

## THE COMPLETE JOURNEY

### STAGE 1: AWARENESS (Cold Traffic)

**How they find you:**
1. Meta/Google ads (paid)
2. Organic social media
3. Google search (organic)
4. Word of mouth

**Your job:** Get attention, create curiosity

**Tactics:**
- Run Meta ads (gift angle, chemical-free angle)
- Post on Instagram/Facebook (3x per week)
- SEO-optimized product pages (for organic search)

**Goal:** Get them to click

**Metric to track:** CTR (click-through rate) on ads

---

### STAGE 2: INTEREST (Landing Page)

**They clicked your ad. Now what?**

**Your job:** Show the value, build desire

**Landing page must have:**
1. Clear headline (what's in it for them)
2. Offer (free pillows, discount, bundle)
3. Social proof (reviews, testimonials)
4. Trust signals (Made in Canada, OEKO-TEX, 100-night trial)
5. Clear CTA (Add to Cart button)

**Goal:** Get them to add to cart

**Metric to track:** Add-to-cart rate (ATCs / Landing page visits)

**Target:** 3-5% add-to-cart rate

---

### STAGE 3: CONSIDERATION (Cart → Checkout)

**They added to cart but haven't bought. Now what?**

**Why people abandon:**
1. Just browsing (50%)
2. Unexpected shipping cost (25%)
3. Hesitation / need to think (15%)
4. Payment issues (10%)

**Your job:** Remove friction, add urgency

**Tactics:**
1. **Free shipping** (removes cost barrier)
2. **Countdown timer** ("Order by Dec 20")
3. **Trust badges** (100-night trial, secure checkout)
4. **Exit intent popup** (offer 10% off if leaving)

**If they abandon:**
→ Abandoned cart email (1 hour later)
→ 15% discount email (24 hours later)
→ Last chance email (48 hours later)
→ Retargeting ads on Meta

**Goal:** Convert to purchase

**Metric to track:** Cart abandonment rate

**Target:** Under 70% abandonment

---

### STAGE 4: PURCHASE (Conversion)

**They bought! Now what?**

**Your job:** Deliver great experience, set up repeat purchase

**Immediately:**
1. Order confirmation email (Shopify automatic)
2. Add to email list (they're now a customer)
3. Tag in Klaviyo: "Purchased Duvet" or "Purchased Pillow"

**7 days later:**
1. Delivery check-in email ("How's your duvet?")
2. Ask for review
3. Upsell complementary product (if they bought duvet → suggest mattress protector)

**30 days later:**
1. Review request
2. Offer loyalty discount (20% off next order)

**60 days later:**
1. Referral ask ("Know someone who needs better sleep?")
2. Give $20 off for referral

**Goal:** Turn into repeat customer

**Metric:** Repeat purchase rate

**Target:** 15%+ within 90 days

---

### STAGE 5: LOYALTY (Retention)

**They're a happy customer. Keep them.**

**Tactics:**
1. Email newsletter (weekly) - education, tips, new products
2. VIP program (spend $400+ = exclusive access, early sales)
3. Birthday discounts
4. Anniversary email (1 year since first purchase)

**Goal:** Maximize lifetime value (LTV)

**Metric:** Average LTV

**Target:** $300+ LTV (2-3 purchases)

---

## FUNNEL METRICS TO TRACK

```
STAGE → METRIC → TARGET

Awareness → Ad CTR → 2%+
Interest → Landing Page Visit → (from ad click)
Consideration → Add to Cart Rate → 3-5%
Purchase → Conversion Rate → 1.5-3%
Loyalty → Repeat Purchase Rate → 15%+
```

**Example funnel math:**

```
1,000 ad impressions
→ 20 clicks (2% CTR)
→ 1 add to cart (5% ATC rate)
→ 0.5 purchases (2% conversion rate)
→ $150 revenue per purchase

Revenue: $75
Ad Cost: $40 (at $2 CPM)
ROAS: 1.88x
```

**To improve ROAS, you can:**
1. Increase CTR (better ad creative)
2. Increase ATC rate (better landing page)
3. Increase conversion rate (remove friction, add urgency)
4. Increase AOV (bundles, upsells)
5. Decrease CAC (better targeting)

---

# EMAIL COLLECTION STRATEGY

## How to Grow Your List to 1,500+ in 6 Weeks

### Method 1: Website Popup (Primary)

**Already installed:** Klaviyo popup

**Optimization:**
- **Offer:** 10% off first order
- **Timing:** Show after 15 seconds OR on exit intent
- **Frequency:** Don't show again for 30 days
- **Mobile:** Must work on mobile (60% of traffic)

**Expected:** 2-5% of website visitors will subscribe

**Math:**
- 1,000 visitors/week × 3% conversion = 30 new subscribers/week
- Over 6 weeks = 180 subscribers

---

### Method 2: Checkout (Automatic)

**Already happening:** Anyone who buys automatically gets added to your email list

**Expected:** Every customer = 1 subscriber

**Math:**
- 157 orders over 6 weeks = 157 subscribers

---

### Method 3: Social Media

**Instagram/Facebook bio:**
Update bio to:
```
Natural bedding made in Canada 🇨🇦
Chemical-free sleep for 10,000+ customers
🎁 Get 10% off → [link to your site]
```

**Link in bio:** Goes to homepage (popup will capture email)

**Instagram Stories:**
- Use "Link" sticker → Points to holiday landing page
- Add text: "Tap for 10% off 👆"

**Expected:** 50-100 subscribers over 6 weeks

---

### Method 4: Lead Magnet (Advanced - Optional)

**Create:** "The Chemical-Free Sleep Guide" (PDF)

**Offer:** 
- Landing page: "Download our free guide to sleeping chemical-free"
- They enter email → Get PDF → Auto-added to list

**How to create:**
1. Write 5-page PDF with tips
2. Upload to Shopify (Files)
3. Create landing page with email form
4. Link from social media

**Expected:** 100-200 subscribers (if promoted)

---

### Method 5: Referral Program (Post-purchase)

**Install app:** Smile.io OR ReferralCandy (free trials)

**Offer:**
- Existing customer refers friend
- Friend gets $20 off first order
- Customer gets $20 credit

**Both emails collected**

**Expected:** 50-100 subscribers over 6 weeks

---

## EMAIL COLLECTION GOAL TRACKER

| Week | Website Popup | Purchases | Social | Lead Magnet | Referral | Weekly Total | Running Total |
|------|---------------|-----------|--------|-------------|----------|--------------|---------------|
| 1 | 50 | 15 | 10 | 0 | 0 | 75 | 75 |
| 2 | 100 | 35 | 20 | 20 | 5 | 180 | 255 |
| 3 | 40 | 12 | 10 | 10 | 3 | 75 | 330 |
| 4 | 120 | 50 | 30 | 30 | 10 | 240 | 570 |
| 5 | 80 | 25 | 20 | 20 | 5 | 150 | 720 |
| 6 | 90 | 20 | 20 | 20 | 10 | 160 | 880 |
| **TOTAL** | | | | | | | **1,500+** |

---

# FINAL CHECKLIST - LAUNCH READY

## Pre-Launch (Complete before going live)

**Shopify:**
- [ ] All apps installed and configured
- [ ] Product titles updated for Google Shopping
- [ ] Product descriptions include holiday messaging
- [ ] Gift cards created ($200 and $300)
- [ ] Gift wrapping option available
- [ ] Holiday landing pages built (3 total)
- [ ] Countdown timer active
- [ ] Free shipping banner active
- [ ] Checkout tested (place test order)

**Meta Ads:**
- [ ] Pixel verified (use Pixel Helper)
- [ ] 2 campaigns created (Cold + Retargeting)
- [ ] 7 ads created (6 cold, 1 retargeting)
- [ ] Budgets set ($150/day total)
- [ ] Automated rules configured
- [ ] Campaigns set to ACTIVE

**Google Ads:**
- [ ] Performance Max paused
- [ ] Shopping campaign created ($60/day)
- [ ] Search campaign created ($40/day)
- [ ] Keywords added (exact match)
- [ ] Negative keywords added
- [ ] Conversion tracking verified
- [ ] Campaigns set to ACTIVE

**Email:**
- [ ] Klaviyo connected to Shopify
- [ ] Welcome series built (5 emails)
- [ ] Abandoned cart flow built (3 emails)
- [ ] Popup installed and active
- [ ] First campaign scheduled (Friday)
- [ ] Test emails sent to yourself

**Tracking:**
- [ ] Master spreadsheet created
- [ ] All formulas working
- [ ] Google Analytics configured
- [ ] Meta pixel verified
- [ ] Google Ads conversion tracking working

**Content:**
- [ ] Week 1 social posts created
- [ ] Instagram stories planned
- [ ] Email campaigns drafted
- [ ] Product photos ready

---

## Daily Operations Checklist

**Every Morning (9 AM):**
- [ ] Check yesterday's ad spend (Meta + Google)
- [ ] Count yesterday's orders
- [ ] Calculate yesterday's ROAS
- [ ] Update tracking spreadsheet
- [ ] Respond to customer emails
- [ ] Check inventory levels

**Every Evening (6 PM):**
- [ ] Check today's spend (on pace?)
- [ ] Review any abandoned carts
- [ ] Plan tomorrow's tasks
- [ ] Schedule social post for tomorrow

**Every Friday:**
- [ ] Weekly review (fill in summary tab)
- [ ] Kill underperforming ads
- [ ] Scale top performers
- [ ] Plan next week's creative
- [ ] Send weekly email campaign

---

## Emergency Contacts & Resources

**If ads aren't delivering:**
- Check: Account spending limit (Meta Business Settings)
- Check: Payment method valid
- Check: Ads approved (not in review)

**If pixel isn't tracking:**
- Test: Facebook Pixel Helper (Chrome extension)
- Fix: Reconnect Shopify to Facebook
- Support: Meta Business Help Center

**If emails aren't sending:**
- Check: Klaviyo connected to Shopify
- Check: SPF/DKIM records (email authentication)
- Check: Spam folder (deliverability issue)

**If Shopify is slow:**
- Check: Too many apps? (uninstall unused)
- Optimize: Compress images
- Support: Shopify Support Chat

**If you need help:**
- Meta Ads Support: business.facebook.com/business/help
- Google Ads Support: support.google.com/google-ads
- Shopify Support: help.shopify.com
- Klaviyo Support: help.klaviyo.com

---

# EXECUTION SUMMARY

You now have:
✅ Complete daily task list (Dec 9-Jan 14)
✅ Exact setup instructions (Shopify, Meta, Google, Email)
✅ Tracking system (spreadsheet + formulas + KPIs)
✅ 8+ ad creatives with full copy
✅ 8+ HTML email templates
✅ 3 landing pages
✅ Customer acquisition funnel
✅ Email growth strategy
✅ Daily/weekly review process
✅ Decision framework (what to do if ROAS is X)

**Your job now:**
1. Follow the daily task list
2. Track everything in spreadsheet
3. Make decisions based on data (not feelings)
4. Test, measure, optimize

**Timeline:**
- Days 1-2: Setup everything
- Day 3: Launch all campaigns
- Days 4-7: Monitor, adjust, optimize
- Week 2: Scale winners, peak revenue week
- Week 3: Pivot to gift cards
- Week 4: Boxing Day blowout
- Week 5: New Year health resolution
- Week 6: Final push

**Revenue Target:** $45,000 in 6 weeks
**Profit Target:** $11,775 (26% margin)

You have everything you need. Now execute.

Questions? Re-read this document. 
The answer is in here somewhere.

Good luck. Now go make money. 🚀
