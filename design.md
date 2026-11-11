---
name: Precast and Foam Works
business_info:
  name: Precast and Foam Works
  phone: '(727) 657-9195'
  phone_e164: '+17276579195'
  address: '6612 Osteen Rd #332-333, New Port Richey, FL 34653'
  hours:
    monday_friday: '7:00 AM – 4:30 PM'
    saturday: '9:00 AM – 2:00 PM'
    sunday: 'Closed'
colors:
  surface: '#111317'
  surface-dim: '#111317'
  surface-bright: '#37393d'
  surface-container-lowest: '#0c0e12'
  surface-container-low: '#1a1c20'
  surface-container: '#1e2024'
  surface-container-high: '#282a2e'
  surface-container-highest: '#333539'
  on-surface: '#e2e2e7'
  on-surface-variant: '#d2c4b7'
  inverse-surface: '#e2e2e7'
  inverse-on-surface: '#2e3035'
  outline: '#9b8f83'
  outline-variant: '#4e453b'
  surface-tint: '#e6c093'
  primary: '#e6c093'
  on-primary: '#432c0a'
  primary-container: '#8c6d46'
  on-primary-container: '#fff8f4'
  inverse-primary: '#765934'
  secondary: '#ffb691'
  on-secondary: '#542101'
  secondary-container: '#713714'
  on-secondary-container: '#f4a277'
  tertiary: '#ffb598'
  on-tertiary: '#591c00'
  tertiary-container: '#c84900'
  on-tertiary-container: '#fff8f6'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffddb6'
  primary-fixed-dim: '#e6c093'
  on-primary-fixed: '#2a1800'
  on-primary-fixed-variant: '#5c421f'
  secondary-fixed: '#ffdbcb'
  secondary-fixed-dim: '#ffb691'
  on-secondary-fixed: '#341100'
  on-secondary-fixed-variant: '#713714'
  tertiary-fixed: '#ffdbce'
  tertiary-fixed-dim: '#ffb598'
  on-tertiary-fixed: '#370e00'
  on-tertiary-fixed-variant: '#7f2b00'
  background: '#111317'
  on-background: '#e2e2e7'
  surface-variant: '#333539'
typography:
  display:
    fontFamily: Playfair Display
    fontSize: 56px
    fontWeight: '600'
    lineHeight: 64px
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: Playfair Display
    fontSize: 36px
    fontWeight: '600'
    lineHeight: 44px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 40px
    fontWeight: '500'
    lineHeight: 48px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 28px
    fontWeight: '500'
    lineHeight: 36px
  headline-md:
    fontFamily: Playfair Display
    fontSize: 28px
    fontWeight: '500'
    lineHeight: 36px
  headline-sm:
    fontFamily: Playfair Display
    fontSize: 22px
    fontWeight: '600'
    lineHeight: 30px
  title:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 26px
    letterSpacing: 0.01em
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 26px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 22px
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.08em
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 10px
    fontWeight: '700'
    lineHeight: 14px
    letterSpacing: 0.12em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1.5rem
  gutter-mobile: 1rem
  margin: 4rem
  margin-mobile: 1.25rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 3rem
---

# Precast and Foam Works — Design System & Technical Specification

## 1. Brand Identity & NAP (Single Source of Truth)
- **Business Name:** Precast and Foam Works
- **Phone:** (727) 657-9195 (`tel:+17276579195`)
- **Address:** 6612 Osteen Rd #332-333, New Port Richey, FL 34653
- **Operating Hours:**
  - **Monday–Friday:** 7:00 AM – 4:30 PM
  - **Saturday:** 9:00 AM – 2:00 PM
  - **Sunday:** Closed

## 2. Brand & Style Philosophy
The brand manifests an ultra-luxurious, bespoke architectural facade and stone craftsmanship identity. Designed for elite architects, custom home builders, real estate developers, and high-end residential visionaries across Florida, the interface projects timeless permanence, structural precision, and monumental weight.

The aesthetic fuses **Architectural Minimalism** with **Dark Luxury Modernism**. High-contrast tonal surfaces echo raw limestone slabs, hand-patinated architectural bronze, and charcoal structural steel. Layouts evoke architectural portfolio monographs—deliberate whitespace, monolithic alignments, and hairline bronze division lines rather than casual UI framing. Interactions feel measured, dense, and deliberate, avoiding playful bounce in favor of damped, mechanical transitions.

## 3. Signature Scroll Choreography

### 3.1 Scroll-Linked Hero Background Zoom-Out & Clarify
- **Initial State (Scroll = 0):** The Hero architectural photography (`hero-luxury-architectural-precast-foam-estate-florida.webp`) begins at an intimate, monumental scale (`scale(1.26)`) behind a directional charcoal-and-bronze scrim so headline typography commands immediate focus.
- **Scroll Progression:** As the user scrolls through the Hero viewport, the background image smoothly scales down toward `scale(1.0)` while the overlay scrim opacity eases back (`0.82` -> `0.38`) and image brightness/contrast sharpens. This allows the user to progressively see the full architectural detail of the Corinthian columns, arches, and cornice profiles before the next section glides over.

### 3.2 Tabular / Rolodex Section Overlap Stack
- **Card-Stack Architecture:** Every major page section after the Hero acts as a physical architectural dossier plate in a **Tabular / Rolodex stack** (`position: sticky` with dynamic viewport top pinning).
- **Tabular Index Lip:** Each section features a top architectural index bar (`01 // HERO FOUNDRY`, `02 // ENGINEERED FABRICATION`, `03 // ARCHITECTURAL PORTFOLIO`, `04 // BUILDER ENDORSEMENTS`, `05 // TECHNICAL FAQS`, `06 // BESPOKE ESTIMATION & FACILITY`) with a 1px specular bronze top border (`rgba(230, 192, 147, 0.35)`) and deep upward occlusion shadow (`0 -28px 64px rgba(0, 0, 0, 0.88)`).
- **Receding Rolodex Physics:** As the incoming section slides upward to overlap the active section, the outgoing section smoothly recedes in 3D space (`scale(0.94) translateY(-18px) rotateX(2.5deg)`) and dims (`brightness(0.38) blur(2px)`), disappearing cleanly behind the new plate.

## 4. Color Architecture
The color architecture mirrors natural structural elements: patinated bronze, heat-treated copper, monolithic graphite, and aged quarry travertine.

- **Primary (`#8C6D46` / Bronze Container & `#E6C093` Primary Accent):** Anchors primary actions, architectural highlights, and elevated linear detailing. Emits the deep, non-reflective luster of hand-rubbed statuary bronze.
- **Secondary (`#C87D55` / `#FFB691` Warm Copper):** Serves as warm chromatic support for active states, material specification badges, and subtle linear gradients across dark substrates.
- **Tertiary (`#C84900` / `#FFB598` Terracotta Core):** Applied for high-priority engineering CTAs, status indicators, and focal points against deep charcoal canvases.
- **Neutral Charcoal Slate (`#111317` Canvas, `#1E2024` Card / Surface, `#282A2E` Elevation):** Creates a high-depth background hierarchy mimicking honed basalt and graphite panels.
- **Travertine Ivory (`#E2E2E7` / `#FFF8F4`):** Reserved for high-legibility display headings, technical readouts, and primary body copy to preserve contrast across dark stone fields.

## 5. Typography & Semantic SEO Hierarchy
Typographic pairings balance classical monumental prestige (`Playfair Display`) with modern engineering clarity (`Plus Jakarta Sans`).

- **`<h1>` (Single Primary Page Title):** Reserved strictly for the Hero headline (*"Mastering Florida’s Architectural Elegance & Stone Precision"*), establishing primary topical authority for custom EPS architectural foam and precast limestone in New Port Richey & Tampa Bay, Florida.
- **`<h2>` (Major Section Headings):** Used for each primary Rolodex section title (*Architectural Mastery & Materials Science*, *Architectural Portfolio Elements*, *Trusted by Florida’s Elite Builders*, *Frequently Asked Engineering & Fabrication Questions*, *Request Bespoke Estimation Consultation*).
- **`<h3>` (Sub-Section & Card Titles):** Used for individual material systems, portfolio categories (*Tuscan & Corinthian Columns*, *Custom Mantels & Fireplace Surrounds*, etc.), FAQ questions, and the *New Port Richey Production Facility* heading.
- **`<h4>` (Technical Sub-Headings & Footer Columns):** Used for metric callouts, client endorsement attributions, facility dispatch sub-blocks, and footer taxonomy headers.

## 6. Image & Structured Data Standards
- **100% WebP Asset Pipeline:** All visual assets (`assets/images/*.webp`) are encoded in `.webp` format with explicit `width`, `height`, `loading` (`eager` + `fetchpriority="high"` for LCP hero/logo; `lazy` for below-the-fold portfolio cards), and descriptive keyword-rich `alt` attributes describing the exact architectural profile and material.
- **JSON-LD Schema Markup:**
  - `HomeAndConstructionBusiness` / `LocalBusiness` + `ManufacturingBusiness` with full NAP (`Precast and Foam Works`, `6612 Osteen Rd #332-333, New Port Richey, FL 34653`, `(727) 657-9195`), geo coordinates, `OpeningHoursSpecification` (Mon–Fri 07:00–16:30, Sat 09:00–14:00), `hasOfferCatalog`, and `AggregateRating` / `Review` nodes.
  - `FAQPage` schema matching the visible technical FAQ accordion section 1-to-1.
  - `WebPage` & `ImageObject` metadata for rich search indexing.
