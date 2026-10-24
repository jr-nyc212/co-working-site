# WeBarelyWork – Coworking Listings Page

A mobile-first landing page for a fictional coworking brand, built from a
Scrimba design spec: a dark nav bar, a bold heading, three full-width photo
cards with captions and booking buttons, and a floating chat button. Each
lesson became its own issue, branch and pull request, so the commit history
doubles as a log of the changes.

**Live site:** https://co-working-site.netlify.app

## What was built

- **Layout from a design spec.** Translated the colour, font, size and
  margin values from the design slide into CSS, with Montserrat from Google
  Fonts and `rem` units for type.
- **Flexbox nav.** Logo, location pin and burger menu in one row, with an
  auto margin pushing the menu to the far right while the rest stay put.
- **Responsive images.** Full-width photos that scale to any screen using
  percentage widths and a viewport meta tag.
- **Positioned overlay.** An "Exclusive" banner pinned to the top-left of
  the first photo with relative and absolute positioning.
- **Caption rows.** Text and a Book button at opposite ends of each caption,
  with a flex gap that keeps at least 20px between them on narrow screens.
- **Fixed chat button.** A circular button anchored to the bottom-right
  corner of the window, with the icon centred using flex and auto margins.

## Run it locally

```
npm install
npm run dev
```

Vite serves the page at http://localhost:5173.

## Built with

HTML, CSS and Vite. No frameworks.

## Course

Built while working through Scrimba's
[Fullstack Developer Path](https://scrimba.com/fullstack-path-c0fullstack).
The starter code is Scrimba's; the styling and layout are mine.
