# Fariba Fallah – website

A one-page, mobile-first website to link from Instagram. Visitors see photos, a short bio, the services with prices
(auto-moving carousel), client reviews, and a floating **Book now** button that opens WhatsApp.

## What is in this folder

| Folder / file | What it is |
|---|---|
| `index.html` | **The website** (Dark Luxe design, chosen on 22 Nov 2026). This single file plus the `photos` folder is everything that goes online. |
| `templates/` | The three original proposals (Ivory & Gold, Modern Minimal, Dark Luxe), kept for reference |
| `previews/` | Full-page screenshots: `index-mobile.png` and `index-desktop.png` are the site, the others are the old proposals |
| `photos/` | Web-sized copies of the photos used on the page (the originals stay in Downloads) |
| `content-checklist.md` | What is still missing to finish the site |

Double-click `index.html` to open the site in your browser. Make the window narrow to see the phone version.

Design decisions so far: one "Book now" button only, floating at the bottom right (the header has none);
every service card and the cover-up section open WhatsApp with a ready-made message; a "Cover-up, step by step"
section explains the photo-check-first flow from the ads.

## What is real and what is still an example

Real, taken from your photos and your Instagram ads: the profession (permanent makeup artist), Dubai Media City and
free parking, the Instagram handle `@fariba.fallahpmu`, the cover-up price of 1,800 AED and its
"send a photo first, then we book" flow.

Examples to replace: the WhatsApp number, every other price, the bio text, the "8+ years · 1,200+ clients · 5.0"
row, the reviews and the opening hours.

## Photos used

| File in `photos/` | Comes from | Used for |
|---|---|---|
| `portrait.jpg` | IMG_7851 (café, lipstick) | Main photo at the top |
| `about-1.jpg` | IMG_7849 (laptop at the café) | About section |
| `about-2.jpg` | IMG_7850 (mirror photo) | About section, small photo |
| `microblading.jpg` | IMG_7845, "after" half | Microblading card |
| `powder-brows.jpg` | IMG_7846, "after" half | Powder brows card |
| `lip-blush.jpg` | Close-up of brows and lips, cropped to the lips | Lip blush card |
| `cover-up.jpg` | IMG_7845, before and after stacked | Cover-up card |
| `before-after-1.jpg`, `before-after-2.jpg` | IMG_7845, IMG_7846 | Gallery |
| `brows-lips.jpg` | Close-up of brows and lips | Gallery |
| `lash-lift.jpg`, `lash-lift-2.jpg`, `brow-lamination.jpg` | IMG_2307, IMG_5346, IMG_3923 | Lash lift and brow lamination cards, gallery |

To change a photo, replace the file in `photos/` and keep the same name, or drop new photos in that folder and say
which goes where.

## How the content works

At the bottom of `index.html` there is a block that starts with `EDIT YOUR CONTENT HERE`. It holds the WhatsApp
number, the Instagram handle, the services (name, description, duration, price, photo) and the reviews.
Changing a price or adding a service only needs a change there.

## Going online, step by step

1. Create a free GitHub account at github.com/signup (in Safari or Chrome). Choose the username **faribafallah**
   if it is free: the site address becomes `https://faribafallah.github.io`. If it is taken, use `fariba-fallah`
   (address `https://fariba-fallah.github.io`). Pick the Free plan and confirm the email they send you.
2. Run the one-line command Claude gives you in the terminal. It creates a key on this Mac; copy the text it prints.
3. Add that key to the account, so the site can be updated from here without passwords:
   GitHub → profile picture → Settings → SSH and GPG keys → New SSH key → paste the text → Add SSH key.
4. Create the repository: GitHub → + (top right) → New repository → name it exactly `faribafallah.github.io`
   (your username followed by `.github.io`) → Public → Create repository.
5. Say "done" in the chat. Claude publishes the site, and the address works a minute or two later.

## Putting it online for free

The address `fariba.fallah` is not possible: a web address must end with a real extension such as `.com` or `.ae`,
and `.fallah` does not exist. Free options that keep the name:

| Option | Address | Notes |
|---|---|---|
| GitHub Pages (recommended) | `https://faribafallah.github.io` | Free, reliable, no ads. Needs a free GitHub account. |
| Netlify | `https://fariba-fallah.netlify.app` | Free, drag-and-drop upload. |
| Vercel | `https://fariba-fallah.vercel.app` | Free, similar to Netlify. |

A real domain such as `faribafallah.com` costs about 10–15 € per year and can be connected to any of these later
without changing the site.
