# Moxie's Run — moxiesrun.com

Charity 5K run/walk for canine cancer. Mirrors the original Squarespace site at moxiesrun.com, rebuilt with Astro + Tailwind on Vercel.

## Stack

- **Astro 6** (static site)
- **Tailwind CSS 4** (via @tailwindcss/vite)
- **Vercel** — auto-deploys from `main`
- **Domain**: moxiesrun.com (currently on Squarespace — needs DNS switch to Vercel)

## Live URLs

- **Preview**: https://moxiesrun.vercel.app
- **Repo**: https://github.com/Aneshv1/moxiesrun

## Color Palette (extracted from Squarespace CSS)

| Token | Hex | HSL | Usage |
|-------|-----|-----|-------|
| `brand` | `#6554ba` | 250, 43%, 53% | Buttons, accents, dark purple |
| `brand-light` | `#7a6bc7` | — | Button hover |
| `accent` | `#beabfd` | 254, 95%, 83% | Light purple highlights |
| `light-accent` | `#bae4e9` | 186, 52%, 82% | Soft blue, icon backgrounds |

## Pages

| Route | File | Content |
|-------|------|---------|
| `/` | `index.astro` | Hero (photo + overlay), The Run, The Mission, Where Support Goes, CTA |
| `/about` | `about.astro` | Moxie's story (Beagle, brain/thyroid cancer), objectives, donations |
| `/event` | `event.astro` | Race details, schedule timeline, race kit, course map |
| `/sponsors` | `sponsors.astro` | Sponsorship inquiry form |
| `/fundraising` | `fundraising.astro` | $25/$100 donations, athletic hoodie ($74.14) |
| `/registration` | `registration.astro` | 3 tiers: With Dog ($97.95), No Dog ($67.95), Virtual ($29) |

## Images

All 18 images downloaded from Squarespace CDN into `public/images/`:

- `logo-main.png` — white logo (for dark backgrounds, used in footer)
- `logo-secondary.png` — colored blue/purple logo (for white backgrounds, used in header)
- `hero-home-1.jpg`, `hero-home-2.jpeg`, `content-home.jpg` — homepage
- `about-hero.jpg` — Moxie photo
- `event-hero.jpeg`, `course-map.jpg` — event page
- `sponsors-hero.jpg` — sponsors page
- `fundraising-collars-1/2.png`, `fundraising-hoodie-1/2/3/4.png` — merch
- `reg-with-dog.jpg`, `reg-no-dog.jpg`, `reg-virtual.jpg` — registration cards

## TODO

- [ ] Connect moxiesrun.com domain to Vercel (switch DNS from Squarespace)
- [ ] Hook up payment/registration links (currently `#` placeholders) — need Squarespace commerce URLs or new payment processor
- [ ] Wire up sponsor form to backend (Supabase, Formspree, etc.)
- [ ] Update event date/details for next year's race
- [ ] Add Google Analytics / Meta Pixel tracking

## Contact Info (hardcoded in site)

- **Phone**: 647-376-7016
- **Email**: info@k9academy.ca
- **Instagram**: @k9academyto
- **Location**: Toronto, Ontario

## Commands

```sh
npm install        # Install deps
npm run dev        # Dev server (check port — other projects may be on 4321-4324)
npm run build      # Build to ./dist/
git push           # Auto-deploys to Vercel
```
