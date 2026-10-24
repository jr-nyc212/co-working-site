# HISTORY — Co-Working Site

Newest first. One section per shipped milestone.

## [M2 — Polish] — 2026-10-24

Outcome: the project is presentable as portfolio work and live on the web.

- **Head metadata.** Added `lang`, `charset`, and a `<title>` so the page is
  well-formed for browsers, search, and assistive tech.
- **Portfolio README.** Replaced the Scrimba boilerplate with a README that describes
  what was built and links the live site, written to the `/scrimba-readme` pattern.
- **Netlify deploy.** One-off manual deploy of the Vite build to
  https://co-working-site.netlify.app. Deliberately not linked to GitHub so pushes do
  not consume Free-plan deploy credits.
- **Repo metadata.** Description and homepage set on the GitHub repo.

## [M1 — Core] — 2026-10-24 (193ae24..7544211)

Outcome: the page matches the Scrimba design spec on phone and laptop widths.

- **Layout from the design spec** (PR #2). Nav bar colours, Montserrat, h1 and caption
  margins, `rem` type sizes. Images set to `width: 100%` so they scale to any screen,
  plus the viewport meta tag. Flexbox on the `ul` to put the logo and pin in a row.
- **Menu icon at the right** (PR #4). Burger icon added to the nav and pushed to the
  far end with an auto left margin, leaving the logo and pin in place. Header
  background and text colour moved onto `header` and `body`.
- **Exclusive banner** (PR #6). Overlay pinned to the top-left of the first photo with
  `position: relative` on the card and `position: absolute` on the banner.
- **Book buttons** (PR #8). Each caption is a flex row with the text and a Book button
  at opposite ends; `gap: 20px` guarantees the minimum spacing on narrow screens and
  `margin: auto` on the button handles both the push-right and vertical centring.
- **Floating chatbox** (PR #10). Circular button fixed 6px from the bottom-right of the
  window, with the speech-bubble icon centred by `display: flex` on the circle and
  `margin: auto` on the icon.

Decision kept from the course: `display: block` is not set on `.item-img`, matching
Scrimba's solution. Add it if anything ever sits flush against an image's bottom edge.
