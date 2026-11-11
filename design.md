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
  background: '#FAF7F2'
  surface: '#FAF7F2'
  surface-dim: '#EFE9DF'
  surface-bright: '#FFFFFF'
  surface-container-lowest: '#FFFFFF'
  surface-container-low: '#F4EFE6'
  surface-container: '#FFFFFF'
  surface-container-high: '#EDE5D8'
  surface-container-highest: '#E2D7C5'
  on-surface: '#1C1917'
  on-surface-variant: '#575047'
  outline: '#786F63'
  outline-variant: '#DCD2C4'
  primary: '#8C5E35'
  primary-container: '#8C5E35'
  on-primary-container: '#FFFFFF'
  secondary: '#B45309'
  tertiary: '#C84900'
typography:
  display:
    fontFamily: Playfair Display
    fontSize: 56px
    fontWeight: '600'
    lineHeight: 64px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 40px
    fontWeight: '500'
    lineHeight: 48px
    letterSpacing: -0.01em
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

## 2. Brand & Style Philosophy (Sunlit Florida Limestone & Travertine)
Designed for Florida homeowners, custom builders, and architects, the interface projects warmth, sunlit clarity, architectural elegance, and inviting residential curb appeal.

- **Light Luxury Palette:** Alternating sections of Warm Alabaster (`#FAF7F2`), Soft Travertine Cream (`#F4EFE6`), Crisp White (`#FFFFFF`) elevated cards, and Honed Limestone Sand (`#EDE5D8`).
- **Clean Hero Viewport:** Starts immediately with the `<h1>` below the fixed navigation header over a bright, wide-angle sunlit Florida Mediterranean estate photograph (`hero-luxury-architectural-precast-foam-estate-florida.webp`) with zero dark scrims or cluttered technical badges above the headline, and two focused CTA buttons (*Request Bespoke Quote* and *Explore Elements Gallery*).
- **Scroll Choreography:**
  - **Hero Zoom-Out:** The wide-angle estate photo loads at full brightness and gently scales down from `1.16x` to `1.00x` as the user scrolls.
  - **Rolodex / Tabular Section Stacking:** Each subsequent section slides upward with a rounded top edge and soft daylight shadow over the previous section as the outgoing section gently recedes (`scale(0.945)`).
