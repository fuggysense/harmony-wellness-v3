# Harmony Wellness V3 — Site-Builder Assembly Guide

## Section Order

| # | File | Section | Background |
|---|------|---------|------------|
| 00 | `00-fonts.html` | Google Fonts | Add to `<head>` |
| 01 | `01-nav.html` | Navigation bar | White `#ffffff` |
| 02 | `02-hero.html` | Hero + parallax | Photo/video bg |
| 03 | `03-about.html` | Brand intro | Cream `#FAF7F2` |
| 04 | `04-trust.html` | Trust badges | Cream `#FAF7F2` |
| 05 | `05-treatments.html` | Treatment cards (scroll-pin) | Cream `#FAF7F2` |
| 06 | `06-conditions.html` | Conditions grid | Stone `#F4EFE8` |
| 07 | `07-philosophy.html` | Three Pillars | Cream `#FAF7F2` |
| 08 | `08-gallery.html` | Photo gallery | Cream `#FAF7F2` |
| 09 | `09-heritage.html` | Five Centuries (dark) | Dark `#1E1B18` |
| 10 | `10-trial.html` | $89 Trial offer | Dark overlay |
| 11 | `11-testimonials.html` | Marquee testimonials | Cream `#FAF7F2` |
| 12 | `12-contact.html` | Visit Us + CTAs | Cream `#FAF7F2` |
| 13 | `13-footer.html` | Footer, QR, social | Dark `#1E1B18` |
| 14 | `14-whatsapp-fab.html` | Floating WhatsApp btn | Fixed position |

## How to Use in Page Builders

### GoHighLevel / WordPress Elementor / Any HTML block

1. Add `00-fonts.html` content to your page's **Header Code Injection** or `<head>` area
2. Paste each section (01–14) into sequential HTML blocks
3. Each section is self-contained with its own `<style>` block

### Find & Replace Checklist

Before publishing, search for these placeholders and replace:

| Find | Replace With |
|------|-------------|
| `https://placehold.co/600x800/...` | Your treatment card photos (600x800px) |
| `https://placehold.co/480x360/...` | Your gallery photos (480x360px) |
| `https://placehold.co/1440x720/...` | Your hero background photo |
| `https://placehold.co/1440x800/...` | Your trial section background photo |
| `wechat-qr.png` | Path to your WeChat QR code image |
| `whatsapp-qr.png` | Path to your WhatsApp QR code image |
| `https://wa.me/6590897778` | Your WhatsApp number link |
| `tel:+6590897778` | Your phone number |
| `<!-- EDIT:` markers | Review each and customize content |

### Sections with JavaScript

These sections include `<script>` tags that must be kept:

- **02-hero.html** — Parallax scroll effect on background
- **05-treatments.html** — Scroll-pinned card expansion (desktop only)
- **07-philosophy.html** — Stagger animation on pillar reveal

### Sections with CSS Animations

- **11-testimonials.html** — `@keyframes marquee-10-scroll` for auto-scrolling

## Color Palette

| Name | Hex | Usage |
|------|-----|-------|
| Background | `#FAF7F2` | Main page background |
| Surface | `#F4EFE8` | Conditions section bg |
| Sand | `#EDE8E0` | Borders, subtle fills |
| Text | `#2C2420` | Primary headings |
| Muted | `#8A7E74` | Section headings, labels |
| Body | `#6B5F56` | Body text |
| Jade | `#4A7C6F` | WhatsApp CTA button |
| Gold | `#C4956A` | Accent color throughout |
| Dark | `#1E1B18` | Heritage, footer backgrounds |

## Fonts

- **DM Serif Display** — Headings (serif)
- **Figtree** — Body text (sans-serif)
- **Noto Serif SC** — Chinese characters (serif)

## Responsive

All sections respond at `768px` breakpoint. Mobile behavior:
- Nav collapses to logo + Book Now button
- Treatment cards stack vertically (no scroll-pin)
- Two-column grids become single column
- Heritage section stacks story/poetry vertically

## Preview

Open `full-preview.html` in a browser to see all sections assembled with shared styles and scripts.
