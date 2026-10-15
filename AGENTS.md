# Website improvement instructions for Codex

## Project goal
Improve this existing GitHub Pages website in small, reviewable steps. Preserve the site's recognisable HTML5 UP design language and the author's content while improving responsive behaviour, accessibility, usability, performance, maintainability, and search/social metadata.

## Before making changes
- Inspect the repository structure and identify the actual entry page, stylesheets, scripts, images, fonts, template assets, and any build/deployment configuration.
- Read the existing code and preserve the current architecture unless a change is clearly necessary.
- For a broad request, first give a concise audit and prioritised plan. Do not edit files during an audit-only task.
- Check `git status` before editing. Do not overwrite, discard, or reformat unrelated user changes.
- For changes affecting several pages or core styling, propose a small first milestone before proceeding.

## Visual design constraints
- Preserve the template's core visual identity: typography, palette, content hierarchy, spacing rhythm, imagery, navigation patterns, and overall character.
- Refine and modernise rather than replacing the design with a generic new theme.
- Prefer small, coherent CSS changes and existing project conventions over a full rewrite.
- Do not migrate to React, another framework, a CSS framework, a bundler, or a new component system unless explicitly requested and justified.
- Do not add dependencies or external services without explaining why and asking first.
- Keep existing content, URLs, page names, image paths, navigation destinations, and working interactions unless a change is requested.
- Preserve applicable HTML5 UP attribution and licence notices. If the template's licence or attribution is unclear, flag it rather than removing credits.

## Responsive layout and browser zoom
- Treat browser zoom and user text-size preferences as normal supported ways to use the site; do not try to detect, prevent, or override browser zoom.
- Prefer responsive and fluid CSS: flexible containers, Grid/Flexbox, `max-width`, percentages, `rem`/`em`, and content-driven breakpoints.
- Avoid fixed-width layouts, fixed heights around text, unnecessary absolute positioning, and other choices that cause clipping when text grows.
- Check the layout at approximately 320, 375, 768, 1024, and 1440 CSS pixels wide, and at 200% browser zoom where practical.
- Ensure content reflows without loss of information or functionality; prevent unintended horizontal scrolling, overlapping elements, clipped controls, and unreadable text.
- Ensure images and media scale within their containers and retain sensible aspect ratios.
- Respect `prefers-reduced-motion`; don't add animation merely for decoration.

## Accessibility and quality
- Aim for WCAG 2.2 AA where practical, and call out any issue that cannot reasonably be resolved.
- Use semantic HTML, a logical heading hierarchy, meaningful link text, labels for form controls, useful image alt text, visible keyboard focus, and keyboard-operable interactions.
- Check colour contrast, focus visibility, skip navigation where appropriate, and that content does not rely on colour alone.
- Keep browser-native functionality where it helps accessibility. Do not add ARIA where native HTML already provides the correct semantics.
- Review page titles, descriptions, canonical/preview metadata where appropriate, heading structure, broken links, missing assets, console errors, and loading/performance issues.
- Do not invent page content, personal details, testimonials, statistics, or claims. Ask or flag uncertainty when information is missing.
- Never introduce secrets, API keys, tracking, analytics, cookies, or third-party services without explicit permission.

## Implementation and validation
- Make the smallest coherent change that fulfils the request.
- Before editing, summarise the intended changes when the task is substantial or cross-cutting.
- After editing, inspect the diff and report which files changed and why.
- Run only checks supported by the repository and environment. Do not claim a test passed unless it was actually run.
- If browser testing is available, check representative desktop and mobile widths, keyboard navigation, zoom/reflow, and any changed interactions. Otherwise, provide precise manual testing steps and state what remains unverified.
- Do not silently suppress errors, delete existing features to make tests pass, or make unrelated edits.
- Never commit, push, publish, change GitHub Pages settings, or deploy the site unless the user explicitly asks.

## Working style
- Explain technical choices in beginner-friendly language.
- Separate findings into critical problems, worthwhile improvements, and optional polish.
- Prefer incremental improvements that are easy to review and reverse.
- If requirements conflict, explain the trade-off and favour accessibility, content preservation, and the existing design identity.
