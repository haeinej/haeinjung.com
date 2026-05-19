# HaeinJung.com Current Style Guide

Use this file when creating or revising pages for `haeinjung.com`.

## Reuse Prompt

Apply the current HaeinJung.com editorial style: flat navy archive pages, white editorial reader pages, Instrument Sans throughout, no grid textures, no decorative waves on writing pages, clean custom cursor, small readable typography, and quiet categorized structure. Keep the writing index compact and Substack-like, while individual essays and whitepapers use the white reader template with progress bar.

## Global Identity

- Brand voice: calm, precise, reflective, intellectual, slightly intimate.
- Primary font: `Instrument Sans`.
- Avoid wavy/decorative font treatment except where an existing homepage interaction explicitly uses it.
- Letter spacing should be `0` for readable titles and article text. Uppercase metadata may use wide tracking.
- Avoid grid backgrounds, texture overlays, decorative blobs, and card-heavy layouts.
- Keep the site feeling flat, clean, and editorial.

## Colors

- Main navy background: `#050914`.
- White reader paper: `#fbfaf7`.
- Reader ink: `#17130f`.
- Dark-page ink: `#f5f1e8`.
- Muted text on white: `rgba(23, 19, 15, 0.68)`.
- Muted text on navy: `rgba(245, 241, 232, 0.72)`.
- Soft dividers on white: `rgba(23, 19, 15, 0.14)`.
- Soft dividers on navy: `rgba(245, 241, 232, 0.12)`.

## Writing Index

- File: `writing/index.html`.
- Background: flat navy.
- Do not use a scroll progress bar on the index.
- Do not include wave/photo/profile hero elements on the writing index.
- Use a compact archive structure with categorized sections.
- Current categories:
  - Latest
  - Whitepaper
  - AI + Design
  - Becoming
- The intro copy should stay small and quiet, not hero-marketing scale.
- Current intro: `A slower index of what I am noticing: from technology to trivial frictions and beauty that make thinking feel alive.`
- Article titles on the index are compact:
  - `font-size: clamp(1.05rem, 1.55vw, 1.36rem)`
  - `line-height: 1.16`
- Article subtitles:
  - `font-size: 0.9rem`
  - `line-height: 1.55`
- The index should not include an external directory section like `Elsewhere`.

## Reader Pages

- Use for essays and whitepapers.
- Background: white editorial paper, `#fbfaf7`.
- Include:
  - sticky reader topbar
  - reading progress bar
  - back link to `/writing/`
  - custom cursor
- Body font: `Instrument Sans`.
- Body type:
  - `font-size: clamp(0.95rem, 1.1vw, 1.06rem)`
  - `line-height: 1.66`
- Title type:
  - `font-size: clamp(2rem, 5vw, 4.1rem)`
  - `line-height: 0.92`
  - `font-weight: 600`
  - `letter-spacing: 0`
- Mobile reader title:
  - `font-size: clamp(2.15rem, 12vw, 3.35rem)`
- Mobile body:
  - `font-size: 0.95rem`
- Section headings:
  - `font-size: clamp(1rem, 1.8vw, 1.32rem)`
  - `font-weight: 600`
  - `letter-spacing: 0`

## Cursor

- Every page with a custom cursor should use the shared healthy cursor behavior block.
- Cursor element:
  - `<div class="site-cursor" aria-hidden="true"></div>`
- Use `mix-blend-mode: difference` so the circle works on both navy and white pages.
- The cursor should be enabled only for `(hover: hover) and (pointer: fine)`.
- One cursor element per page, one active cursor script per page.

## Social Links

The visible social set should be:

- X: `https://x.com/haeinjvng_`
- Instagram: `https://www.instagram.com/haeinjvng/`
- LinkedIn: `https://www.linkedin.com/in/haein-jung-a8441a304/`
- Substack: `https://haeinej.substack.com/`

Do not show Naver in the visible site directory/social set.

## Publishing Notes

- Work from the clean deployment worktree when possible.
- Keep changes focused to the requested pages.
- After editing, verify:
  - writing index has no `Elsewhere`, Naver, or stale directory links
  - reader pages have white background, progress bar, and cursor
  - GitHub Pages deploy completes successfully
