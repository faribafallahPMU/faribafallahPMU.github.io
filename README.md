# Fariba Fallah – website

A one-page, mobile-first website to link from Instagram. Visitors see photos, a short bio, the services with prices
(auto-moving carousel), client reviews, and a floating **Book now** button that opens WhatsApp.

## What is in this folder

| Folder / file | What it is |
|---|---|
| `index.html` | **The website** (Dark Luxe design, chosen on 22 Nov 2026), live at https://faribafallahpmu.github.io. This single file plus the `photos` folder is everything that is online. |
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

Still missing (hidden or shown as "price on request" until provided): the WhatsApp number, every other price,
the highlights row, the reviews, the opening hours and the bio details.

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

## The site online

The site is live at **https://faribafallahpmu.github.io** (GitHub account `faribafallahPMU`, repository
`faribafallahPMU.github.io`, published by GitHub Pages from the `main` branch, HTTPS enforced). It was uploaded
through GitHub's website on 22 Nov 2026 from a logged-in Chrome; no key or password is stored on this Mac.

To update the site: change `index.html` or a photo here, then either upload the changed file again through
GitHub's website (Add file → Upload files, same name replaces the old one) or set up the one-time SSH key from
the command below so updates can be pushed directly from this folder.

The address `fariba.fallah` is not possible: a web address must end with a real extension such as `.com` or `.ae`.
A real domain such as `faribafallah.com` costs about 10–15 € per year and can be connected to the GitHub Pages
site later (Settings → Pages → Custom domain) without changing anything else.

One-time key setup (optional, run in the terminal, then add the printed line to GitHub → Settings → SSH and GPG keys):

```
mkdir -p ~/.ssh && chmod 700 ~/.ssh && ssh-keygen -t ed25519 -N "" -C "fariba-website" -f ~/.ssh/id_ed25519_github && printf '\nHost github.com\n  IdentityFile ~/.ssh/id_ed25519_github\n  IdentitiesOnly yes\n' >> ~/.ssh/config && ssh-keyscan -t ed25519 github.com >> ~/.ssh/known_hosts 2>/dev/null && cat ~/.ssh/id_ed25519_github.pub
```
