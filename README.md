# Fariba Fallah – website

A one-page, mobile-first website to link from Instagram. Visitors see photos, a short bio, the services grouped by
category (Brows, Lips, Eyes, Extras) with an explanation, photos and a price for each, a price list, how to book,
aftercare, and a floating **Book now** button that opens WhatsApp.

## What is in this folder

| Folder / file | What it is |
|---|---|
| `index.html` | **The website** (Dark Luxe design, chosen on 22 Nov 2026), live at https://faribafallahpmu.github.io. This single file plus the `photos` folder is everything that is online. |
| `templates/` | The three original proposals (Ivory & Gold, Modern Minimal, Dark Luxe), kept for reference |
| `previews/` | Full-page screenshots: `index-mobile.png` and `index-desktop.png` are the site, the others are the old proposals |
| `photos/` | Web-sized copies of the photos used on the page (the originals stay in Downloads) |
| `content-checklist.md` | What is still missing to finish the site |

Double-click `index.html` to open the site in your browser. Make the window narrow to see the phone version.

Design decisions so far: Dark Luxe colours and shapes; no buttons under the name at the top, only small text links to
the categories; every booking button is WhatsApp green and opens WhatsApp with a ready-made message; the cover-up
block asks for a photo first; location shown as "Dubai Media City" only.

## Where the content comes from

All texts, prices, aftercare steps and work photos come from the page you wrote earlier in a claude.ai chat
(artifact "Fariba Fallah PMU"), restyled in the Dark Luxe design. Only the "Powder brows" explanation was written here,
since the artifact listed it with a price but no description. Client reviews are still hidden until you provide some.

## Photos used

| File in `photos/` | Used for |
|---|---|
| `portrait.jpg` | Main photo at the top (café, lipstick) |
| `about-1.jpg` | About section (laptop at the café) |
| `microblading-1..3.jpg`, `nanoblading-1..3.jpg` | Brows: microblading and nanoblading strips |
| `cover-up-1..9.jpg` | Brows: cover-up strip, before on top and after below |
| `lamination-1..2.jpg` | Brows: lamination strip |
| `lip-blush-1..7.jpg` | Lips: lip blush strip |
| `lash-line-1..5.jpg`, `lash-lift-1..2.jpg` | Eyes: lash line and lash lift strips |
| `beauty-spot-1.jpg` | Extras: beauty spot |

To change a photo, replace the file in `photos/` and keep the same name, or drop new photos in that folder and say
which goes where.

## How the content works

At the bottom of `index.html` there is a block that starts with `EDIT YOUR CONTENT HERE`. It holds the WhatsApp
number, the Instagram handle, the highlights row, the reviews, the service categories (each service with its texts,
photos, key points, price and WhatsApp message) and the price list. Changing a price or adding a service only needs
a change there.

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
