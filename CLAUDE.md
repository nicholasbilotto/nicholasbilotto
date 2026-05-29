# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is the GitHub profile repository (`nicholasbilotto/nicholasbilotto`). The `README.md` is rendered automatically on Nicholas's GitHub profile page at `github.com/nicholasbilotto`. There is no build system, test suite, or package manager — this is a content repository.

## Files

- `README.md` — GitHub profile display page. Linked projects point to external repos.
- `Resume.md` — Markdown resume, linked from the profile README.
- `Resume.html` — Styled HTML resume intended for browser/PDF viewing. This is the canonical visual resume.

**Keep `Resume.md` and `Resume.html` in sync.** When updating one, update the other. The HTML version is the source of truth for visual design; the Markdown version should match its content.

## Design System (`Resume.html`)

The HTML resume uses a dark, premium aesthetic defined via CSS custom properties:

```css
--color-bg: #08090a          /* page background */
--color-surface: #0f1011     /* card/section base */
--color-brand: #5e6ad2       /* accent blue-purple */
--color-accent: #7170ff      /* hover state */
--color-text-primary: #f7f8f8
--color-text-secondary: #d0d6e0
--color-text-tertiary: #8a8f98
```

Typography: **Inter** for body, **JetBrains Mono** for dates/metadata. Max content width is `800px`.

When adding new sections or components to the HTML resume, follow the existing card pattern (`.project-card`) and section structure. Do not introduce inline styles — use the existing CSS variables.

## Content Conventions

- Voice is first-person, confident, and direct. Avoid corporate filler language.
- The design philosophy is "Presence Over Noise" — concise, high-signal content over exhaustive lists.
- Nicholas's technical focus: MERN stack, Next.js, React Native/Expo, Python data tools.
- Lohmont is his software development company (founded 2024).
