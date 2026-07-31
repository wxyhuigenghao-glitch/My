# design.spec.md

## Premium Creative Marketplace Light Design System

Theme: Light Mode / Editorial / Creative Commerce

## Visual Language

- Soft white background
- Large editorial typography
- Floating artwork cards
- Rounded surfaces
- Minimal navigation
- Soft shadows
- Elegant motion

## Color Tokens

```yaml
background:
  primary: "#F8F8F6"
  surface: "#FFFFFF"

text:
  primary: "#111111"
  secondary: "#555555"
  muted: "#8A8A8A"

accent:
  mint: "#65CDB2"
  blue: "#4268FF"
  yellow: "#F4C84A"
  coral: "#F46A54"

shadow:
  soft: "0 20px 60px rgba(0,0,0,0.08)"
```

## Typography

Hero headings are the primary visual anchor.

```css
font-size: clamp(48px,6vw,88px);
font-weight:500;
letter-spacing:-0.05em;
```

## Layout

Hero sequence:

1. Floating navbar
2. Large headline
3. Artwork gallery
4. Description
5. CTA

## Artwork Card Rules

- Rounded corners
- Overlapping composition
- Different rotation angles
- Soft shadow
- Hover elevation

## Components

BEM naming:

.hero
.hero__title
.hero__gallery
.art-card
.navbar
.button
.tag

## Motion

Use slow premium transitions:
- fade
- floating
- subtle scale

Respect prefers-reduced-motion.

## Responsive

Desktop:
- Full gallery composition

Mobile:
- Stack content
- Reduce artwork overlap
- Collapse navigation

## Accessibility

- WCAG AA contrast
- Keyboard focus
- 44px touch targets
- Reduced motion support
