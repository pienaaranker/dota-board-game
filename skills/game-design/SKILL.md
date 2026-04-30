---
name: game-design
description: "Board game design and rules editing for the Dota 2–inspired board game. Use when: designing or balancing mechanics; drafting hero cards, Abilities Cards, planning tokens, or item cards; editing or expanding Rule-book.md; creating supporting documents (hero rosters, item lists, scenario guides); proposing new game modes; resolving rules inconsistencies; playtesting analysis or balance feedback."
argument-hint: "Describe what you want to design, add, or balance (e.g. 'hero Abilities Card for a support hero', 'jungle camp rules', 'item shop economy')"
---

# Game Design Skill

## Purpose
Assist with all board game design tasks for the Dota 2–inspired board game. This covers rules writing, content creation, mechanical balance, and documentation structure.

## When to Use
- Drafting or editing sections of `Rule-book.md`
- Creating new hero cards, Abilities Cards, planning tokens, or item cards
- Designing new mechanics (e.g. Roshan, Runes, Buyback)
- Writing supporting documents: hero rosters, item lists, scenario guides
- Balancing stats, costs, and effects across heroes and items
- Resolving ambiguities or contradictions in existing rules
- Proposing new game modes or optional rule variants

## Procedure

### For Rules Editing
1. Read the relevant section(s) of `Rule-book.md` for context
2. Identify the formatting conventions in use (tables, headers, bullet lists)
3. Draft the addition or change, matching the existing style
4. Flag any interactions with other rules that may need updating

### For New Content (Heroes, Items, Abilities)
1. Reference comparable existing content for stat and cost calibration
2. Apply Dota 2 thematic identity: mana costs, cooldowns, gold values, stat ranges
3. Format using Markdown tables consistent with the rulebook
4. Note any new tokens, counters, or components the content requires

### For Balance Review
1. Compare the proposed content against the existing roster or item pool
2. Identify outliers (too strong, too weak, too complex)
3. Suggest specific numerical adjustments with reasoning

## Document Conventions
- Main rules: `Rule-book.md`
- Hero rosters: `heroes/` folder
- Item lists: `items/` folder
- Scenario and game mode guides: `scenarios/` folder
- Use H2 (`##`) for top-level sections, H3 (`###`) for subsections
- Stats and ability descriptions go in Markdown tables

## Design Principles
- Keep mechanics accessible but strategically deep
- Honour Dota 2 identity: asymmetric heroes, comeback mechanics, map pressure
- Every rule should resolve unambiguously during play
- Prefer established Dota 2 vocabulary (CS, Last Hit, Deny, BKB, TP, Gank)
