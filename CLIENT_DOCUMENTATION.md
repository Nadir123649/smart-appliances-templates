# 📄 Smart Appliance Services — Client Template Suite Guide & Maintenance Documentation

Welcome to the official **HTML Email Template Suite Guide** for **Smart Appliance Services**. This document provides a complete overview of all four production-ready email templates, step-by-step instructions on how to easily edit text, headlines, offers, links, and images, and how to deploy them into your Email Service Provider (ESP) such as Mailchimp, Klaviyo, HubSpot, or SendGrid.

---

## 📌 Executive Summary & Confirmed Template Suite

Each template in this suite has been built according to your confirmed directions, using modern responsive email standards, high-converting design patterns, and cross-client compatibility.

| Template File | Confirmed Direction | Campaign Use Case | Primary CTA & Offer |
| :--- | :--- | :--- | :--- |
| [`index.html`](file:///d:/Projects%20Company/smart-appliances-templates/index.html) | **Base Template** | Post-Service Follow-up & Quick Check-In | `Schedule Appointment →` |
| [`template-2-maintenance.html`](file:///d:/Projects%20Company/smart-appliances-templates/template-2-maintenance.html) | **Template 2 – V1** | Annual Tune-Up & Seasonal Savings | `Claim Your Savings ($89 Diagnostic Credit)` |
| [`template-3-review-request.html`](file:///d:/Projects%20Company/smart-appliances-templates/template-3-review-request.html) | **Template 3 – V2** | Same-Day Service Dispatch & Urgent Openings | `Claim Your Slot Online ($25 OFF Code: FAST25)` |
| [`template-4-warranty.html`](file:///d:/Projects%20Company/smart-appliances-templates/template-4-warranty.html) | **Template 4 – V2 (Clean & Focused)** | Targeted Appliance Specialist & Symptom Care | `Book [Appliance] Repair ($30 OFF Code: CARE30)` |

---

## 🎨 Design & Email Compatibility Standards

All 4 templates are engineered with the following production standards:

- **📄 100% Editable HTML Text**: Headlines, body copy, pricing, offer codes, phone numbers, and CTA button labels are pure HTML text (never embedded inside images), allowing quick edits in any text editor or ESP visual builder.
- **📱 Responsive Breakpoint**: Optimized for all screens (`< 599px`) with automatic column stacking and touch-friendly CTA buttons.
- **✉️ Outlook (MSO) 96 DPI Ready**: Features Microsoft Office conditional comments (`mso`) and XML namespaces (`xmlns:v`, `xmlns:o`) to prevent image stretching or table breaking in desktop Outlook (2016–365).
- **📬 Preheader Snippet Protection**: Every template includes a hidden preheader div with zero-width joiner (`&zwnj;`) spacers so inbox snippet previews display compelling text instead of raw URLs or footer copy.
- **🛡️ Format Detection Shield**: Prevents iOS Apple Mail from turning phone numbers and dates into unwanted blue links.
- **🎨 Brand Typography Stack**: Headers use [`Afacad`](https://fonts.google.com/specimen/Afacad), body text uses [`Manrope`](https://fonts.google.com/specimen/Manrope), with bulletproof fallback to `Arial, sans-serif`.

---

## ✍️ Step-by-Step Guide: How to Edit & Update Content (No Coding Required)

### 1. Editing Headlines & Subheadings
All headlines are wrapped in standard `<h1>`, `<h2>`, or `<h3>` HTML tags. Simply open the file in any code editor (or ESP visual editor) and change the text inside the tags:

```html
<!-- Example in index.html -->
<h1 style="margin: 0; font-family: 'Afacad', Arial, sans-serif; font-size: 26px; font-weight: 700; color: #123A64;">
  How is your [appliance] doing, [first_name]?
</h1>
```
*To edit*: Change `How is your [appliance] doing, [first_name]?` to your desired heading.

---

### 2. Updating Body Paragraph Text
Body copy is wrapped in `<p>` tags. You can add, edit, or shorten any sentence directly:

```html
<!-- Example in template-3-review-request.html -->
<p style="margin: 0 0 14px 0; font-family: 'Manrope', Arial, sans-serif; font-size: 14px; color: #3A4B5B;">
  Need your refrigerator, washer, dryer, or oven repaired fast? Our certified local technicians are in <strong>[City]</strong> today and tomorrow.
</p>
```

---

### 3. Changing CTA Button Text & Landing Page Links
To change the button text or the landing page URL:
1. Locate the `<a>` link tag inside the button table.
2. Update the `href="..."` URL to your preferred booking page.
3. Edit the text between `<a>` and `</a>`.

```html
<!-- Example Button HTML -->
<a href="https://smartapplianceservices.com/booking" target="_blank" style="...">
  SCHEDULE YOUR REPAIR &rarr;
</a>
```

---

### 4. Updating Phone Numbers & Click-to-Call Links
Search for `tel:7272757555` across any template. Update both the `href="tel:..."` link and the visible phone number string:

```html
<!-- Example Click-to-Call HTML -->
Prefer to call? <a href="tel:7272757555" style="..."> (727) 275-7555 </a>
```

---

### 5. Modifying Prices, Discount Offers & Promo Codes
All prices and discount codes are pure HTML text so you can adjust them for seasonal campaigns anytime:

- **Template 2 ($89 Diagnostic Credit)**: Search for `$89` or `CLAIM YOUR SAVINGS` around line 390.
- **Template 3 ($25 OFF / FAST25)**: Search for `FAST25` or `$25 OFF` around line 285.
- **Template 4 ($30 OFF / CARE30)**: Search for `CARE30` or `$30 OFF` around line 378.

```html
<!-- Example Offer Code HTML in Template 3 -->
<span style="font-family: 'Afacad', Arial, sans-serif; font-size: 15px; font-weight: 700; color: #123A64;">
  🎁 <span style="color: #B45309;">$25 OFF</span> Your Same-Day Repair Service
</span>
<span style="font-family: 'Manrope', Arial, sans-serif; font-size: 12px; color: #78350F;">
  Mention code <strong style="color: #123A64;">FAST25</strong> when booking online or by phone.
</span>
```

---

### 6. Updating Testimonials & Reviews
In `index.html`, the customer review quote and reviewer name can be edited directly inside the quote block:

```html
<!-- Reviewer Name & Location -->
<p style="font-family: 'Afacad', Arial, sans-serif; font-size: 15px; font-weight: 700; color: #123A64;">
  Lori DeFelice <span style="font-weight: 500; color: #64748B;">&middot; Saint Petersburg, FL</span>
</p>

<!-- Customer Review Text -->
<p style="font-family: 'Manrope', Arial, sans-serif; font-size: 13px; color: #334155;">
  &ldquo;Dennis from Smart Appliance arrived right on time for our refrigerator repair...&rdquo;
</p>
```

---

### 7. Swapping Placeholder Images with Real Business Photos
All graphics are hosted on Cloudinary for reliable delivery:
- **Header Dark Logo**: `https://res.cloudinary.com/qi6tz0xr/image/upload/v1790145483/23634436.png`
- **Footer Light Logo**: `https://res.cloudinary.com/qi6tz0xr/image/upload/v1790145490/9823597823.png`
- **5-Star Rating Badge**: `https://res.cloudinary.com/qi6tz0xr/image/upload/v1790145536/Stars.png`

*When ready to replace placeholder graphics with real business photos (e.g. technicians working, vans, kitchen scenes)*:
Upload your photo to your CDN/ESP image manager and replace the `src="..."` link in the `<img>` tag:
```html
<img src="https://your-domain.com/your-technician-photo.jpg" width="140" height="auto" alt="Technician Service" style="display: block; width: 100%; height: auto; border: 0;" />
```

---

## 🔄 Dynamic CRM Personalization Tags Reference

The templates use standardized brackets `[...]` for dynamic personalization tags. When uploading into your CRM or ESP, you can leave these tags as-is or replace them with your platform's specific merge tags:

| Placeholder Tag | Description | Example ESP Merge Tag (Mailchimp) | Example ESP Merge Tag (Klaviyo) |
| :--- | :--- | :--- | :--- |
| `[first_name]` | Customer's first name | `*|FNAME|*` | `{{ first_name\|default:'there' }}` |
| `[appliance]` | Serviced appliance (e.g. Refrigerator) | `*|APPLIANCE|*` | `{{ event.Appliance\|default:'appliance' }}` |
| `[City]` / `[city]` | Customer's city / service location | `*|CITY|*` | `{{ person.city\|default:'your area' }}` |
| `[City/Month]` | Location & service month | `*|CITY_MONTH|*` | `{{ event.CityMonth }}` |

---

## 📥 ESP / CRM Deployment Guide

### For Mailchimp:
1. Go to **Campaigns** → **Email Templates** → **Create Template** → **Code your own** → **Paste in HTML**.
2. Copy the entire content of the target template file (`index.html`, `template-2-maintenance.html`, `template-3-review-request.html`, or `template-4-warranty.html`).
3. Paste into Mailchimp's HTML editor and save.

### For Klaviyo:
1. Go to **Email Templates** → **Create Template** → **Import HTML**.
2. Upload the desired `.html` file or paste the raw code directly.
3. Ensure preview tags match Klaviyo's syntax (`{{ first_name }}`).

### For HubSpot / ActiveCampaign / SendGrid:
1. Select **Custom HTML** when creating an email draft or template.
2. Paste the template code and replace merge variables if needed.

---

## 🎯 Template 4 Focus & Clean Design Notes

As requested by Alex:
> *"For Template 4, I like the V2 structure, just keep it fairly clean and focused so it doesn’t become too busy."*

**Key Highlights of Template 4 (V2 Clean & Focused)**:
1. **Dynamic Segment Header**: Clean location badge `Serving [City, FL]` in header.
2. **Specialist Hero Block**: Highlighted headline (`Expert service for your [Refrigerator]`) with concise, 2-sentence intro copy.
3. **3-Symptom Diagnostic Grid**: Clean, balanced icons for *Temperature Issues*, *Unusual Noises*, and *Water Leaks*.
4. **Focused Promo Banner**: Single high-contrast Navy Card highlighting `$30 OFF Any [Appliance] Repair` (Code `CARE30`) with direct action buttons.
5. **Universal Trust Footer**: Sleek checkmarks for 1-Year Warranty, Factory-Trained Techs, and 4.9★ Rating.

---

## 📞 Support & Walkthrough Assistance

If you or your team need a live walkthrough of the template files or assistance integrating them into your ESP, please feel free to reach out anytime!

*Made with ❤️ for Smart Appliance Services.*
