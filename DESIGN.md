---
name: Executive Suite Design System
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#434651'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f1f1f1'
  outline: '#747782'
  outline-variant: '#c4c6d3'
  surface-tint: '#375ca8'
  primary: '#002155'
  on-primary: '#ffffff'
  primary-container: '#003580'
  on-primary-container: '#7fa1f2'
  inverse-primary: '#b0c6ff'
  secondary: '#7b5900'
  on-secondary: '#ffffff'
  secondary-container: '#febb02'
  on-secondary-container: '#6c4d00'
  tertiary: '#002251'
  on-tertiary: '#ffffff'
  tertiary-container: '#00377a'
  on-tertiary-container: '#72a2ff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d9e2ff'
  primary-fixed-dim: '#b0c6ff'
  on-primary-fixed: '#001945'
  on-primary-fixed-variant: '#1a438e'
  secondary-fixed: '#ffdea4'
  secondary-fixed-dim: '#febb02'
  on-secondary-fixed: '#261900'
  on-secondary-fixed-variant: '#5d4200'
  tertiary-fixed: '#d8e2ff'
  tertiary-fixed-dim: '#adc6ff'
  on-tertiary-fixed: '#001a41'
  on-tertiary-fixed-variant: '#004494'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
  success-emerald: '#10B981'
  warning-amber: '#F59E0B'
  error-rose: '#E11D48'
  charcoal-text: '#1A1A1A'
  room-dirty: '#94A3B8'
  room-out-of-order: '#475569'
typography:
  display-lg:
    fontFamily: Montserrat
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  title-lg:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  status-badge:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 12px
    letterSpacing: 0.03em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  grid-margin: 24px
  gutter: 16px
  stack-sm: 4px
  stack-md: 12px
  stack-lg: 24px
  section-padding: 40px
---

## Brand & Style
The design system is engineered for the high-stakes environment of hotel property management. The brand personality is **composed, efficient, and premium**, balancing the technical requirements of a SaaS platform with the warmth of the hospitality industry.

The design style follows a **Modern Corporate** aesthetic with **Minimalist** leanings. It prioritizes clarity and information density without sacrificing the high-end feel of a luxury hotel. The interface utilizes generous whitespace, a refined color palette, and subtle depth to guide the user through complex workflows such as room allocation, guest check-ins, and revenue management.

## Colors
The palette is anchored by a deep **Executive Blue** (`#003580`) to convey stability and authority. A **Hospitality Gold** (`#FEBB02`) is used sparingly as a secondary accent to highlight premium features or high-priority calls to action, evoking a sense of luxury.

Functional colors are critical for property management:
- **Success Emerald** is used exclusively for confirmed bookings and room availability.
- **Warning Amber** denotes pending actions or tentative reservations.
- **Room Status Grays** differentiate between service states (Clean, Dirty, Out of Order) without competing with actionable UI elements.
- The neutral scale uses cool-toned grays to maintain a crisp, professional atmosphere.

## Typography
This design system employs a dual-font strategy. **Montserrat** is used for headings to provide an authoritative, geometric structure that feels modern and architectural. **Inter** is utilized for all body text, data tables, and interface labels to ensure maximum legibility at small sizes, which is essential for dense property management dashboards.

Hierarchical rules:
- Use **Display** sizes only for dashboard overviews (e.g., Today's Occupancy).
- **Label-md** should be uppercase when used for table headers.
- **Status-badge** typography is optimized for high-contrast visibility within small UI containers.

## Layout & Spacing
The layout uses a **12-column fluid grid** for desktop, transitioning to a **4-column grid** for mobile. A strict 8px base unit (the "Step") governs all spatial relationships.

- **Dashboards:** Use a "Master-Detail" pattern. The left sidebar remains fixed at 260px, while the main content area expands.
- **Data Tables:** Utilize compact vertical spacing (8px cell padding) to maximize information density for room lists.
- **Modals:** Centered with a maximum width of 600px, utilizing `stack-lg` for internal padding to maintain a spacious, high-end feel.

## Elevation & Depth
Depth is conveyed through **Tonal Layering** supplemented by **Ambient Shadows**. 

- **Level 0 (Surface):** The main background uses the neutral `#F5F5F5`.
- **Level 1 (Cards):** White containers with a very soft, diffused shadow (`0px 4px 12px rgba(0,0,0,0.05)`) to create a subtle lift.
- **Level 2 (Popovers/Dropdowns):** A more defined shadow with a slight blue tint (`rgba(0, 53, 128, 0.1)`) to separate interactive layers from the content.
- **Interactive States:** Buttons use a slight inset shadow on press to mimic a physical "click" feel, reinforcing the professional tactile nature of the system.

## Shapes
The shape language is defined by a **Rounded** (8px to 16px) corner radius. This softens the "industrial" feel of the HMS data, making the software feel more approachable and aligned with the service-oriented nature of hospitality.

- **Small Components (Buttons, Inputs):** 8px radius.
- **Medium Components (Cards, Modals):** 12px radius.
- **Status Badges:** Fully rounded (pill-shaped) to distinguish them from interactive buttons.

## Components
### Interactive Calendars
The centerpiece of the HMS. Use a low-contrast grid. Available rooms are white; occupied rooms use the Primary Blue. Tentative bookings use a striped background pattern with Warning Amber.

### Data Tables
Tables must feature "Sticky Headers." Use alternating row stripes (Zebra striping) using the lightest neutral gray. Actions (Edit/View) should be represented by subtle ghost buttons that appear on hover.

### Status Badges
High-contrast indicators for room status:
- **Clean:** Emerald background with white text.
- **Dirty:** Light gray background with Charcoal text.
- **Out of Order:** Deep charcoal background with white text.

### Buttons
- **Primary:** Solid `#003580` with white text.
- **Secondary:** Outlined `#003580` with 1.5px border.
- **Luxury Action:** Solid `#FEBB02` with `#003580` text (used for "Upsell" or "VIP Check-in").

### Input Fields
Fields should have a 1px border in a medium-gray, which thickens and changes to Primary Blue on focus. Labels are always positioned above the field for clarity in fast-paced data entry.