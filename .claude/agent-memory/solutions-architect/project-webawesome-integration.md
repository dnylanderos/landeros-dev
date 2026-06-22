---
name: project-webawesome-integration
description: User is integrating WebAwesome design system into their Astro v6 personal/portfolio site
metadata:
  type: project
---

User wants to add WebAwesome (web component design system built on Shoelace/Lit, from Font Awesome team) to their personal/portfolio Astro v6 site at /Users/danny/dev/landeros-dev.

**Why:** Building out a personal site/portfolio and wants a design system. WebAwesome is framework-agnostic via custom elements — ideal fit for Astro with no JS framework.

**How to apply:** When suggesting component usage, use vanilla web component syntax (`<wa-button>`, etc.), not JSX wrappers. The npm package is `@awesome.me/webawesome`. CDN approach chosen for initial install (see [[feedback-webawesome-cdn-vs-npm]] if a preference was stated later). Main CSS import: `@awesome.me/webawesome/dist/styles/webawesome.css`. Icons load from Font Awesome CDN by default; self-hosting requires `setIconPath()`.
