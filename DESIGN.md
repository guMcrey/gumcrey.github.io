# Design System

## Existing Visual Theme

A quiet document page for someone reading privacy information on a phone in ordinary daylight. Preserve the light theme and restrained green accents from `policy.css`.

## Colors

Use the existing OKLCH variables in `policy.css`: `--paper`, `--surface`, `--ink`, `--muted`, `--green`, `--line` and `--focus`. Do not introduce a second palette for Tiro Total.

## Typography

Keep the existing local system-font stack. Body text is 16px with generous line height; headings use scale and weight contrast. The article is capped at 72ch.

## Layout and Components

Reuse `.site-header`, `.brand`, `.language-switch`, `.page-heading`, `.reading-layout`, `.contents`, `.summary`, `.version-note`, `.permission-list` and `.site-footer`. Desktop has a sticky contents column; phones show contents above the article. Language links use real URLs and `aria-current`.

## Interaction and Accessibility

Keep native links, in-page anchors, visible keyboard focus, the skip link and existing print styles. No animations, modal dialogs, external assets or client-side tracking are required.
