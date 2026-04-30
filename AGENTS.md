# AGENTS.md

## Project Type
Board game design project. **No code is written here.** All output is Markdown suitable for a rulebook or design document.

## Critical Constraint
Do not write or suggest code. If an task feels like it needs code, clarify with the user first.

## Relevant Instruction Files
- `.github/copilot-instructions.md` — project role and constraints (always read first)
- `skills/game-design/SKILL.md` — procedures for rules editing, content creation, and balance review

## Document Structure
- `docs/rulebook/` — canonical rules (entry: `Rule-book.md`)
- `docs/content/` — hero cards, items, tokens, components
- `docs/production/` — layout specs, art direction, print prep
- `docs/reference/` — glossary, change log, links
- `assets/` — art files organized by type (board/, cards/, tokens/, exports/)
- `templates/` — authoring templates for heroes, items, components, scenarios

## Content Entry Points
- Rulebook: `docs/rulebook/Rule-book.md`
- Mechanics: `docs/rulebook/mechanics/Mechanics.md`
- Hero roster: `docs/content/heroes/roster.md`
- Item list: `docs/content/items/items.md`
- Token reference: `docs/content/components/tokens.md`

## Workflow Conventions
- **Rules edits**: read relevant section of `Rule-book.md`, match existing style (H2 for sections, H3 for subsections, Markdown tables for stats)
- **New heroes/items**: use templates in `templates/` (hero-template.md, item-template.md)
- **Balance reviews**: compare against existing roster; flag outliers with specific numerical adjustments
- When in doubt about formatting, check the existing document you're editing before inferring

## Design Principles
- Keep mechanics accessible but strategically deep
- Honour Dota 2 identity: lanes, creeps, gold/XP economy, towers, asymmetric heroes
- Every rule should resolve unambiguously during play
- Use established Dota 2 vocabulary (CS, last hit, deny, BKB, TP, gank)