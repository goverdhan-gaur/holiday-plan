# Abandoned Cart - Email 3: Last Chance (48 Hours)

**Flow:** Abandoned Cart
**Email #:** 3 of 3
**Trigger:** 24 hours after Email 2 (48 hours total after abandonment)
**Subject Line:** Your 15% discount expires in 6 hours
**Preview Text:** Last chance to save on your order (cart releasing soon)

---

## Email HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Last Chance</title>
</head>
<body style="margin: 0; padding: 0; font-family: 'Helvetica Neue', Arial, sans-serif; background-color: #f8fafc;">

  <table width="100%" cellpadding="0" cellspacing="0" style="background-color: #f8fafc;">
    <tr>
      <td align="center" style="padding: 40px 20px;">

        <!-- Main Container -->
        <table width="600" cellpadding="0" cellspacing="0" style="background-color: #ffffff; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">

          <!-- Header -->
          <tr>
            <td style="background: linear-gradient(135deg, #7f1d1d 0%, #991b1b 100%); padding: 40px 30px; text-align: center; border-radius: 8px 8px 0 0;">
              <h1 style="margin: 0; color: #ffffff; font-size: 38px; font-weight: 700;">⏰ Final Call</h1>
              <p style="margin: 15px 0 0 0; color: #fca5a5; font-size: 20px; font-weight: 600;">Your 15% discount expires in 6 hours</p>
            </td>
          </tr>

          <!-- Body Content -->
          <tr>
            <td style="padding: 40px 30px;">

              <p style="font-size: 18px; line-height: 1.6; color: #1f2937; margin-top: 0;">
                This is the last reminder.
              </p>

              <p style="font-size: 18px; line-height: 1.6; color: #1f2937;">
                Your <strong>CART15</strong> discount code expires in <strong>6 hours</strong>. After that, we'll release your cart and the 15% discount will no longer be available.
              </p>

              <!-- Urgency Countdown Box -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0; background: linear-gradient(135deg, #7f1d1d 0%, #991b1b 100%); border-radius: 12px; padding: 40px; text-align: center; color: #ffffff; box-shadow: 0 8px 20px rgba(127, 29, 29, 0.4);">
                <tr>
                  <td>
                    <div style="font-size: 64px; font-weight: 700; margin-bottom: 10px; text-shadow: 0 2px 8px rgba(0,0,0,0.3);">6</div>
                    <div style="font-size: 24px; font-weight: 600; margin-bottom: 15px;">HOURS LEFT</div>
                    <div style="font-size: 16px; opacity: 0.9; line-height: 1.4;">
                      Until CART15 expires<br>
                      and your cart is released
                    </div>
                  </td>
                </tr>
              </table>

              <p style="font-size: 20px; line-height: 1.6; color: #1f2937; text-align: center; font-weight: 600;">
                We can't hold inventory forever—and this is your last chance to save 15%.
              </p>

              <!-- CTA Button -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0;">
                <tr>
                  <td align="center">
                    <a href="{{ event.extra.checkout_url }}?discount=CART15" style="display: inline-block; background-color: #dc2626; color: #ffffff; text-decoration: none; padding: 22px 55px; border-radius: 8px; font-size: 24px; font-weight: 700; box-shadow: 0 8px 20px rgba(220, 38, 38, 0.5); text-transform: uppercase;">Complete Order Now</a>
                    <p style="margin: 15px 0 0 0; font-size: 16px; color: #dc2626; font-weight: 600;">CART15 auto-applied • Expires in 6 hours</p>
                  </td>
                </tr>
              </table>

              <!-- What You're About to Lose -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 50px 0; background-color: #fef2f2; border: 3px solid #dc2626; padding: 30px; border-radius: 8px;">
                <tr>
                  <td>
                    <h3 style="margin: 0 0 25px 0; font-size: 24px; color: #991b1b; text-align: center;">What You're About to Lose:</h3>

                    <table width="100%" cellpadding="0" cellspacing="0" style="margin-bottom: 20px;">
                      <tr>
                        <td style="padding: 15px 0; border-bottom: 2px solid #fecaca;">
                          <span style="font-size: 18px; color: #7f1d1d; font-weight: 600;">❌ 15% OFF (CART15)</span>
                        </td>
                        <td style="padding: 15px 0; text-align: right; border-bottom: 2px solid #fecaca;">
                          <span style="font-size: 18px; color: #dc2626; font-weight: 700;">-${{ event.extra.subtotal_price | times: 0.15 | money }}</span>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 15px 0; border-bottom: 2px solid #fecaca;">
                          <span style="font-size: 18px; color: #7f1d1d; font-weight: 600;">❌ Your Saved Cart</span>
                        </td>
                        <td style="padding: 15px 0; text-align: right; border-bottom: 2px solid #fecaca;">
                          <span style="font-size: 18px; color: #dc2626; font-weight: 700;">Released</span>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 15px 0;">
                          <span style="font-size: 18px; color: #7f1d1d; font-weight: 600;">❌ Guaranteed Stock</span>
                        </td>
                        <td style="padding: 15px 0; text-align: right;">
                          <span style="font-size: 18px; color: #dc2626; font-weight: 700;">No Longer Reserved</span>
                        </td>
                      </tr>
                    </table>

                    <p style="margin: 25px 0 0 0; font-size: 16px; color: #991b1b; text-align: center; line-height: 1.6;">
                      After 6 hours, you'll need to start over—and pay full price.
                    </p>
                  </td>
                </tr>
              </table>

              <!-- Quick Reminders -->
              <h3 style="font-size: 22px; color: #1f2937; margin: 50px 0 25px 0; text-align: center;">Quick Reminders:</h3>

              <table width="100%" cellpadding="0" cellspacing="0">
                <tr>
                  <td width="50%" style="padding: 10px;">
                    <table width="100%" style="background-color: #ecfdf5; border-radius: 8px; padding: 20px; text-align: center; height: 100%;">
                      <tr>
                        <td>
                          <div style="font-size: 40px; margin-bottom: 10px;">✓</div>
                          <p style="margin: 0; font-size: 16px; color: #065f46; font-weight: 600; line-height: 1.4;">100-Night Risk-Free Trial</p>
                        </td>
                      </tr>
                    </table>
                  </td>
                  <td width="50%" style="padding: 10px;">
                    <table width="100%" style="background-color: #eff6ff; border-radius: 8px; padding: 20px; text-align: center; height: 100%;">
                      <tr>
                        <td>
                          <div style="font-size: 40px; margin-bottom: 10px;">🚚</div>
                          <p style="margin: 0; font-size: 16px; color: #1e40af; font-weight: 600; line-height: 1.4;">Free Shipping + Ships in 24 Hours</p>
                        </td>
                      </tr>
                    </table>
                  </td>
                </tr>
                <tr>
                  <td width="50%" style="padding: 10px;">
                    <table width="100%" style="background-color: #fef3c7; border-radius: 8px; padding: 20px; text-align: center; height: 100%;">
                      <tr>
                        <td>
                          <div style="font-size: 40px; margin-bottom: 10px;">🇨🇦</div>
                          <p style="margin: 0; font-size: 16px; color: #92400e; font-weight: 600; line-height: 1.4;">Made in Canada (OEKO-TEX Certified)</p>
                        </td>
                      </tr>
                    </table>
                  </td>
                  <td width="50%" style="padding: 10px;">
                    <table width="100%" style="background-color: #fce7f3; border-radius: 8px; padding: 20px; text-align: center; height: 100%;">
                      <tr>
                        <td>
                          <div style="font-size: 40px; margin-bottom: 10px;">★</div>
                          <p style="margin: 0; font-size: 16px; color: #9f1239; font-weight: 600; line-height: 1.4;">4.8/5 Stars (2,847 Reviews)</p>
                        </td>
                      </tr>
                    </table>
                  </td>
                </tr>
              </table>

              <!-- Customer Testimonial -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0; background-color: #f0fdf4; border-left: 4px solid #10b981; padding: 25px; border-radius: 6px;">
                <tr>
                  <td>
                    <div style="margin-bottom: 10px; color: #fbbf24; font-size: 20px;">★★★★★</div>
                    <p style="margin: 0 0 15px 0; font-size: 16px; line-height: 1.6; color: #047857; font-style: italic;">
                      "I almost didn't buy it because I was overthinking the price. Then I used the cart discount code and just went for it. Best. Decision. Ever. I sleep so much better now—and my night sweats are completely gone."
                    </p>
                    <p style="margin: 0; font-size: 14px; color: #059669;">
                      <strong>— Michael D.</strong>, Toronto
                    </p>
                  </td>
                </tr>
              </table>

              <!-- Second CTA -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0;">
                <tr>
                  <td align="center">
                    <p style="margin: 0 0 20px 0; font-size: 22px; color: #1f2937; font-weight: 700;">This is your last chance.</p>
                    <a href="{{ event.extra.checkout_url }}?discount=CART15" style="display: inline-block; background-color: #dc2626; color: #ffffff; text-decoration: none; padding: 20px 50px; border-radius: 8px; font-size: 22px; font-weight: 700; box-shadow: 0 6px 16px rgba(220, 38, 38, 0.5);">Claim 15% Off Before It's Gone</a>
                  </td>
                </tr>
              </table>

              <!-- Final Note -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0; background-color: #fffbeb; border-radius: 8px; padding: 25px;">
                <tr>
                  <td style="text-align: center;">
                    <p style="margin: 0 0 10px 0; font-size: 18px; color: #92400e; font-weight: 600;">Questions? We're Here to Help</p>
                    <p style="margin: 0; font-size: 16px; line-height: 1.6; color: #78350f;">
                      Reply to this email and we'll respond within 2 hours.<br>
                      <span style="font-size: 14px;">Real humans, real answers—no bots!</span>
                    </p>
                  </td>
                </tr>
              </table>

              <!-- Signature -->
              <p style="font-size: 16px; line-height: 1.6; color: #4b5563; margin-top: 50px;">
                Last call—don't miss out,<br>
                <strong style="color: #1f2937;">Sarah & The EcoComfort Team</strong>
              </p>

              <p style="font-size: 14px; color: #9ca3af; margin-top: 10px;">
                P.S. This is the final email about your cart. After 6 hours, CART15 expires and we'll release your items back to inventory. If you want natural, chemical-free bedding at 15% off, now is the time.
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
2. **Previous Email:** Email 2 (15% Discount)
3. **Wait Time:** 24 hours after Email 2 (48 hours total after abandonment)
4. **Filter:** Only if checkout still not completed
5. **From Name:** Sarah - EcoComfort
6. **From Email:** hello@ecocomfort.co
7. **Reply To:** hello@ecocomfort.co
8. **Subject:** Your 15% discount expires in 6 hours
9. **Preview Text:** Last chance to save on your order (cart releasing soon)

## Important Notes

- This is the **final email** in the abandoned cart sequence
- Make the urgency clear without being pushy
- After this email, stop sending cart reminders (don't annoy customers)
- Consider adding these customers to a "Browse Abandonment" or general email list

## Klaviyo Variables Used

- `{{ event.extra.checkout_url }}` - Link back to checkout
- `{{ event.extra.subtotal_price }}` - Cart total for discount calculation

## Variables to Update

- Replace `https://ecocomfort.co` with your actual domain
- Adjust the "6 hours" timeline if needed (some brands use 12 or 24 hours)
- Add `{{unsubscribe_link}}` variable in footer

## A/B Test Ideas

- **Subject Line A:** Your 15% discount expires in 6 hours
- **Subject Line B:** Final call: Your cart is being released
- **Subject Line C:** ⏰ LAST CHANCE: 15% off expires tonight

## What Happens Next?

After this email:
1. If customer purchases → Move to Post-Purchase flow
2. If customer doesn't purchase → Stop cart emails, consider:
   - Adding to "Browse Abandonment" flow
   - Adding to general newsletter list
   - Retargeting with ads
