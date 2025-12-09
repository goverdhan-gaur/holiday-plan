# Abandoned Cart - Email 2: 15% Discount Incentive (24 Hours)

**Flow:** Abandoned Cart
**Email #:** 2 of 3
**Trigger:** 23 hours after Email 1 (24 hours total after abandonment)
**Subject Line:** Still interested? Here's 15% off
**Preview Text:** Special discount just for you (better than 10%!)

---

## Email HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Here's 15% Off</title>
</head>
<body style="margin: 0; padding: 0; font-family: 'Helvetica Neue', Arial, sans-serif; background-color: #f8fafc;">

  <table width="100%" cellpadding="0" cellspacing="0" style="background-color: #f8fafc;">
    <tr>
      <td align="center" style="padding: 40px 20px;">

        <!-- Main Container -->
        <table width="600" cellpadding="0" cellspacing="0" style="background-color: #ffffff; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">

          <!-- Header -->
          <tr>
            <td style="background: linear-gradient(135deg, #7c2d12 0%, #ea580c 100%); padding: 40px 30px; text-align: center; border-radius: 8px 8px 0 0;">
              <h1 style="margin: 0; color: #ffffff; font-size: 36px; font-weight: 700;">Wait! Here's 15% Off 🎁</h1>
              <p style="margin: 15px 0 0 0; color: #fed7aa; font-size: 18px; font-weight: 500;">A special discount just for you</p>
            </td>
          </tr>

          <!-- Body Content -->
          <tr>
            <td style="padding: 40px 30px;">

              <p style="font-size: 18px; line-height: 1.6; color: #1f2937; margin-top: 0;">
                We noticed you didn't complete your order yesterday.
              </p>

              <p style="font-size: 18px; line-height: 1.6; color: #1f2937;">
                No pressure—but if price was holding you back, we'd like to help.
              </p>

              <!-- Discount Code Box -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0;">
                <tr>
                  <td style="background: linear-gradient(135deg, #dc2626 0%, #ef4444 100%); border-radius: 12px; padding: 35px; text-align: center; color: #ffffff; box-shadow: 0 8px 20px rgba(220, 38, 38, 0.3);">
                    <p style="margin: 0 0 10px 0; font-size: 18px; font-weight: 600; opacity: 0.9;">Your Exclusive Cart Rescue Code</p>
                    <p style="margin: 0; font-size: 42px; font-weight: 700; letter-spacing: 4px; text-shadow: 0 2px 4px rgba(0,0,0,0.2);">CART15</p>
                    <p style="margin: 15px 0 0 0; font-size: 20px; font-weight: 600;">15% OFF</p>
                    <p style="margin: 10px 0 0 0; font-size: 14px; opacity: 0.9;">Valid for 48 hours only</p>
                  </td>
                </tr>
              </table>

              <p style="font-size: 18px; line-height: 1.6; color: #1f2937; text-align: center;">
                <strong>This is better than the 10% welcome code</strong>—and it's only available for the next 48 hours.
              </p>

              <!-- CTA Button -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0;">
                <tr>
                  <td align="center">
                    <a href="{{ event.extra.checkout_url }}?discount=CART15" style="display: inline-block; background-color: #dc2626; color: #ffffff; text-decoration: none; padding: 20px 50px; border-radius: 8px; font-size: 22px; font-weight: 700; box-shadow: 0 6px 16px rgba(220, 38, 38, 0.5);">Apply Code & Checkout</a>
                    <p style="margin: 15px 0 0 0; font-size: 14px; color: #9ca3af;">Code auto-applied at checkout</p>
                  </td>
                </tr>
              </table>

              <!-- Savings Breakdown -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0; background-color: #fef2f2; border-radius: 8px; padding: 25px;">
                <tr>
                  <td>
                    <h3 style="margin: 0 0 20px 0; font-size: 22px; color: #991b1b; text-align: center;">Here's What You'll Save:</h3>

                    <table width="100%" cellpadding="0" cellspacing="0">
                      <tr>
                        <td style="padding: 10px 0; border-bottom: 1px solid #fecaca;">
                          <span style="font-size: 16px; color: #7f1d1d;">Cart Subtotal:</span>
                        </td>
                        <td style="padding: 10px 0; text-align: right; border-bottom: 1px solid #fecaca;">
                          <span style="font-size: 16px; color: #7f1d1d; font-weight: 600;">${{ event.extra.subtotal_price }}</span>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 10px 0; border-bottom: 1px solid #fecaca;">
                          <span style="font-size: 16px; color: #dc2626; font-weight: 600;">15% OFF (CART15):</span>
                        </td>
                        <td style="padding: 10px 0; text-align: right; border-bottom: 1px solid #fecaca;">
                          <span style="font-size: 16px; color: #dc2626; font-weight: 600;">-${{ event.extra.subtotal_price | times: 0.15 | money }}</span>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 15px 0 0 0;">
                          <span style="font-size: 20px; color: #991b1b; font-weight: 700;">Your New Total:</span>
                        </td>
                        <td style="padding: 15px 0 0 0; text-align: right;">
                          <span style="font-size: 24px; color: #991b1b; font-weight: 700;">${{ event.extra.subtotal_price | times: 0.85 | money }}</span>
                        </td>
                      </tr>
                    </table>

                    <p style="margin: 20px 0 0 0; font-size: 14px; color: #991b1b; text-align: center; font-style: italic;">
                      Plus free shipping = No hidden costs!
                    </p>
                  </td>
                </tr>
              </table>

              <!-- Why This Matters -->
              <h3 style="font-size: 22px; color: #1f2937; margin: 40px 0 20px 0; text-align: center;">Why People Love EcoComfort:</h3>

              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 20px 0;">
                <tr>
                  <td width="50%" style="padding: 10px;">
                    <table width="100%" style="background-color: #ecfdf5; border-radius: 8px; padding: 20px; height: 100%;">
                      <tr>
                        <td style="text-align: center;">
                          <div style="font-size: 36px; margin-bottom: 10px;">🌡️</div>
                          <p style="margin: 0; font-size: 16px; color: #065f46; font-weight: 600;">Temperature Control</p>
                          <p style="margin: 5px 0 0 0; font-size: 14px; color: #047857; line-height: 1.4;">"No more night sweats!"</p>
                        </td>
                      </tr>
                    </table>
                  </td>
                  <td width="50%" style="padding: 10px;">
                    <table width="100%" style="background-color: #eff6ff; border-radius: 8px; padding: 20px; height: 100%;">
                      <tr>
                        <td style="text-align: center;">
                          <div style="font-size: 36px; margin-bottom: 10px;">🚫</div>
                          <p style="margin: 0; font-size: 16px; color: #1e40af; font-weight: 600;">Zero Chemicals</p>
                          <p style="margin: 5px 0 0 0; font-size: 14px; color: #1e3a8a; line-height: 1.4;">OEKO-TEX certified safe</p>
                        </td>
                      </tr>
                    </table>
                  </td>
                </tr>
                <tr>
                  <td width="50%" style="padding: 10px;">
                    <table width="100%" style="background-color: #fef3c7; border-radius: 8px; padding: 20px; height: 100%;">
                      <tr>
                        <td style="text-align: center;">
                          <div style="font-size: 36px; margin-bottom: 10px;">🇨🇦</div>
                          <p style="margin: 0; font-size: 16px; color: #92400e; font-weight: 600;">Made in Canada</p>
                          <p style="margin: 5px 0 0 0; font-size: 14px; color: #78350f; line-height: 1.4;">Supporting local jobs</p>
                        </td>
                      </tr>
                    </table>
                  </td>
                  <td width="50%" style="padding: 10px;">
                    <table width="100%" style="background-color: #fce7f3; border-radius: 8px; padding: 20px; height: 100%;">
                      <tr>
                        <td style="text-align: center;">
                          <div style="font-size: 36px; margin-bottom: 10px;">✓</div>
                          <p style="margin: 0; font-size: 16px; color: #9f1239; font-weight: 600;">100-Night Trial</p>
                          <p style="margin: 5px 0 0 0; font-size: 14px; color: #881337; line-height: 1.4;">Risk-free guarantee</p>
                        </td>
                      </tr>
                    </table>
                  </td>
                </tr>
              </table>

              <!-- Urgency Box -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0; background-color: #fffbeb; border: 2px solid #f59e0b; padding: 25px; border-radius: 8px;">
                <tr>
                  <td style="text-align: center;">
                    <p style="margin: 0 0 10px 0; font-size: 20px; color: #92400e; font-weight: 700;">⏰ This Code Expires in 48 Hours</p>
                    <p style="margin: 0; font-size: 16px; line-height: 1.6; color: #78350f;">
                      CART15 is only valid until <strong>{{ 'now' | date: '%s' | plus: 172800 | date: '%B %d at %I:%M %p' }}</strong><br>
                      <span style="font-size: 14px;">After that, we can't guarantee this discount or stock availability.</span>
                    </p>
                  </td>
                </tr>
              </table>

              <!-- Second CTA -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0;">
                <tr>
                  <td align="center">
                    <a href="{{ event.extra.checkout_url }}?discount=CART15" style="display: inline-block; background-color: #dc2626; color: #ffffff; text-decoration: none; padding: 18px 45px; border-radius: 6px; font-size: 20px; font-weight: 700;">Claim My 15% Off Now</a>
                  </td>
                </tr>
              </table>

              <!-- Testimonial -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0; background-color: #f0fdf4; border-left: 4px solid #10b981; padding: 25px; border-radius: 6px;">
                <tr>
                  <td>
                    <div style="margin-bottom: 10px; color: #fbbf24; font-size: 20px;">★★★★★</div>
                    <p style="margin: 0 0 15px 0; font-size: 16px; line-height: 1.6; color: #047857; font-style: italic;">
                      "I was hesitant about the price, but then I used a discount code. Best decision ever. The bamboo duvet is incredible—I sleep so much better now. Wish I hadn't waited!"
                    </p>
                    <p style="margin: 0; font-size: 14px; color: #059669;">
                      <strong>— Rachel T.</strong>, Ottawa
                    </p>
                  </td>
                </tr>
              </table>

              <!-- Signature -->
              <p style="font-size: 16px; line-height: 1.6; color: #4b5563; margin-top: 40px;">
                We're here if you have any questions,<br>
                <strong style="color: #1f2937;">Sarah & The EcoComfort Team</strong>
              </p>

              <p style="font-size: 14px; color: #9ca3af; margin-top: 10px;">
                P.S. This is our best cart rescue offer. After 48 hours, it expires—and we won't be able to send it again. Don't miss out!
              </p>

            </td>
          </tr>

          <!-- Footer -->
          <tr>
            <td style="background-color: #f9fafb; padding: 30px; text-align: center; border-radius: 0 0 8px 8px;">
              <p style="margin: 0 0 10px 0; font-size: 14px; color: #6b7280;">
                EcoComfort Natural Bedding<br>
                Made in Canada 🇨🇦 | OEKO-TEX Certified
              </p>
              <p style="margin: 0; font-size: 12px; color: #9ca3af;">
                <a href="https://ecocomfort.co" style="color: #059669; text-decoration: none;">Visit Website</a> |
                <a href="{{unsubscribe_link}}" style="color: #9ca3af; text-decoration: none;">Unsubscribe</a>
              </p>
            </td>
          </tr>

        </table>

      </td>
    </tr>
  </table>

</body>
</html>
```

---

## Klaviyo Setup Instructions

1. **Flow:** Abandoned Cart
2. **Previous Email:** Email 1 (Cart Reminder)
3. **Wait Time:** 23 hours after Email 1 (24 hours total after abandonment)
4. **Filter:** Only if checkout still not completed
5. **From Name:** Sarah - EcoComfort
6. **From Email:** hello@ecocomfort.co
7. **Reply To:** hello@ecocomfort.co
8. **Subject:** Still interested? Here's 15% off
9. **Preview Text:** Special discount just for you (better than 10%!)

## Shopify Discount Code Setup

**Create this discount code in Shopify:**
- **Code:** CART15
- **Type:** Percentage
- **Value:** 15%
- **Applies to:** All products
- **Minimum requirements:** None
- **Customer eligibility:** All customers
- **Usage limits:** One per customer
- **Active dates:** Always active (no expiry in Shopify, but email says 48 hours)

## Klaviyo Variables Used

- `{{ event.extra.checkout_url }}` - Link back to checkout
- `{{ event.extra.subtotal_price }}` - Cart total
- Math operations for discount calculation

## Important Notes

- Make sure CART15 code is created in Shopify before sending
- The `?discount=CART15` parameter auto-applies the code at checkout
- Confirm the 48-hour expiry logic works with your setup

## Variables to Update

- Replace `https://ecocomfort.co` with your actual domain
- Adjust discount percentage if needed
- Add `{{unsubscribe_link}}` variable in footer

## A/B Test Ideas

- **Subject Line A:** Still interested? Here's 15% off
- **Subject Line B:** We'll give you 15% off (just this once)
- **Subject Line C:** Your cart + this code = 15% savings
