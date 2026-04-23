---
name: Noto
description: A dark, focused note-taking and chat interface by Backboard.io
colors:
  surface: "#1e1e1e"
  surface-raised: "#2a2a2a"
  surface-inset: "#333"
  surface-overlay: "#252525"
  border: "#444"
  border-subtle: "#3a3a3a"
  text: "#e0e0e0"
  text-secondary: "#999"
  text-tertiary: "#777"
  text-muted: "#666"
  accent: "#7c6af7"
  accent-hover: "#6b5ce7"
  on-accent: "#ffffff"
  success: "#4ade80"
  error: "#f87171"
  tag-bg: "#3a2f6b"
  tag-text: "#b8a9f0"
  tag-bg-hover: "#4a3f8b"
  tag-text-hover: "#d4c9ff"
typography:
  h1:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica, Arial, sans-serif"
    fontSize: 1.75rem
    fontWeight: 600
  h2:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica, Arial, sans-serif"
    fontSize: 1.1rem
    fontWeight: 600
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica, Arial, sans-serif"
    fontSize: 0.95rem
    fontWeight: 400
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica, Arial, sans-serif"
    fontSize: 0.85rem
    fontWeight: 500
    letterSpacing: 0.5px
    textTransform: uppercase
  caption:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica, Arial, sans-serif"
    fontSize: 0.75rem
    fontWeight: 400
rounded:
  sm: 6px
  md: 8px
  lg: 10px
  xl: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 20px
  2xl: 24px
  3xl: 30px
  4xl: 40px
components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.on-accent}"
    rounded: "{rounded.md}"
    padding: "12px"
  button-primary-hover:
    backgroundColor: "{colors.accent-hover}"
  button-outline:
    backgroundColor: "transparent"
    borderColor: "{colors.border}"
    textColor: "{colors.text-secondary}"
    rounded: "{rounded.md}"
  button-outline-hover:
    borderColor: "{colors.accent}"
    textColor: "{colors.text}"
  card:
    backgroundColor: "{colors.surface-inset}"
    borderColor: "{colors.border-subtle}"
    rounded: "{rounded.md}"
  input:
    backgroundColor: "{colors.surface-inset}"
    borderColor: "{colors.border}"
    textColor: "{colors.text}"
    rounded: "{rounded.md}"
  input-focus:
    borderColor: "{colors.accent}"
  message-user:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.on-accent}"
    rounded: "{rounded.lg}"
  message-assistant:
    backgroundColor: "{colors.surface-inset}"
    textColor: "{colors.text}"
    borderColor: "{colors.border-subtle}"
    rounded: "{rounded.lg}"
---

## Overview

Noto is a focused, dark-mode interface for saving notes and chatting with an AI assistant. The design philosophy is "distraction-free productivity" — a deep charcoal workspace with a single violet accent that guides the eye to actionable elements.

## Colors

The palette is built on a dark surface hierarchy with one vibrant accent.

- **Surface (#1e1e1e):** The deepest layer — app background and body.
- **Surface Raised (#2a2a2a):** Cards, panels, headers, and modal shells.
- **Surface Inset (#333):** Input fields, message backgrounds, and note cards.
- **Surface Overlay (#252525):** Subtle overlays like the tag filter bar.
- **Text (#e0e0e0):** Primary readable text on dark surfaces.
- **Text Secondary (#999):** Labels, captions, and inactive states.
- **Text Tertiary (#777):** Timestamps and metadata.
- **Text Muted (#666):** Hints and the least important information.
- **Accent (#7c6af7):** The signature Backboard violet. Used for primary buttons, active tabs, user message bubbles, and interactive highlights.
- **Accent Hover (#6b5ce7):** A slightly deeper violet for hover states.
- **Success (#4ade80):** Green for confirmation messages.
- **Error (#f87171):** Red for destructive actions and errors.

## Typography

All type uses the system sans-serif stack for maximum performance and native feel. The scale is tight and utilitarian.

- **H1 (1.75rem / 600):** Gate screen title.
- **H2 (1.1rem / 600):** Panel headers, modal titles.
- **Body (0.95rem / 400):** Chat messages, note content, inputs.
- **Label (0.85rem / 500):** Form labels and section headers, uppercase with letter-spacing.
- **Caption (0.75rem / 400):** Timestamps, meta, small badges.

## Layout

- App padding: 30px on mobile, 12px internal grid gap on desktop.
- Desktop layout: 3-column grid (280px / 1fr / 300px) with 12px gaps.
- Mobile layout: Stacked tab panels with a bottom tab bar.
- History panel: 320px wide slide-out drawer.
- Settings modal: 520px wide centered dialog.

## Elevation & Depth

Depth is expressed through surface color rather than shadows.

- Modal overlay: `rgba(0,0,0,0.6)` backdrop.
- History overlay: `rgba(0,0,0,0.5)` backdrop.
- Panels sit on Surface, cards on Surface Raised, inputs on Surface Inset.

## Shapes

- Small: 6px (buttons, icon buttons, tags)
- Medium: 8px (inputs, cards, tabs)
- Large: 10px (panels, app header)
- XL: 12px (modals)
- Full: 9999px (pills, filter chips)

## Components

### Buttons
- **Primary:** Accent background, white text, 8px radius, 12px padding. Hover lightens opacity.
- **Outline:** Transparent background, border color, secondary text. Hover adds accent border.
- **Icon:** 32x32 square, 8px radius, transparent background, bordered.

### Inputs
- Background: Surface Inset, border: Border color, text: Text color.
- Focus: Accent border.

### Messages
- **User:** Accent background, white text, rounded bubble with sharp bottom-right corner.
- **Assistant:** Surface Inset background, text color, subtle border, sharp bottom-left corner.

### Cards
- Background: Surface Inset, border: Border Subtle, 8px radius.
- Hover: Accent border color.

### Tags
- Background: Deep violet (#3a2f6b), text: Light violet (#b8a9f0).
- Hover: Brighter violet background and text.

## Do's and Don'ts

- **Do** use the accent color sparingly — only for primary actions and the user's own messages.
- **Do** rely on surface layers to create hierarchy without drop shadows.
- **Don't** introduce additional accent colors; the violet is the brand signature.
- **Don't** use pure black or pure white — the dark greys and soft off-whites reduce eye strain.
