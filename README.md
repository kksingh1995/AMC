# Anshu Medicine Center — Website

Live-ready static website for **Anshu Medicine Center**, Phulwarisharif, Patna. Mobile-friendly, WhatsApp ordering, prescription upload, ready to deploy on Render.

---

## 📁 Files in this folder

| File | Purpose |
|---|---|
| `index.html` | Complete website (open this in a browser) |
| `logo.svg` | AMC logo — used everywhere on the site (guaranteed to show) |
| `render.yaml` | Render deployment configuration (auto-detected) |
| `README.md` | This file |

Nothing else needed. Zero build step. Zero dependencies. Just static HTML.

---

## 🚀 Deploy on Render (2 methods)

### Method 1 — GitHub deploy (recommended, auto-updates)

1. Create a new GitHub repository (name it anything, e.g. `anshu-medicine`).
2. Upload all 4 files (`index.html`, `logo.svg`, `render.yaml`, `README.md`) to the repo — you can drag-and-drop on github.com.
3. Go to **[render.com](https://render.com)** → sign in with GitHub.
4. Click **New +** → **Static Site**.
5. Select your repository.
6. Render auto-detects `render.yaml` and fills everything. Just click **Create Static Site**.
7. Wait ~1 minute → your site is live at `https://anshu-medicine-center.onrender.com` (or a similar URL).

**Bonus:** Every time you push a change to GitHub, Render auto-deploys the new version.

### Method 2 — Direct upload (fastest, no GitHub)

1. ZIP the entire folder (all 4 files).
2. Go to **[render.com](https://render.com)** → **New +** → **Static Site**.
3. Choose **"Deploy without a Git repository"** (if the option is available) OR create a private GitHub repo and upload the ZIP contents there.
4. Set **Publish directory** to `./` (root).
5. Deploy.

### Custom domain (optional)

Once deployed, in the Render dashboard:
- Go to **Settings → Custom Domains → Add**.
- Enter your domain (e.g. `anshumedicine.com`).
- Update your DNS provider with the CNAME record Render gives you.
- Done — HTTPS is free and automatic.

---

## 🖼️ Want to use your own logo image?

The site currently uses `logo.svg` — a clean AMC-branded vector logo. If you want to replace it with your original JPEG/PNG:

1. Save your logo file as `logo.svg` (or `logo.png`) in the same folder.
2. If you use a different filename or extension, open `index.html` and search for `logo.svg` — replace **both occurrences** (header + footer) with your filename.
3. Also update the `<link rel="icon" href="logo.svg">` line at the top.

**Tip:** For a professional look, keep the logo transparent-background and roughly 3:1 aspect ratio (wider than tall).

---

## 📱 How the WhatsApp order works

When someone fills the prescription order form:

1. Their details (name, phone, address, medicines, order type) get packed into a WhatsApp message.
2. WhatsApp opens with the message pre-filled, addressed to **+91 77810 08157**.
3. A popup reminds them to **attach the prescription photo** in the chat.
4. Customer sends → you receive the complete order on WhatsApp.

Category cards, floating WhatsApp button, and header "Order Now" button all open WhatsApp with context-aware messages too.

---

## ✏️ Where to update details

Open `index.html` in any text editor and use **Ctrl+F** (Find & Replace):

| Change | Find |
|---|---|
| Primary WhatsApp / phone | `917781008157` |
| Second phone | `917783034951` |
| Address | `Askuri Complex` |
| Business hours | `8:00 AM — 10:00 PM` |
| Store name | `Anshu Medicine Center` |
| Facebook link | `aria-label="Facebook"` (nearby `href="#"`) |
| Instagram link | `aria-label="Instagram"` (nearby `href="#"`) |

### Changing the map location

1. Open Google Maps, search your exact shop location.
2. **Share → Embed a map → Copy HTML.**
3. In `index.html`, find `<iframe` (in the Contact section) and replace the `src` URL.

---

## 🎨 Color palette

Defined once at the top of the stylesheet in `index.html`. Change these variables and the whole site updates:

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
- ✅ Sticky mobile-friendly header
- ✅ Prescription order form → auto WhatsApp
- ✅ 12 medicine categories with one-click WhatsApp inquiry
- ✅ Floating WhatsApp button with pulse animation
- ✅ Trust indicators, services grid, 3-step ordering guide
- ✅ Google Maps location embed
- ✅ Optimized mobile view with proper navigation
- ✅ SEO meta tags
- ✅ Zero dependencies, zero build step
- ✅ Free HTTPS on Render

---

## 🆘 Troubleshooting

**Logo not showing?** Make sure `logo.svg` is in the same folder as `index.html` and both are uploaded to your host.

**Form doesn't open WhatsApp?** WhatsApp must be installed on the customer's device (or they need WhatsApp Web open). This is normal behavior.

**Site looks broken on Render?** Check that your **Publish Directory** is set to `./` (just a dot and slash) — not `dist` or `build`.

---

Made with care for Anshu Medicine Center • Askuri Complex, Utri Sangat, Phulwarisharif, Patna
