# Abandoned Cart - Email 1: Cart Reminder (1 Hour)

**Flow:** Abandoned Cart
**Email #:** 1 of 3
**Trigger:** 1 hour after cart abandonment
**Subject Line:** You left something in your cart
**Preview Text:** Your items are waiting (plus your 10% off code is still active!)

---

## Email HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>You Left Something Behind</title>
</head>
<body style="margin: 0; padding: 0; font-family: 'Helvetica Neue', Arial, sans-serif; background-color: #f8fafc;">

  <table width="100%" cellpadding="0" cellspacing="0" style="background-color: #f8fafc;">
    <tr>
      <td align="center" style="padding: 40px 20px;">

        <!-- Main Container -->
        <table width="600" cellpadding="0" cellspacing="0" style="background-color: #ffffff; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">

          <!-- Header -->
          <tr>
            <td style="background: linear-gradient(135deg, #065f46 0%, #047857 100%); padding: 40px 30px; text-align: center; border-radius: 8px 8px 0 0;">
              <h1 style="margin: 0; color: #ffffff; font-size: 32px; font-weight: 700;">You Left Something Behind</h1>
              <p style="margin: 15px 0 0 0; color: #d1fae5; font-size: 16px;">Your cart is waiting for you</p>
            </td>
          </tr>

          <!-- Body Content -->
          <tr>
            <td style="padding: 40px 30px;">

              <p style="font-size: 18px; line-height: 1.6; color: #1f2937; margin-top: 0;">
                Hi there! 👋
              </p>

              <p style="font-size: 18px; line-height: 1.6; color: #1f2937;">
                It looks like you started an order but didn't finish. No worries—we saved your cart for you!
              </p>

              <!-- Cart Items Section -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 30px 0; background-color: #f9fafb; border-radius: 8px; padding: 25px;">
                <tr>
                  <td>
                    <h3 style="margin: 0 0 20px 0; font-size: 20px; color: #1f2937; text-align: center;">Your Cart:</h3>

                    <!-- Dynamic cart items go here - Klaviyo variable -->
                    <div style="text-align: center; padding: 20px 0;">
                      {% for item in event.extra.line_items %}
                        <table width="100%" cellpadding="0" cellspacing="0" style="margin-bottom: 20px;">
                          <tr>
                            <td width="30%" style="padding-right: 15px;">
                              <img src="{{ item.product.images.0.src }}" alt="{{ item.product.title }}" style="width: 100%; max-width: 120px; border-radius: 6px; border: 1px solid #e5e7eb;">
                            </td>
                            <td width="70%" style="text-align: left; vertical-align: middle;">
                              <p style="margin: 0 0 5px 0; font-size: 16px; font-weight: 600; color: #1f2937;">{{ item.product.title }}</p>
                              <p style="margin: 0; font-size: 14px; color: #6b7280;">Quantity: {{ item.quantity }}</p>
                              <p style="margin: 10px 0 0 0; font-size: 18px; font-weight: 700; color: #047857;">${{ item.line_price }}</p>
                            </td>
                          </tr>
                        </table>
                      {% endfor %}
                    </div>

                    <!-- Total -->
                    <table width="100%" cellpadding="0" cellspacing="0" style="margin-top: 20px; padding-top: 20px; border-top: 2px solid #e5e7eb;">
                      <tr>
                        <td style="text-align: right; padding-right: 10px;">
                          <p style="margin: 0; font-size: 18px; color: #6b7280;">Subtotal:</p>
                        </td>
                        <td width="120" style="text-align: right;">
                          <p style="margin: 0; font-size: 22px; font-weight: 700; color: #1f2937;">${{ event.extra.subtotal_price }}</p>
                        </td>
                      </tr>
                    </table>
                  </td>
                </tr>
              </table>

              <!-- CTA Button -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0;">
                <tr>
                  <td align="center">
                    <a href="{{ event.extra.checkout_url }}" style="display: inline-block; background-color: #059669; color: #ffffff; text-decoration: none; padding: 18px 50px; border-radius: 6px; font-size: 20px; font-weight: 700; box-shadow: 0 4px 12px rgba(5, 150, 105, 0.4);">Complete My Order</a>
                  </td>
                </tr>
              </table>

              <!-- Reminder Section -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0; background-color: #fffbeb; border: 2px dashed #f59e0b; padding: 25px; border-radius: 8px;">
                <tr>
                  <td style="text-align: center;">
                    <p style="margin: 0 0 10px 0; font-size: 20px; color: #92400e; font-weight: 600;">💡 Don't Forget Your Discounts!</p>

                    <table width="100%" cellpadding="0" cellspacing="0" style="margin: 20px 0;">
                      <tr>
                        <td style="padding: 15px; background-color: #fef3c7; border-radius: 6px;">
                          <p style="margin: 0 0 5px 0; font-size: 16px; color: #78350f; font-weight: 600;">Option 1: Use your 10% code</p>
                          <p style="margin: 0; font-size: 24px; font-weight: 700; color: #92400e; letter-spacing: 2px;">WELCOME10</p>
                        </td>
                      </tr>
                    </table>

                    <p style="margin: 15px 0; font-size: 16px; color: #92400e;">— OR —</p>

                    <table width="100%" cellpadding="0" cellspacing="0">
                      <tr>
                        <td style="padding: 15px; background-color: #fef3c7; border-radius: 6px;">
                          <p style="margin: 0 0 5px 0; font-size: 16px; color: #78350f; font-weight: 600;">Option 2: Use BOGO (ends Jan 15)</p>
                          <p style="margin: 0; font-size: 14px; color: #78350f;">Buy 1 pillow/duvet/mattress, get 1 FREE</p>
                        </td>
                      </tr>
                    </table>

                    <p style="margin: 15px 0 0 0; font-size: 14px; color: #92400e; font-style: italic;">
                      (Can't combine, but we'll apply whichever saves you more!)
                    </p>
                  </td>
                </tr>
              </table>

              <!-- Why Buy Section -->
              <h3 style="font-size: 22px; color: #1f2937; margin: 40px 0 20px 0; text-align: center;">Why Complete Your Order?</h3>

              <table width="100%" cellpadding="0" cellspacing="0">
                <tr>
                  <td style="padding: 12px 0; border-bottom: 1px solid #e5e7eb;">
                    <span style="color: #10b981; font-size: 20px; margin-right: 10px;">✓</span>
                    <span style="font-size: 16px; color: #4b5563;"><strong>100-Night Trial</strong> – Try it risk-free</span>
                  </td>
                </tr>
                <tr>
                  <td style="padding: 12px 0; border-bottom: 1px solid #e5e7eb;">
                    <span style="color: #10b981; font-size: 20px; margin-right: 10px;">✓</span>
                    <span style="font-size: 16px; color: #4b5563;"><strong>Free Shipping</strong> – No extra costs</span>
                  </td>
                </tr>
                <tr>
                  <td style="padding: 12px 0; border-bottom: 1px solid #e5e7eb;">
                    <span style="color: #10b981; font-size: 20px; margin-right: 10px;">✓</span>
                    <span style="font-size: 16px; color: #4b5563;"><strong>Ships in 24 Hours</strong> – Fast delivery</span>
                  </td>
                </tr>
                <tr>
                  <td style="padding: 12px 0;">
                    <span style="color: #10b981; font-size: 20px; margin-right: 10px;">✓</span>
                    <span style="font-size: 16px; color: #4b5563;"><strong>OEKO-TEX Certified</strong> – Zero chemicals</span>
                  </td>
                </tr>
              </table>

              <!-- Second CTA -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0;">
                <tr>
                  <td align="center">
                    <a href="{{ event.extra.checkout_url }}" style="display: inline-block; background-color: #059669; color: #ffffff; text-decoration: none; padding: 16px 40px; border-radius: 6px; font-size: 18px; font-weight: 600;">Return to My Cart</a>
                  </td>
                </tr>
              </table>

              <!-- Questions Section -->
              <table width="100%" cellpadding="0" cellspacing="0" style="margin: 40px 0; background-color: #f0fdf4; border-radius: 8px; padding: 25px;">
                <tr>
                  <td style="text-align: center;">
                    <p style="margin: 0 0 10px 0; font-size: 18px; color: #065f46; font-weight: 600;">Have Questions?</p>
                    <p style="margin: 0; font-size: 16px; line-height: 1.6; color: #047857;">
                      Just reply to this email. We're real humans and we read every message!<br>
                      <span style="font-size: 14px;">Average response time: Under 2 hours</span>
                    </p>
                  </td>
                </tr>
              </table>

              <!-- Signature -->
              <p style="font-size: 16px; line-height: 1.6; color: #4b5563; margin-top: 40px;">
                Your cart is waiting,<br>
                <strong style="color: #1f2937;">Sarah & The EcoComfort Team</strong>
              </p>

              <p style="font-size: 14px; color: #9ca3af; margin-top: 10px;">
                P.S. We'll hold your cart for 48 hours. After that, we can't guarantee stock availability.
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
2. **Trigger:** Checkout Started
3. **Wait Time:** 1 hour after checkout started
4. **Filter:** Only if checkout not completed
5. **From Name:** Sarah - EcoComfort
6. **From Email:** hello@ecocomfort.co
7. **Reply To:** hello@ecocomfort.co
8. **Subject:** You left something in your cart
9. **Preview Text:** Your items are waiting (plus your 10% off code is still active!)

## Klaviyo Variables Used

- `{{ event.extra.checkout_url }}` - Link back to checkout
- `{{ event.extra.line_items }}` - Cart items
- `{{ event.extra.subtotal_price }}` - Cart total
- `{{ item.product.title }}` - Product name
- `{{ item.product.images.0.src }}` - Product image
- `{{ item.quantity }}` - Item quantity
- `{{ item.line_price }}` - Item price

## Important Notes

- Ensure Klaviyo is properly integrated with Shopify for cart data
- Test the dynamic cart item display before going live
- Make sure checkout URLs include UTM parameters for tracking

## Variables to Update

- Replace `https://ecocomfort.co` with your actual domain
- Update BOGO end date as needed
- Add `{{unsubscribe_link}}` variable in footer

## A/B Test Ideas

- **Subject Line A:** You left something in your cart
- **Subject Line B:** Did you forget something?
- **Subject Line C:** Your cart is waiting (plus 10% off!)
