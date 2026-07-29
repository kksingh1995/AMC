# Anshu Medicine Centre — Website

Live-ready static website for **Anshu Medicine Centre**, Phulwarisharif, Patna. Mobile-friendly, WhatsApp ordering, prescription upload, and full compliance pages (Privacy, Refund, T&C) — ready for RCS / WhatsApp Business API approval and Render deployment.

---

## 📁 Files in this folder

| File | Purpose |
|---|---|
| `index.html` | Main homepage (logo embedded inside — always displays) |
| `privacy-policy.html` | Privacy Policy (required by WhatsApp Business API) |
| `refund-policy.html` | Refund & Return Policy (required by WhatsApp Business API) |
| `terms-and-conditions.html` | Terms & Conditions (required by WhatsApp Business API) |
| `logo.png` | AMC logo with **transparent background** (for social sharing / OG image) |
| `logo-square.png` | Square logo (for social sharing / OG image) |
| `render.yaml` | Render deployment configuration |
| `README.md` | This file |

Zero build step. Zero dependencies. Pure static HTML.

> ✅ **Logo is embedded directly inside each HTML file** (base64), so it will *always* display — even if the JPEG files fail to upload or serve. This is bulletproof.

---

## 🏥 WhatsApp Business API / RCS Approval

Meta (WhatsApp) and RCS providers require **publicly accessible URLs** for these three legal pages when reviewing your business API application. After deployment, your policies will be at:

- `https://YOUR-SITE.onrender.com/privacy-policy.html`
- `https://YOUR-SITE.onrender.com/refund-policy.html`
- `https://YOUR-SITE.onrender.com/terms-and-conditions.html`

These URLs are exactly what you paste into the WhatsApp Business API / RCS application forms.

> ⚠️ **Important:** The policies included are professionally drafted templates covering the standard requirements for an Indian pharmacy business (Drugs and Cosmetics Act, IT Act 2000, DPDP Act 2023, Consumer Protection Act 2019). **We recommend having a lawyer review them once** before official submission to WhatsApp/Meta — this is standard practice for any business.

---

## 🚀 Deploy on Render

### GitHub deploy (recommended)

1. Create a GitHub repo (e.g. `anshu-medicine`).
2. Upload **all files** to the repo (including the 3 new policy HTMLs).
3. Sign in on [render.com](https://render.com) → **New + → Static Site**.
4. Select your repository. Render auto-detects `render.yaml` → click **Create Static Site**.
5. Live in ~1 minute at `https://YOUR-SITE.onrender.com`.

Every commit auto-deploys.

### Custom domain

Render dashboard → **Settings → Custom Domains → Add**. Free HTTPS.

---

## 📞 Contact details baked into the site

| Detail | Value |
|---|---|
| Primary WhatsApp | +91 70709 99457 |
| Secondary phone | +91 77830 34951 |
| Address | Askuri Complex, Utri Sangat, Phulwarisharif, Patna |
| Coordinates | 25.57954868414266, 85.0747359 |
| Store hours | Mon – Sun, 8:00 AM – 10:00 PM |

To change any of these, open the relevant `.html` file and search-and-replace:

| Change | Find |
|---|---|
| Primary WhatsApp / phone | `917070999457` and `70709 99457` |
| Secondary phone | `917783034951` and `77830 34951` |
| Address | `Askuri Complex` |
| Map coordinates | `25.57954868414266` |
| Business hours | `8:00 AM — 10:00 PM` |

The policy pages also contain these details — update all HTML files at once for consistency.

---

## 🎨 Design & Branding

**Brand typography:**
- **Anshu** — bold, 26px, deep blue (primary emphasis)
- **MEDICINE CENTRE** — small caps, 11px, green (tagline)

**Color palette:**
```css
--primary-blue:   #1F4E7A;   /* deep AMC blue */
--secondary-blue: #2C6FA6;   /* lighter blue */
--accent-green:   #3FB255;   /* AMC green */
--light-green:    #A8D468;   /* soft green */
--whatsapp:       #25D366;   /* WhatsApp brand green */
```

---

## ✨ Features included

- ✅ Fully responsive (phone → tablet → desktop)
- ✅ Auto-rotating hero slider with 3 slides
- ✅ Sticky mobile-friendly header with clean brand typography
- ✅ Prescription order form → auto WhatsApp
- ✅ 12 medicine categories with one-click WhatsApp inquiry
- ✅ Floating WhatsApp button
- ✅ Google Maps embed pinned to exact shop location
- ✅ "Get Directions" button
- ✅ Schema.org structured data for local SEO
- ✅ Open Graph tags for social sharing
- ✅ **Privacy Policy, Refund Policy, T&C — full pages for API approval**
- ✅ Zero dependencies, zero build step
- ✅ Free HTTPS on Render

---

## 🖼️ Replacing the logo

The site uses `logo.jpg` (wide) in header/footer and `logo-square.jpg` for favicon & social share. To replace:

1. Save your new file with the **same filename** in the same folder.
2. Done — no code changes needed.

---

## 🆘 Troubleshooting

**Policies not accessible?** Confirm all 3 HTML files are uploaded alongside `index.html`. Test in the browser: `yoursite.onrender.com/privacy-policy.html` etc.

**WhatsApp API application rejected?** Common reasons:
- Missing contact info on policy pages (all 3 have full contact block ✓)
- Missing "last updated" date (all 3 have this ✓)
- Policies not accessible via HTTPS (Render provides free HTTPS ✓)
- Business name mismatch between WhatsApp account and website — make sure both say "Anshu Medicine Centre"

**Logo not showing?** Confirm `logo.jpg` and `logo-square.jpg` are in the same folder as HTML files.

**Cache issue after update?** Hard refresh: Ctrl+Shift+R (desktop) or clear browser cache (mobile).

---

Made with care for Anshu Medicine Centre • Askuri Complex, Utri Sangat, Phulwarisharif, Patna
