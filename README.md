# Dota Board Game

This repository now separates gameplay rules, content libraries, production references, and assets so the project can grow without crowding the top level.

## Structure

- `docs/rulebook/` — Canonical rules and future scenario guides
- `docs/content/` — Heroes, items, tokens, and other game content
- `docs/production/` — Layout specs, art direction, and print-prep notes
- `docs/reference/` — Glossary, links, and project tracking notes
- `assets/` — Board art, card art, icons, token art, diagrams, and export files
- `templates/` — Reusable authoring templates for new design documents
- `archive/` — Legacy or superseded material kept for reference

## Current Entry Points

- Rulebook: `docs/rulebook/Rule-book.md`
- Mechanics reference: `docs/rulebook/mechanics/Mechanics.md`
- Hero designs: `docs/content/heroes/roster.md`
- Hero shortlist: `docs/content/heroes/hero-shortlist.md`
- Items: `docs/content/items/items.md`
- Tokens: `docs/content/components/tokens.md`

## Asset Storage

Store source and export assets by component type rather than by software tool. For example:

- Board renders in `assets/board/`
- Hero art in `assets/cards/heroes/`
- Ability card art in `assets/cards/abilities/`
- Item card art in `assets/cards/items/`
- Print-ready sheets in `assets/exports/print-ready/`