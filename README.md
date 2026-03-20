# 🏨 JW Marriott Hotel Chandigarh — Premium Website Template (v2)

> A production-grade, fully animated luxury hotel website built with pure HTML, CSS & JavaScript. Deep ink + teal color theme with advanced micro-interactions, custom cursor, page loader, and cinematic animations.


---

## 🌐 Live Demo

👉 **[View Live Site](https://lucee8.github.io/Resort-Sample-1/)**

> Replace this link with your GitHub Pages URL after deployment (Settings → Pages → Enable).

---

## ✨ What Makes This Version Different

This is **Version 2** — a complete redesign over v1 with a brand new color palette and a full suite of professional animations.

### 🎨 New Color Theme — Deep Ink + Teal + Ivory

| Element | Color |
|---|---|
| Background | Near-black ink `#0D0D0F` |
| Primary accent | Deep teal `#1A6B6B` |
| Glow / highlight | Teal light `#4DB8B8` |
| Text | Soft ivory `#E8E4DC` |
| Gold touches | Warm amber `#C8A96E` |

### 🎬 Animation Features

| Animation | Description |
|---|---|
| **Page Loader** | Animated JW logo with sweeping bar — plays for 1.4s on first load |
| **Custom Cursor** | Glowing teal dot + lagging ring that expands on interactive elements |
| **Hero Pan** | Background image slowly drifts on an 18-second CSS keyframe loop |
| **Rotating Diamond** | Location `◆` icon continuously rotates on a 4s animation |
| **Slide-in Reveals** | Sections animate from left, right, or bottom on scroll |
| **Button Fill Effect** | All buttons fill with teal color from left-to-right on hover |
| **Logo Rotate** | Diamond logo mark rotates from 45° to 90° on hover |
| **Card Hover Depth** | Cards lift, brighten, and gain a teal glow border on hover |
| **Amenity Icon Bounce** | Icons spring up with `cubic-bezier(0.34, 1.56, 0.64, 1)` on hover |
| **Review Line Sweep** | Teal gradient line sweeps across card top on hover |
| **Scroll Indicator** | Bobbing scroll arrow at the bottom of the hero section |
| **Noise Texture** | Subtle film-grain overlay on the entire page for depth |

---

## 📦 Sections Overview

| Section | Description |
|---|---|
| **Navbar** | Fixed glassmorphism nav with animated underline links + diamond logo |
| **Hero** | Full-screen parallax with staggered reveal, stats row, scroll indicator |
| **Award Strip** | Teal bar listing hotel highlights (microbrewery, spa, Bonvoy, pool) |
| **Booking Bar** | Date pickers + guest counters → opens WhatsApp with pre-filled message |
| **Rooms & Suites** | 6 cards with tier badges, pricing overlay, hover brightness effect |
| **The JW Experience** | Two-column split with numbered list + layered image with badge |
| **Dining** | All 6 restaurants — Saffron, Cafe@JW, XO, 35 BrewHouse, CBC, Room Service |
| **Amenities** | 8 cards with animated icon bounce and teal top-border reveal |
| **Gallery** | Asymmetric 2-column grid with hover tint and spring icon |
| **CTA Strip** | Teal full-width call-to-action with decorative circle shapes |
| **Guest Reviews** | 3 cards with line-sweep hover effect and large quote mark |
| **Contact & Bookings** | Info cards + WhatsApp CTA + animated reservation form |
| **Footer** | 4-column footer with social icons, dining list, contact details |

---

## 🚀 Deploy to GitHub Pages (Step by Step)

### Step 1 — Rename the file
Rename `jw_marriott_v2_premium.html` → **`index.html`**
> GitHub Pages only serves `index.html` as the homepage.

### Step 2 — Create a GitHub Repository
1. Go to [github.com](https://github.com) → click **New**
2. Name it: `jw-marriott-chandigarh` (or any name)
3. Set to **Public** → click **Create repository**

### Step 3 — Upload Your Files
1. Inside the repo → click **"Add file" → "Upload files"**
2. Drag and drop both:
   - `index.html`
   - `README.md`
3. Write commit message: `Initial commit — JW Marriott v2`
4. Click **"Commit changes"**

### Step 4 — Enable GitHub Pages
1. Go to **Settings** tab → left sidebar → **Pages**
2. Under **Branch** → select `main`, folder `/ (root)`
3. Click **Save**
4. Wait ~2 minutes → your site is live at:

```
https://your-username.github.io/jw-marriott-chandigarh/
```

### Step 5 — Update the Live Demo Link
Edit this `README.md`, replace the placeholder URL at the top with your actual live URL.

---

## 🎨 How to Customize for Any Hotel Client

Everything lives in one `index.html` file. Open it in VS Code or any text editor and find-replace the following:

### Colors (CSS Variables — top of `<style>` tag)
```css
--teal: #1A6B6B;        /* Change to client's brand color */
--teal2: #228080;       /* Slightly lighter version */
--teal-light: #4DB8B8;  /* Glow and highlight color */
--accent: #C8A96E;      /* Gold / secondary accent */
```

### Hotel Details
| Find | Replace with |
|---|---|
| `JW Marriott` | Client hotel name |
| `Hotel Chandigarh` | Client's city/location |
| `Sector 35 B, Chandigarh 160035` | Client's actual address |
| `911724555555` | Client's WhatsApp number (country code + number, no +) |
| `+91 172-455 5555` | Client's display phone number |
| `stay@resortname.com` | Client's email |
| `5 Star Luxury` | Client's tier / tagline |
| `1800-102-5000` | Client's toll-free (or remove this line) |

### Logo Mark
Find the `JW` text inside the diamond logo:
```html
<span>JW</span>
```
Replace `JW` with the first 1–2 letters of the hotel name.

### Room Names & Prices
Find the room cards in the `#rooms` section and update:
- Room names (`Deluxe Room`, `Junior Suite`, etc.)
- Prices (`₹12,000`, `₹18,000`, etc.)
- Features (`City View`, `Club Lounge`, etc.)

### Restaurant Names
Find the `#dining` section and update:
- Restaurant names
- Cuisine tags
- Descriptions

### Photos
Replace Unsplash URLs with client's actual images:
```html
<!-- Before -->
src="https://images.unsplash.com/photo-1566073771259-6a8506099945?w=1600&q=90"

<!-- After (local file) -->
src="assets/images/hero.jpg"

<!-- After (hosted URL) -->
src="https://client-website.com/images/hero.jpg"
```

### Disable Custom Cursor (optional)
If the client prefers a standard cursor, find and remove:
```html
<div class="cursor" id="cursor"></div>
<div class="cursor-ring" id="cursorRing"></div>
```
And in CSS, change:
```css
body { cursor: none; }
```
to:
```css
body { cursor: auto; }
```

---

## 📁 Project Structure

```
jw-marriott-chandigarh/
│
├── index.html         ← Complete website (HTML + CSS + JS in one file)
├── README.md          ← This file
└── assets/            ← (Optional) Add client images here
    └── images/
        ├── hero.jpg
        ├── room-1.jpg
        └── ...
```

> This is a **single-file website** — everything is inside `index.html`. No build tools, no npm, no dependencies. Just open and it works.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure |
| CSS3 | Animations, layout, responsive design |
| Vanilla JavaScript | Cursor, loader, scroll effects, booking logic |
| Google Fonts | Cormorant (display serif) + Outfit (body sans) |
| CSS Custom Properties | Full theming system via variables |
| IntersectionObserver API | Scroll-triggered reveal animations |
| requestAnimationFrame | Smooth custom cursor lag effect |

**Zero dependencies. Zero frameworks. Zero build steps.**

---

## 💬 WhatsApp Integration — 3 Touchpoints

| Location | Behavior |
|---|---|
| **Floating button** (bottom right) | Always visible — opens WhatsApp chat instantly |
| **Contact section button** | "Chat on WhatsApp" with a pre-written greeting |
| **Check Availability button** | Sends check-in date, check-out date, adults, children & rooms as a pre-filled WhatsApp message |

To update the number, search for `911724555555` in the HTML and replace all instances:
- Format: country code + number, **no `+`, no spaces**
- Example India: `919876543210` (91 + 10-digit mobile)

---

## ✅ Pre-Delivery Checklist

Use this before handing the website to a client:

- [ ] Rename file to `index.html`
- [ ] Replace hotel name everywhere (`JW Marriott`, `Hotel Chandigarh`)
- [ ] Update WhatsApp number (`911724555555` → client's number)
- [ ] Update phone number and email address
- [ ] Update physical address and city
- [ ] Replace logo letters (`JW` → client initials)
- [ ] Update room names, features, and prices
- [ ] Update restaurant names and descriptions
- [ ] Replace all Unsplash placeholder images with real photos
- [ ] Adjust brand color (change `--teal` CSS variable)
- [ ] Test all WhatsApp links open correctly
- [ ] Test on mobile (hamburger menu, stacked layout)
- [ ] Test page loader works on first load
- [ ] Test custom cursor (or disable if client prefers default)
- [ ] Deploy to GitHub Pages or client's hosting
- [ ] Update live demo link in README

---

## 🔄 Version History

| Version | Theme | Key Features |
|---|---|---|
| **v1** | Dark Burgundy + Gold | Basic animations, booking bar, WhatsApp |
| **v2** | Deep Ink + Teal ← *this file* | Custom cursor, loader, parallax, slide reveals, button fills |

---

## 📄 License

This template is built for client delivery. Each deployed copy is customized for a specific hotel. Not for redistribution as-is.

---

## 👨‍💻 Built By

**Lucee** — Student & Web Developer
Building professional websites for hotels, resorts & local businesses.

📱 WhatsApp: [Chat with me](https://wa.me/91XXXXXXXXXX)
📷 Instagram: [@your_handle](https://instagram.com/your_handle)

---

> ⭐ Star this repo if you found it useful — it helps a student developer grow!
