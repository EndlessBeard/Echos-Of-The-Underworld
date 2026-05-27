# Echoes from the Underworld
## Homepage Wireframe Specification (Desktop + Mobile)

Date: April 23, 2026  
Clients: Rachel and Laura  
Design and Development Lead: Dave

## 1. Purpose

Define the homepage layout as an implementation-ready wireframe spec with:
- Desktop block structure
- Mobile block structure
- Exact component order per block
- Reusable component system

This spec translates the planning notes into a cohesive, buildable page architecture.

## 2. Experience Goals

- Immediate clarity: who this is, what it offers, and where to start.
- Emotional alignment: elegant, grounded, transformational, underworld-inspired.
- Fast action paths: listen, subscribe, book, shop.
- Scannable on mobile, rich on desktop.

## 3. Breakpoints and Layout System

## 3.1 Breakpoints
- Mobile: 320 to 767 px
- Tablet: 768 to 1023 px
- Desktop: 1024 px and up
- Max content width: 1280 px

## 3.2 Grid
- Desktop: 12-column grid, 24 px gutters, 72 to 96 px side padding
- Tablet: 8-column grid, 20 px gutters, 32 px side padding
- Mobile: 4-column fluid grid, 16 px gutters, 16 px side padding

## 3.3 Vertical Rhythm
- Desktop section spacing: 96 to 128 px
- Mobile section spacing: 56 to 80 px
- Card internal spacing: 16 to 24 px

## 4. Global Component Inventory

Use these component IDs in design files and dev tickets.

- C01: Sticky header shell
- C02: Primary nav links
- C03: Utility CTA buttons (Listen, Book, Join)
- C04: Hero media frame (image/video/slideshow)
- C05: Hero brand lockup
- C06: Section title block
- C07: Episode card
- C08: Person profile card
- C09: Inline signup form
- C10: Resource card
- C11: Service card
- C12: Product card
- C13: Modal shell
- C14: Footer link group
- C15: Legal/disclaimer block

Design note: Content cards and pill-style containers should use lightly contrasting 4px borders with approximately 80% background opacity to preserve depth while remaining grounded and subtle.

## 5. Homepage Block Order (Canonical)

This order is required on both desktop and mobile unless approved otherwise.

1. Header
2. Hero: Watch and Connect
3. Mission Snapshot
4. Latest Podcast Episodes
5. About Rachel and Laura
6. Blog and Newsletter
7. Resources
8. Services
9. Shop and Merch
10. Contact CTA band
11. Footer

## 6. Desktop Wireframe Spec

## 6.1 Desktop Map (High-Level)

```text
--------------------------------------------------------------
| D01 Sticky Header                                           |
--------------------------------------------------------------
| D02 Hero: Brand + Media + Primary Actions                  |
--------------------------------------------------------------
| D03 Mission Snapshot                                        |
--------------------------------------------------------------
| D04 Latest Episodes (3-5 cards)                            |
--------------------------------------------------------------
| D05 About (2 profile columns)                              |
--------------------------------------------------------------
| D06 Blog + Newsletter split                                |
--------------------------------------------------------------
| D07 Resources (cards + modal trigger)                      |
--------------------------------------------------------------
| D08 Services (3 cards + booking CTA)                       |
--------------------------------------------------------------
| D09 Shop (featured 4-6 products)                           |
--------------------------------------------------------------
| D10 Contact CTA Band                                        |
--------------------------------------------------------------
| D11 Footer + Disclaimer                                    |
--------------------------------------------------------------
```

## 6.2 Block-by-Block Specs (Desktop)

### D01 Header (Sticky)
- Height: 72 px
- Grid span: full width
- Component order:
1. C01 header shell
2. C05 mini brand mark
3. C02 nav links (Home, Podcast, About, Resources, Services, Shop, Contact)
4. C03 utility CTAs (Listen Now, Book, Join)

### D02 Hero: Watch and Connect
- Height: 78 to 88 vh
- Layout: 7/5 split on 12-column grid
- Left (7 cols) component order:
1. C05 brand lockup
2. One-line value statement
3. Primary CTA row (Listen, Join Email)
4. Secondary CTA row (Services, Shop)
- Right (5 cols) component order:
1. C04 hero media frame
2. Platform icon links (YouTube, Spotify, Apple)
3. Social links

### D03 Mission Snapshot
- Height: auto (min 240 px)
- Layout: centered copy band
- Component order:
1. C06 section title block (Mission)
2. 2 to 4 sentence mission copy
3. Value chips (Authentic, Grounded, Intuitive)

### D04 Latest Podcast Episodes
- Height: auto
- Layout: heading row + 3 to 5 cards
- Component order:
1. C06 section title block
2. Episode list container
3. C07 episode cards (newest to oldest)
4. View All Episodes button (opens C13 Podcast Modal)

### D05 About Rachel and Laura
- Height: auto
- Layout: two equal columns
- Component order:
1. C06 section title block
2. C08 profile card (Rachel)
3. C08 profile card (Laura)
4. Shared perspective statement
5. Contact trigger

### D06 Blog and Newsletter
- Height: auto
- Layout: 6/6 split
- Left (blog preview) order:
1. C06 section title block
2. Most recent post card
3. Read blog archive button
- Right (newsletter) order:
1. Newsletter value statement
2. C09 inline signup form
3. Privacy microcopy

### D07 Resources
- Height: auto
- Layout: 3-column card grid
- Component order:
1. C06 section title block
2. C10 resource cards
3. Explore All Resources button (opens C13 Resources Modal)

### D08 Services
- Height: auto
- Layout: 3 service cards in row
- Component order:
1. C06 section title block
2. C11 service card (Speaking)
3. C11 service card (Readings)
4. C11 service card (Coaching)
5. Book a Service CTA (opens C13 Booking Modal)

### D09 Shop and Merch
- Height: auto
- Layout: 4-up product grid
- Component order:
1. C06 section title block
2. C12 product cards (4 to 6 featured)
3. Visit Full Shop CTA (opens C13 Shop Modal or external)

### D10 Contact CTA Band
- Height: 180 to 240 px
- Layout: centered single column
- Component order:
1. Direct invite headline
2. Contact button
3. Email link

### D11 Footer
- Height: auto
- Layout: 3-column footer + legal row
- Component order:
1. Brand micro statement
2. C14 platform/social links
3. C14 quick nav links
4. C15 legal + disclaimer block

## 7. Mobile Wireframe Spec

## 7.1 Mobile Map (High-Level)

```text
---------------------------------------
| M01 Compact Sticky Header            |
---------------------------------------
| M02 Hero (stacked)                   |
---------------------------------------
| M03 Mission Snapshot                 |
---------------------------------------
| M04 Latest Episodes (vertical cards) |
---------------------------------------
| M05 About (stacked profiles)         |
---------------------------------------
| M06 Blog then Newsletter             |
---------------------------------------
| M07 Resources (horizontal scroll)    |
---------------------------------------
| M08 Services (stacked cards)         |
---------------------------------------
| M09 Shop (2-up then 1-up fallback)   |
---------------------------------------
| M10 Contact CTA                      |
---------------------------------------
| M11 Footer + Disclaimer              |
---------------------------------------
```

## 7.2 Block-by-Block Specs (Mobile)

### M01 Header (Sticky)
- Height: 60 px
- Component order:
1. Brand mark
2. Menu button
3. Quick action icon (Listen)

### M02 Hero (Stacked)
- Height: auto (min 72 vh)
- Component order:
1. Brand lockup
2. Value statement
3. Primary CTA row
4. Hero media frame
5. Platform links
6. Social links

### M03 Mission Snapshot
- Component order:
1. Mission heading
2. Mission copy
3. Value chips (wrap to multiple lines)

### M04 Latest Episodes
- Component order:
1. Section heading
2. C07 episode cards stacked vertically
3. View All Episodes button

### M05 About Rachel and Laura
- Component order:
1. Section heading
2. Rachel profile card
3. Laura profile card
4. Shared perspective statement
5. Contact button

### M06 Blog and Newsletter
- Component order:
1. Blog heading
2. Most recent post card
3. Newsletter heading
4. C09 signup form

### M07 Resources
- Component order:
1. Section heading
2. Resource cards (horizontal scroll rail)
3. Explore All button

### M08 Services
- Component order:
1. Section heading
2. Speaking card
3. Readings card
4. Coaching card
5. Book button

### M09 Shop and Merch
- Component order:
1. Section heading
2. Product cards (2-up grid, collapse to 1-up under 360 px)
3. Visit Full Shop button

### M10 Contact CTA
- Component order:
1. CTA headline
2. Contact button
3. Email link

### M11 Footer
- Component order:
1. Social/platform links
2. Quick nav links
3. Legal/disclaimer block

## 8. Modal and Overlay Order

Modal stack priority:
1. Navigation drawer (mobile)
2. Podcast archive modal
3. Resources modal
4. Booking modal
5. Shop modal

Modal requirements:
- Focus trap on open
- Escape key closes
- Overlay click closes
- Body scroll lock while open

## 9. Visual Progression Rules

- Use subtle section tone shifts to suggest underworld descent.
- Keep text contrast consistent and accessible.
- Preserve a simple, elegant feel (low visual noise).
- Keep animation minimal: soft reveal, subtle parallax optional.

## 10. Content Priority Rules

If space is constrained, preserve this order:
1. Listen path
2. Trust building (About)
3. Conversion path (Services)
4. Secondary growth (Blog/Resources)
5. Shop

## 11. Implementation Handoff Checklist (Dave)

- Build section wrappers in canonical order.
- Implement shared components C01 to C15.
- Apply breakpoint behavior exactly as specified.
- Verify mobile tap targets and spacing.
- Add semantic headings for SEO structure.
- Apply lightly contrasting 4px borders and 80% opacity surface treatments to content containers, cards, and pill elements.
- Add legal/disclaimer content in footer.
- QA: iPhone SE width, common Android width, iPad portrait, desktop.

## 12. Client Sign-Off Items (Rachel and Laura)

1. Confirm hero media direction (static, slideshow, or short loop).
2. Approve exact section order and naming.
3. Confirm launch scope for Blog, Resources depth, and Shop readiness.
4. Approve disclaimer language.

---

This file is now the homepage wireframe specification source of truth for design and build execution.