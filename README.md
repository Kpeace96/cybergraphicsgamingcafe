# Cyber Graphics Gaming Cafe — Website

A single-page, mobile-friendly website for Cyber Graphics Gaming Cafe (South Africa), built with plain HTML, CSS, and JavaScript — no frameworks, no build step required.

## Overview

This site showcases services, collects orders via WhatsApp, and includes a live (browser-local) comments section.

**Current service status:**
- ✅ Active: Website Setup, Graphic Design, Business Registration
- 🚧 Under Construction: Gaming Sessions, Printing

## Features

- **Responsive design** — adapts from desktop down to mobile
- **Services section** — pricing cards for all 5 services, with disabled states for services under construction
- **Order form** — collects name, email, service, budget, and details, then opens WhatsApp with a pre-filled message
- **Live comments** — visitors can post comments, saved in the browser via `localStorage`
- **Reviews section** — static testimonials
- **Social links** — WhatsApp, Facebook, Instagram
- **Reduced motion support** — respects `prefers-reduced-motion` for accessibility

## File Structure

## Setup

1. Download/save `index.html`.
2. (Optional) Add a `logo.jpg` file in the same folder for your logo — if missing, a styled "CG" fallback badge is shown automatically.
3. Open `index.html` in any browser, or upload it to any static web host.

## Customization

| To change... | Edit this... |
|---|---|
| WhatsApp number | `waNumber` variable in the `<script>` section, and the `href="https://wa.me/..."` links |
| Prices/services | The `.service` cards inside `<section id="services">` |
| Social links | The `<div class="socials">` block |
| Colors/theme | CSS variables at the top of `<style>` (`--brand`, `--brand2`, `--bg`, etc.) |
| Reviews | `<section id="reviews">` testimonial cards |

## Notes on the Comments Section

- Comments are stored using `localStorage`, meaning they are **only visible on the device/browser that posted them** — they are not shared publicly or synced across visitors.
- If you want public, shared comments visible to all visitors, this would need a backend or database (currently not implemented).

## Deployment

This is a static site — it can be hosted for free on services like:
- GitHub Pages
- Netlify
- Vercel
- Any standard web hosting (cPanel, etc.)

Just upload `index.html` (and `logo.jpg` if used) — no build tools or server required.

## License / Ownership

© 2026 Cyber Graphics Gaming Cafe. All rights reserved.
