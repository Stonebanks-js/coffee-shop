# Fernrow — café website

A four-page static website for a small café, built to the brief in
*Simple Café Website — Website Development Project* (HTML, CSS, a little JavaScript).

| Page | File | What is on it |
| --- | --- | --- |
| Home | `index.html` | Welcome, what the café is, where it is, opening hours, popular food and drinks, pictures of the room |
| About | `about.html` | How the café started, and what it believes in |
| Menu | `menu.html` | Breakfast, lunch, drinks and desserts, with prices |
| Contact | `contact.html` | Contact form, address, opening hours, directions |
| Credits | `credits.html` | Photograph sources and licences |

## Running it locally

It is plain HTML, CSS and JavaScript — no build step. The scripts are ES modules, so
open it over HTTP rather than from the file system:

```bash
npx serve .
# then open http://localhost:3000
```

## Deploying

The site is a static deployment. From this folder:

```bash
npx vercel login      # once
npx vercel --prod
```

`vercel.json` sets long cache headers for `assets/` and two security headers.
`.vercelignore` keeps the build-check folders out of the upload.

## What the client still has to supply

Everything in this list is a stand-in. The site is finished; these values are not.

1. **The name.** "Fernrow" is a coined placeholder (the searches are recorded in `names.json`).
   Replace it in the `<title>`, the nav logo, the footer and `credits.html`.
2. **The address.** Only a district is printed ("Jericho, Oxford"), never a street number — add
   the real street and district, and update the five OpenStreetMap links.
3. **The phone number.** Deliberately left out rather than invented. `contact.html` has a
   commented-out slot in the visit block; fill it in and uncomment it.
4. **The form endpoint.** The contact form posts to `mailto:hello@fernrow.example`. Point
   `action` at the café's real form handler (or a real mailbox).
5. **The opening hours and every price.** Plausible values, not real ones.
6. **The story on the About page** and the three beliefs.
7. **The photographs.** Every picture is a library stand-in of another café, used under the
   licences listed on `credits.html`. They must be replaced with the café's own before the
   site goes live — see `PHOTO-SHOT-LIST.md`.
8. **The social links** point at the platforms' home pages. Point them at the café's accounts,
   or delete the `.socials` block from the footer of all four pages.

## Structure

```
index.html  about.html  menu.html  contact.html  credits.html
vercel.json
assets/
  system.css  system.js        design system: tokens, grid, nav, footer, cards, forms
  layout/     layout.css .js   section heights, the place hero, the one-section-per-screen rhythm
  motion/     motion.css .js   the hover and focus layer (buttons, links, photo zoom, card lift)
  ui/         cards.css ui.js
  icons/      icon.css + the three social marks
  img/        the photographs (webp, with srcset)
```

Each page carries its own small `<style>` block at the top for the few things the design
system does not size: the large address type on the home page, the picture wall, and one
tablet rule per section.
