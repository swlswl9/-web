---
name: Your Wave Portfolio
description: A blue-and-white sticker-poster portfolio where the supplied artwork leads.
colors:
  wave-blue: "#5c92e0"
  ink: "#101b35"
  paper: "#f6f5f0"
  mist: "#e6e9ed"
  signal-lime: "#dfff38"
typography:
  display:
    fontFamily: "Barlow Condensed, Impact, sans-serif"
    fontSize: "clamp(5.2rem, 11.5vw, 12.2rem)"
    fontWeight: 900
    lineHeight: 0.73
    letterSpacing: "-0.045em"
  body:
    fontFamily: "Archivo, Arial, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.65
rounded:
  pill: "999px"
  sticker: "50%"
spacing:
  compact: "0.55rem"
  control: "0.85rem"
  section: "clamp(5rem, 10vw, 9rem)"
components:
  nav-shell:
    backgroundColor: "{colors.wave-blue}"
    textColor: "{colors.paper}"
    rounded: "{rounded.pill}"
    padding: "0.7rem 0.85rem 0.7rem 1.05rem"
  contact-button:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.wave-blue}"
    rounded: "{rounded.pill}"
    padding: "0.72rem 1.05rem"
  tool-chip:
    textColor: "{colors.wave-blue}"
    rounded: "{rounded.pill}"
    padding: "0.6rem 0.85rem"
---

# Design System: Your Wave Portfolio

## Overview

**Creative North Star: "The Blue Sticker Poster"**

This is a cool-paper portfolio rebuilt directly from the supplied blue-and-white homepage composition. The original paper texture, oversized pale SWL lettering, central dimensional sticker, blue rails, editorial copy, and low-positioned SEE MORE action are preserved as the visual authority.

The main visual energy comes from the artifact, scale, and controlled movement. There is no ambient video: the supplied paper-texture SVG is the full background while the central sticker gets one restrained floating motion. The sections simplify as visitors move from introduction to work and contact.

**Key Characteristics:**
- Cobalt blue and paper carry the surface; lime is a brief signal, not a second brand.
- Condensed display type is cropped, oversized, and assertive.
- Paper texture and artwork shadow provide material depth.
- Motion is buoyant and intentional, with a reduced-motion escape hatch.

## Colors

The palette is a committed blue field with paper contrast and one high-voltage lime signal.

### Primary

- **Wave Blue:** the persistent studio blue used for hero type, navigation, and the work field.
- **Signal Lime:** used sparingly for calls to action, orbit details, and active emphasis.

### Neutral

- **Cool Paper:** the readable base surface and light control fill.
- **Studio Ink:** the near-navy field for services and long-form copy.
- **Studio Mist:** the quiet about-section surface behind large translucent type.

**The One-Signal Rule.** Lime only marks something actionable or moving; it does not become a general decoration.

## Typography

**Display Font:** Barlow Condensed (with Impact fallback)
**Body Font:** Archivo (with Arial fallback)

**Character:** The display face behaves like compressed poster lettering; body copy stays neutral and calmly readable so it does not compete with the artwork.

### Hierarchy

- **Display:** 900 weight, responsive oversized clamp, tight leading; for the hero, section headlines, service names, and email address.
- **Headline:** 900 weight, `clamp(3rem, 5.3vw, 6.2rem)` with compact leading; for major section statements.
- **Body:** 400–600 weight, `1rem` around `1.65` line height; for concise Chinese descriptions.
- **Label:** condensed 800 weight with generous letter spacing; for navigation, service metadata, and small system language.

**The Poster-Then-Reading Rule.** A section gets one dominant display statement; supporting text remains intentionally small and plain.

## Layout

The hero follows the supplied 1366 × 768 composition: paper texture is the base, pale SWL spans the middle field, blue rail sits at the top, editorial copy anchors bottom-left, the dimensional sticker overlaps the center, and SEE MORE sits under a lower divider at right. The MY WORKS section immediately below keeps the supplied full-canvas SVG artwork intact and moves the complete project composition from left to right in a continuous loop; each project has a precisely placed link to its matching long-form image. Skills and about use generous responsive padding.

## Elevation & Depth

Depth is material, not card-like. The supplied sticker artwork carries the dimensional shading; paper texture and flat color fields separate the remaining page.

### Shadow Vocabulary

- **Supplied sticker depth:** inherited within `wangye.svg`; no extra CSS shadow is added over the original art.

## Shapes

Pills belong to navigation, buttons, and skill chips. Circles and irregular rounded loops are reserved for sticker-adjacent geometry. Project surfaces remain square so the artwork, typography, and color blocks feel like posters rather than cards.

## Components

### Buttons

- **Shape:** high-rounded pill (`999px`).
- **Primary:** cool-paper text surface on the wave-blue navigation.
- **Hover / Focus:** a small rotation and scale on hover; lime focus outline with offset for keyboard users.

### Chips

- **Style:** outlined blue skill labels on the mist about surface.
- **State:** static informative tags in the current prototype.

### Navigation

- **Style:** a blue pill shell with paper text and an acid underline on hover.
- **Mobile treatment:** collapses to a labelled two-line menu control and vertical blue menu panel.

### Project Surfaces

- **Corner Style:** square poster fields.
- **Background:** each selected-work tile receives a unique blue, paper, or ink field with abstract CSS geometry.
- **Behavior:** hover lifts the complete visual using transforms only.

### Sticker Stage

Five supplied SVGs form the signature component on one 1366 × 768 canvas: `wangye3.svg` is the paper base, `wangye2.svg` provides the pale oversized SWL layer, `wangye4.svg` supplies the vertical date, `wangye5.svg` supplies the editorial copy, and `wangye.svg` provides the central dimensional sticker. Only the sticker floats slightly; it does not tilt or change the fixed reference layout.

## Do's and Don'ts

### Do:

- **Do** keep the supplied blue-and-white artwork intact and in the visual lead.
- **Do** make every functional accent clear against its background.
- **Do** use transforms and opacity for interactive movement and respect reduced motion.
- **Do** preserve the paper surface and broad empty margins around oversized display type.

### Don't:

- **Don't** replace the hero with a generic grid of matching project cards.
- **Don't** use lime as a base background or introduce unrelated accent colors.
- **Don't** add decorative icons from emoji or mix icon styles.
- **Don't** fabricate personal details, client histories, or project outcomes before they are supplied.
