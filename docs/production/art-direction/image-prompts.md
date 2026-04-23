

---

## Hero Card Style Control System

To keep all generated hero cards consistent while still allowing strong hero identity, use a **3-layer prompt structure**:

1. **Locked System Layer** — the parts that should never change between heroes
2. **Controlled Flavor Layer** — the parts that can change to express the hero's identity
3. **Anti-Drift Layer** — explicit instructions about what the model must not redesign

If these three layers are always present in the prompt, the cards will behave more like a coherent set, similar to a trading card game's frame system, rather than four unrelated poster layouts.

### 1. Locked System Layer

These elements should stay effectively identical across all hero cards:

- Card size and portrait orientation
- Outer frame shape and border treatment
- Name banner position and size
- Class ribbon position
- Attack-type badge position
- Role tag position
- Portrait window position and proportions
- Stat strip position, icon order, and numeric hierarchy
- Progression strip position and milestone icon treatment
- Four-row ability grid structure
- Ability row anatomy: icon medallion, top-line numbers, summary text, scaling line
- Typography system: title font family, rules font family, number emphasis style
- Icon set and icon order
- Divider thickness, corner treatment, and panel spacing
- Overall render angle: always straight-on, flat component view

Think of this layer as the game's **frame template**. The model should not be invited to reinterpret it.

### 2. Controlled Flavor Layer

These elements may change per hero, but only inside the locked frame:

- Portrait artwork
- Accent color palette inside the established card structure
- Hero-specific motif work in the portrait window and subtle background details
- Class-appropriate emblem or hero-specific crest
- Hero atmosphere: frost, moonlight, demonic fire, storm energy, poison, etc.
- Weapon, companion, magic effect, armor style, and silhouette language

This is where the hero gets identity. The layout should stay stable while the **art direction, palette accents, and icon motifs** do the differentiation work.

### 3. Anti-Drift Layer

Every reusable generation prompt should explicitly forbid these kinds of drift:

- redesigning the card frame
- moving major zones around
- changing the stat strip order
- changing the number of ability rows
- replacing the established typography hierarchy
- introducing new decorative badges or UI systems
- changing the card into a poster, splash art, mobile UI, or TCG variant
- turning the card into a 3D mockup or photographed object

### What Should Be Fixed vs Variable

Use this split consistently:

| Fixed Across All Hero Cards | Variable Per Hero |
|---|---|
| Outer border and frame | Portrait art |
| Banner, ribbon, badge, and tag positions | Accent palette |
| Stat icon order | Character motif |
| Progression bar layout | Hero emblem / symbol |
| Ability row layout | Mood and atmosphere |
| Typography system | Magic / weapon / companion visuals |
| Divider style and spacing | Texture details inside portrait area |

### Recommended Prompt Formula

For the most consistent image generation, build hero card prompts in this order:

1. **Base frame instruction**
	- Tell the model to use the Mirana-style hero card system exactly
2. **Locked layout instruction**
	- List the unchanging structural zones
3. **Hero data instruction**
	- Provide stats, class, attack type, and abilities
4. **Flavor instruction**
	- Describe the hero's portrait direction, palette accents, mood, and emblem
5. **Anti-drift instruction**
	- Tell the model what not to redesign

This order matters. If flavor comes too early, the model often starts redesigning the card. If the frame comes first, flavor tends to stay inside the system.

### Recommended Flavor Budget

To prevent hero identity from overwhelming layout consistency, keep the variable layer constrained:

- **1 primary accent palette** per hero
- **1 emblem / symbol family** per hero
- **1 portrait mood** per hero
- **1-2 subtle background motifs** at most

That gives enough uniqueness without causing the frame to mutate.

### Best Practice Prompt Language

When writing hero prompts, prefer wording like:

- `Use the same card architecture, typography, icon order, and panel system as the Mirana example.`
- `Only change the portrait art, accent palette, emblem, and hero-specific flavor details.`
- `Do not redesign the frame or reposition any major card elements.`
- `Keep this visually part of the same manufactured card set.`

Avoid wording like:

- `Create a unique card layout for this hero.`
- `Reimagine the frame to suit the hero.`
- `Make the design match the hero however you think best.`

Those phrases invite inconsistency.

### Manufacturing Mindset

The easiest way to keep the set cohesive is to think like a publisher, not like an illustrator.

- The **card frame** is manufactured and standardized.
- The **hero art and accent treatment** are customized.
- The goal is not four beautiful one-offs.
- The goal is one beautiful card system that many heroes can inhabit.

### Short Master Constraint Block

Add this short block near the end of any reusable hero prompt when consistency matters:

```text
Keep this card in the exact same product family as the Mirana example hero card. Preserve the frame, panel layout, typography hierarchy, icon order, spacing rhythm, and overall card architecture. Only vary the portrait artwork, accent palette, emblem, and hero-specific atmospheric details. Do not redesign the structure.
```

## Example Image Prompt — Crystal Maiden Hero Card

Use the following prompt when generating a sample hero card image for Crystal Maiden:

```text
Create a polished fantasy board game hero card in portrait orientation, designed for a 10 × 15 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the Mirana example hero card. Keep this visually part of the same manufactured hero-card product family.

Overall style: premium tabletop card design, clean information hierarchy, readable at print size, elegant icy magical theme, intelligence-class visual identity, blue and silver palette with frosted glass accents, subtle snowflake patterns, crisp iconography, high contrast text panels, collectible but practical.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, name banner position, class ribbon position, attack-type badge position, role tag position, portrait window position and proportions, stat strip position and icon order, progression strip position, four-row ability grid structure, typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view established by the Mirana example.
- Only change the portrait artwork, accent palette, emblem, and hero-specific atmospheric details inside the established frame.

Card structure:
- Top banner with the name: CRYSTAL MAIDEN
- Intelligence class band in blue
- Attack type badge: Ranged
- Role tags: Support, Nuker, Control
- Large central portrait of Crystal Maiden as an original fantasy frost sorceress: pale winter mage, blue hood and robes, ornate fur-lined mantle, glowing staff, swirling frost magic, composed but dangerous expression, arcane ice energy around her hands
- Horizontal stat strip below portrait with large readable icons and numbers
- Narrow progression strip
- Bottom half contains four compact ability summary rows with chips for unlock level, type, and target only

Base stats to show exactly:
- HP 75
- Mana 50
- Attack 6
- Attack Range 3 hexes
- Defense 1
- Move Speed 1
- AP 10

Progression strip:
- Per Level: +10 HP | +10 Mana | +3 ATK | +1 DEF
- Milestone icons for Level 6, Level 12, Level 18

Ability summary rows to display:

1. Crystal Nova
- Type: Active
- Target: Ground-Targeted AoE
- Unlock: Level 1
- Summary: Blast an area with frost to damage and slow enemies.

2. Frostbite
- Type: Active
- Target: Unit Target
- Unlock: Level 1
- Summary: Root a target in ice and apply damage over time.

3. Arcane Aura
- Type: Passive (Aura)
- Target: Global allied mana regeneration
- Unlock: Level 1
- Summary: Crystal Maiden and allied heroes regenerate mana over time.

4. Freezing Field
- Type: Channeled
- Target: No Target (Self-Cast)
- Unlock: Level 6
- Summary: Channel a massive self-centered ice storm that damages and slows nearby enemies.

Graphic direction:
- The card should feel like a readable tabletop component first, illustration showcase second
- Use clear panel separation and consistent icon chips
- Emphasize frost magic, snow, cold light, crystalline textures, and a calm support-caster identity
- Keep the layout uncluttered and legible; no fake tracker dials, no board-game counters, no 3D mockup angle
- Present as a straight-on flat card render on a neutral background
- Include subtle hex motifs and line-of-sight / range icon language appropriate for a tactical board game

Typography direction:
- Large, elegant fantasy title for the hero name
- Clean, compact sans-serif or highly readable game UI font for rules text
- Important values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the stat strip order, typography hierarchy, or four-row ability layout
- Do not introduce new decorative badges, alternate UI systems, or extra card zones
- Do not turn the card into a poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not print full numerical rules text, costs, cooldowns, or scaling values on the hero card
- Do not copy official game splash art
- Do not use a trading card game frame style
- Do not make it look like a mobile game screenshot
- Do not add extra abilities, extra stats, or extra decorative clutter
- Do not place current HP, current Mana, gold, XP, cooldown trackers, or item slots on the card
```

---

## Example Image Prompt — Magnus Hero Card

Use the following prompt when generating a sample hero card image for Magnus:

```text
Create a polished fantasy board game hero card in portrait orientation, designed for a 10 × 15 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the Mirana example hero card. Keep this visually part of the same manufactured hero-card product family.

Overall style: premium tabletop card design, clean information hierarchy, readable at print size, imposing battlefield-controller theme, strength-class visual identity, crimson, bronze, obsidian, and muted teal force-magic accents, crisp iconography, high contrast text panels, collectible but practical.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, name banner position, class ribbon position, attack-type badge position, role tag position, portrait window position and proportions, stat strip position and icon order, progression strip position, four-row ability grid structure, typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view established by the Mirana example.
- Only change the portrait artwork, accent palette, emblem, and hero-specific atmospheric details inside the established frame.

Card structure:
- Top banner with the name: MAGNUS
- Strength class band in red
- Attack type badge: Melee
- Role tags: Initiator, Disabler, Durable
- Large central portrait of Magnus as an original horned battlefield warlord: towering beast-like frontliner, massive curved horns, heavy bronze armor, rune-scarred polearm or hammer, force magic pulling debris and enemies inward, deliberate and commanding stance
- Horizontal stat strip below portrait with large readable icons and numbers
- Narrow progression strip
- Bottom half contains four compact ability summary rows with chips for unlock level, type, and target only

Base stats to show exactly:
- HP 105
- Mana 35
- Attack 9
- Attack Range 1 hex
- Defense 3
- Move Speed 1
- AP 10

Progression strip:
- Per Level: +12 HP | +8 Mana | +4 ATK | +1 DEF
- Milestone icons for Level 6, Level 12, Level 18
- Scepter badge reminder

Ability summary rows to display:

1. Shockwave
- Type: Active
- Target: Direction/Vector
- Unlock: Level 1
- Summary: Send a force wave that damages enemies, pulls them inward, and slows heroes hit.

2. Empower
- Type: Active
- Target: Unit Target
- Unlock: Level 1
- Summary: Empower an allied hero with bonus Attack and cleaving strikes.

3. Skewer
- Type: Active
- Target: Direction/Vector
- Unlock: Level 1
- Summary: Charge forward, damaging enemy heroes and dragging them with Magnus.

4. Reverse Polarity
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 6
- Summary: Pull nearby enemy heroes together, damage them, and stun them for a massive setup play.

Graphic direction:
- The card should feel like a readable tabletop component first, illustration showcase second
- Use clear panel separation and consistent icon chips
- Emphasize horn silhouette, heavy armor, force-magic distortion, battlefield debris, sweeping momentum, and clustered-enemy control
- Keep the layout uncluttered and legible; no fake tracker dials, no board-game counters, no 3D mockup angle
- Present as a straight-on flat card render on a neutral background
- Include subtle hex motifs and tactical board game icon language for pull effects, forced movement, cones, and area control

Typography direction:
- Large, forceful fantasy title for the hero name
- Clean, compact sans-serif or highly readable game UI font for rules text
- Important values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the stat strip order, typography hierarchy, or four-row ability layout
- Do not introduce new decorative badges, alternate UI systems, or extra card zones
- Do not turn the card into a poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not print full numerical rules text, costs, cooldowns, or scaling values on the hero card
- Do not copy official game splash art
- Do not use a trading card game frame style
- Do not make it look like a mobile game screenshot
- Do not add extra abilities, extra stats, or extra decorative clutter
- Do not place current HP, current Mana, gold, XP, cooldown trackers, or item slots on the card
```

---

## Example Image Prompt — Magnus Abilities Card

Use the following prompt when generating a sample landscape Abilities Card image for Magnus:

```text
Create a polished fantasy board game abilities reference card in landscape orientation, designed for a 15 × 10 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the attached Magnus Hero Card image as the primary visual reference for this Abilities Card. Match its card family exactly: same design language, same frame sensibility, same typography hierarchy, same icon rendering style, same accent palette logic, same material finish, and the same treatment of horned warlord motifs, force-magic distortion, heavy bronze armor, battlefield momentum, and violent displacement effects. The Abilities Card should look like it was manufactured as a companion component to that exact Hero Card, not merely a related card from a similar set.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the established landscape Abilities Card template for this game. Keep this visually part of the same manufactured product family as the attached Hero Card while clearly functioning as a rules reference.

Overall style: premium tabletop reference component, rules-forward layout, highly readable at print size, imposing battlefield-controller theme, strength-class visual identity, crimson, bronze, obsidian, and muted teal force-magic accents, clean dividers, restrained arcane texture, crisp iconography, collectible but practical.

This is an Abilities Card, not a Hero Card. The card should prioritize gameplay clarity, full rules readability, and explicit numerical values over portrait space.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, hero header position, summary strip position, and a four-row stacked ability layout with one ability per horizontal row. Preserve the typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view across all Abilities Cards.
- Derive the small hero portrait or crest, ability icons, accent palette, and hero-specific atmospheric details directly from the attached Hero Card so the spell visuals feel like the same hero package.
- Make the force-wave arcs, cleave motifs, charging momentum lines, clustered pull effects, and heavy battlefield impact language visually consistent with what appears on the attached Hero Card.

Card structure:
- Hero header with the name: MAGNUS
- Small crest or portrait accent
- Summary strip listing Shockwave, Empower, Skewer, Reverse Polarity
- Four clearly separated horizontal ability rows, one per ability, each with icon, type, target, costs, rules text, and scaling
- Upgrade / notes panel for key reminders
- Small footer legend for icon language if needed

Ability data to show exactly:

1. Shockwave
- Type: Active
- Target: Direction/Vector
- Unlock: Level 1
- Mana Cost: 12
- AP Cost: 1
- Cooldown: 2 rounds
- Range: 4 hexes
- Rules: Magnus sends a wave of force in a straight line up to 4 hexes. Enemy units in the path take damage and are pulled 1 hex toward Magnus, if a legal Open hex is available. Enemy heroes hit by Shockwave are also Slowed until the end of their next activation.
- Scaling: 1-5: 16 damage | 6-11: 24 damage | 12+: 32 damage
- Notes: For Shockwave, Slowed means the affected hero's first Move action on their next activation moves 0 hexes and still costs 1 AP.

2. Empower
- Type: Active
- Target: Unit Target
- Unlock: Level 1
- Mana Cost: 10
- AP Cost: 1
- Cooldown: 3 rounds
- Range: 2 hexes
- Duration: 1 round
- Rules: Magnus empowers an allied hero or himself with crushing momentum. The empowered hero gains bonus Attack, and their Attack actions cleave in a 2-hex cone in front of them, dealing bonus damage to all other enemy units in the cone.
- Scaling: 1-5: +3 Attack, 2 cleave damage | 6-11: +5 Attack, 3 cleave damage | 12+: +7 Attack, 4 cleave damage

3. Skewer
- Type: Active
- Target: Direction/Vector
- Unlock: Level 1
- Mana Cost: 16
- AP Cost: 2
- Cooldown: 3 rounds
- Range: Up to 3 hexes
- Rules: Magnus charges in a straight line up to 3 hexes. Enemy heroes in his path take damage and are dragged with him. After Magnus finishes moving, place each dragged hero on a legal Open hex adjacent to Magnus.
- Scaling: 1-5: 15 damage | 6-11: 25 damage | 12+: 35 damage
- Notes: Magnus may move through occupied hexes during Skewer, but must end on a legal Open hex. If multiple heroes are dragged, the Magnus player chooses the order in which they are placed adjacent to Magnus.

4. Reverse Polarity
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 6
- Mana Cost: 30
- AP Cost: 2
- Cooldown: 5 rounds
- Radius: 2 hexes
- Rules: Magnus violently reverses the battlefield's pull. All enemy heroes within 2 hexes are pulled onto the single hex directly in front of Magnus, take damage, and are stunned. For the rest of Magnus's current activation, those heroes may temporarily share that hex so Magnus can follow up with abilities such as Skewer.
- Scaling: 6-11: 20 damage, stun (3 AP loss) | 12-17: 30 damage, stun (4 AP loss) | 18+: 40 damage, stun (5 AP loss)
- Notes: When Magnus's activation ends, all heroes stacked by Reverse Polarity are immediately dispersed to legal Open hexes adjacent to Magnus. The Magnus player chooses the placement order if multiple legal hexes are available.

Upgrade / notes panel:
- Aghanim's Scepter Upgrade: Reverse Polarity radius increases to 3 hexes.

Graphic direction:
- The card should feel like a technical tabletop rules reference first, fantasy illustration second
- Use a wide landscape layout with strong horizontal row separation and consistent icon chips
- Keep the text area bright and readable with minimal texture behind it
- Include subtle horn motifs, force-wave crescents, impact cracks, drag lines, and disciplined martial ornament without reducing clarity
- Ensure the color story, border finish, chip styling, and spell-effect rendering clearly match the attached Hero Card reference
- The look of Shockwave, Empower, Skewer, and Reverse Polarity should feel like direct spell extensions of the attached Hero Card art rather than newly invented visual languages
- Present as a straight-on flat card render on a neutral background

Typography direction:
- Forceful fantasy title for the hero name
- Clear section titles for each ability
- Compact, highly legible game UI font for rules text and numbers
- Costs, timing information, and scaling values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the four-row structure, typography hierarchy, or cost strip order
- Do not arrange the abilities in a 2x2 grid, card quadrant layout, or any multi-column panel system
- Do not turn the card into a hero card, poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not use a large full-card portrait in place of rules text space
- Do not drift away from the attached Hero Card's visual language for spell motifs, icon treatment, palette behavior, or ornamental detailing
- Do not copy official game splash art or spell icons
- Do not add current cooldown markers, current mana trackers, AP trackers, or board-state counters
- Do not invent extra mechanics, extra scaling tiers, or extra decorative clutter
```

---

## Example Image Prompt — Juggernaut Hero Card

Use the following prompt when generating a sample hero card image for Juggernaut:

```text
Create a polished fantasy board game hero card in portrait orientation, designed for a 10 × 15 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the Mirana example hero card. Keep this visually part of the same manufactured hero-card product family.

Overall style: premium tabletop card design, clean information hierarchy, readable at print size, disciplined masked swordsman theme, agility-class visual identity, ivory, crimson, warm gold, and restrained jade accents, crisp iconography, high contrast text panels, collectible but practical.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, name banner position, class ribbon position, attack-type badge position, role tag position, portrait window position and proportions, stat strip position and icon order, progression strip position, four-row ability grid structure, typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view established by the Mirana example.
- Only change the portrait artwork, accent palette, emblem, and hero-specific atmospheric details inside the established frame.

Card structure:
- Top banner with the name: JUGGERNAUT
- Agility class band in green
- Attack type badge: Melee
- Role tags: Carry, Durable, Pusher
- Large central portrait of Juggernaut as an original masked blade master: elegant white mask, flowing red sash, curved katana, controlled whirlwind energy, poised forward stance, calm but lethal presence
- Horizontal stat strip below portrait with large readable icons and numbers
- Narrow progression strip
- Bottom half contains four compact ability summary rows with chips for unlock level, type, and target only

Base stats to show exactly:
- HP 95
- Mana 30
- Attack 9
- Attack Range 1 hex
- Defense 2
- Move Speed 1
- AP 10

Progression strip:
- Per Level: +10 HP | +8 Mana | +4 ATK | +1 DEF
- Milestone icons for Level 6, Level 12, Level 18
- Scepter badge reminder

Ability summary rows to display:

1. Blade Fury
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 1
- Summary: Spin in a bladestorm that damages nearby enemies while Juggernaut advances.

2. Healing Ward
- Type: Active
- Target: Unit Target
- Unlock: Level 1
- Summary: Place a fragile ward that heals nearby allied heroes over time.

3. Blade Dance
- Type: Passive
- Unlock: Level 1
- Summary: Juggernaut's first attack each activation deals bonus damage.

4. Omnislash
- Type: Active
- Target: Unit Target
- Unlock: Level 6
- Summary: Leap through enemy heroes in a rapid series of untargetable slashes.

Graphic direction:
- The card should feel like a readable tabletop component first, illustration showcase second
- Use clear panel separation and consistent icon chips
- Emphasize the iconic mask, disciplined sword form, red cloth movement, sweeping blade arcs, healing aura motifs, and precise burst combat
- Keep the layout uncluttered and legible; no fake tracker dials, no board-game counters, no 3D mockup angle
- Present as a straight-on flat card render on a neutral background
- Include subtle hex motifs and tactical board game icon language for spinning area damage, healing radius, and chained strikes

Typography direction:
- Large, elegant fantasy title for the hero name
- Clean, compact sans-serif or highly readable game UI font for rules text
- Important values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the stat strip order, typography hierarchy, or four-row ability layout
- Do not introduce new decorative badges, alternate UI systems, or extra card zones
- Do not turn the card into a poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not print full numerical rules text, costs, cooldowns, or scaling values on the hero card
- Do not copy official game splash art
- Do not use a trading card game frame style
- Do not make it look like a mobile game screenshot
- Do not add extra abilities, extra stats, or extra decorative clutter
- Do not place current HP, current Mana, gold, XP, cooldown trackers, or item slots on the card
```

---

## Example Image Prompt — Juggernaut Abilities Card

Use the following prompt when generating a sample landscape Abilities Card image for Juggernaut:

```text
Create a polished fantasy board game abilities reference card in landscape orientation, designed for a 15 × 10 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the attached Juggernaut Hero Card image as the primary visual reference for this Abilities Card. Match its card family exactly: same design language, same frame sensibility, same typography hierarchy, same icon rendering style, same accent palette logic, same material finish, and the same treatment of masked swordsman motifs, disciplined bladework, healing ward iconography, whirlwind motion, and precision-strike effects. The Abilities Card should look like it was manufactured as a companion component to that exact Hero Card, not merely a related card from a similar set.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the established landscape Abilities Card template for this game. Keep this visually part of the same manufactured product family as the attached Hero Card while clearly functioning as a rules reference.

Overall style: premium tabletop reference component, rules-forward layout, highly readable at print size, disciplined masked swordsman theme, agility-class visual identity, ivory, crimson, warm gold, and restrained jade accents, clean dividers, restrained motion texture, crisp iconography, collectible but practical.

This is an Abilities Card, not a Hero Card. The card should prioritize gameplay clarity, full rules readability, and explicit numerical values over portrait space.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, hero header position, summary strip position, and a four-row stacked ability layout with one ability per horizontal row. Preserve the typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view across all Abilities Cards.
- Derive the small hero portrait or crest, ability icons, accent palette, and hero-specific atmospheric details directly from the attached Hero Card so the spell visuals feel like the same hero package.
- Make the spinning blade arcs, healing ward glow, sword-trail language, and rapid slash sequencing visually consistent with what appears on the attached Hero Card.

Card structure:
- Hero header with the name: JUGGERNAUT
- Small crest or portrait accent
- Summary strip listing Blade Fury, Healing Ward, Blade Dance, Omnislash
- Four clearly separated horizontal ability rows, one per ability, each with icon, type, target, costs, rules text, and scaling
- Upgrade / notes panel for key reminders
- Small footer legend for icon language if needed

Ability data to show exactly:

1. Blade Fury
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 1
- Mana Cost: 15
- AP Cost: 2
- Cooldown: 3 rounds
- Duration: Current activation
- Rules: Juggernaut enters a spinning bladestorm for the rest of his current activation. While Blade Fury is active, Juggernaut gains Spell Immunity, cannot use Attack actions, and cannot use other abilities or items. When Blade Fury is activated, and each time Juggernaut moves into a new hex during that activation, deal damage to all enemy units within 1 hex.
- Scaling: 1-5: 12 damage per hit | 6-11: 18 damage per hit | 12+: 24 damage per hit
- Notes: Blade Fury is intended to convert Juggernaut's Move actions into area pressure. If Juggernaut does not move after activating Blade Fury, only the initial damage instance is applied.

2. Healing Ward
- Type: Active
- Target: Unit Target
- Unlock: Level 1
- Mana Cost: 12
- AP Cost: 1
- Cooldown: 4 rounds
- Range: 1 hex
- Rules: Place a Healing Ward token on an adjacent Open hex. At the start of each allied hero's activation, that hero restores HP if they are within 2 hexes of the Healing Ward. At the start of each of Juggernaut's activations, he may move the Healing Ward up to 2 hexes. Only one Healing Ward may be on the board for Juggernaut at a time.
- Scaling: 1-5: Heal 8 HP per activation, lasts 1 round | 6-11: Heal 12 HP per activation, lasts 2 rounds | 12+: Heal 16 HP per activation, lasts 2 rounds
- Notes: The Healing Ward is a fragile summon. Any enemy hero adjacent to the ward may spend 1 Attack action to destroy it immediately.

3. Blade Dance
- Type: Passive
- Unlock: Level 1
- Rules: Juggernaut's swordsmanship makes his strikes exceptionally lethal. The first Attack action Juggernaut resolves during each activation deals bonus damage.
- Scaling: 1-5: +4 bonus damage | 6-11: +6 bonus damage | 12+: +9 bonus damage
- Notes: Blade Dance also applies to the first slash of Omnislash each time Juggernaut uses that ability.

4. Omnislash
- Type: Active
- Target: Unit Target
- Unlock: Level 6
- Mana Cost: 30
- AP Cost: 2
- Cooldown: 4 rounds
- Range: 2 hexes
- Rules: Juggernaut targets an enemy hero within range and immediately begins Omnislash. Resolve the listed number of slashes one at a time. For the first slash, Juggernaut hits the chosen target. For each later slash, the Juggernaut player chooses an enemy hero within 1 hex of the hero hit by the previous slash. If there is no other enemy hero within 1 hex, Juggernaut may hit that same hero again instead. Each slash deals damage equal to Juggernaut's current Attack. While Omnislash is resolving, Juggernaut cannot be targeted by enemy attacks or abilities. After the final slash, place Juggernaut on any Open hex adjacent to the hero hit by the last slash.
- Scaling: 6-11: 3 slashes | 12-17: 4 slashes | 18+: 5 slashes

Upgrade / notes panel:
- Aghanim's Scepter Upgrade: Omnislash gains +1 slash at all levels and its cooldown is reduced to 3 rounds.

Graphic direction:
- The card should feel like a technical tabletop rules reference first, fantasy illustration second
- Use a wide landscape layout with strong horizontal row separation and consistent icon chips
- Keep the text area bright and readable with minimal texture behind it
- Include subtle mask motifs, clean sword arcs, healing sigils, wind-swept ribbons, and precise motion trails without reducing clarity
- Ensure the color story, border finish, chip styling, and spell-effect rendering clearly match the attached Hero Card reference
- The look of Blade Fury, Healing Ward, Blade Dance, and Omnislash should feel like direct spell extensions of the attached Hero Card art rather than newly invented visual languages
- Present as a straight-on flat card render on a neutral background

Typography direction:
- Elegant fantasy title for the hero name
- Clear section titles for each ability
- Compact, highly legible game UI font for rules text and numbers
- Costs, timing information, and scaling values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the four-row structure, typography hierarchy, or cost strip order
- Do not arrange the abilities in a 2x2 grid, card quadrant layout, or any multi-column panel system
- Do not turn the card into a hero card, poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not use a large full-card portrait in place of rules text space
- Do not drift away from the attached Hero Card's visual language for spell motifs, icon treatment, palette behavior, or ornamental detailing
- Do not copy official game splash art or spell icons
- Do not add current cooldown markers, current mana trackers, AP trackers, or board-state counters
- Do not invent extra mechanics, extra scaling tiers, or extra decorative clutter
```

---

## Example Image Prompt — Weaver Hero Card

Use the following prompt when generating a sample hero card image for Weaver:

```text
Create a polished fantasy board game hero card in portrait orientation, designed for a 10 × 15 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the Mirana example hero card. Keep this visually part of the same manufactured hero-card product family.

Overall style: premium tabletop card design, clean information hierarchy, readable at print size, temporal insect-skirmisher theme, agility-class visual identity, teal, deep indigo, pale cyan, and iridescent amber accents, crisp iconography, high contrast text panels, collectible but practical.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, name banner position, class ribbon position, attack-type badge position, role tag position, portrait window position and proportions, stat strip position and icon order, progression strip position, four-row ability grid structure, typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view established by the Mirana example.
- Only change the portrait artwork, accent palette, emblem, and hero-specific atmospheric details inside the established frame.

Card structure:
- Top banner with the name: WEAVER
- Agility class band in green
- Attack type badge: Ranged
- Role tags: Carry, Escape, Nuker
- Large central portrait of Weaver as an original time-warping insectoid skirmisher: sleek chitin body, glowing segmented eyes, razor limbs, shimmering wings or temporal fins, distorted time trails, poised to dart through the battlefield
- Horizontal stat strip below portrait with large readable icons and numbers
- Narrow progression strip
- Bottom half contains four compact ability summary rows with chips for unlock level, type, and target only

Base stats to show exactly:
- HP 72
- Mana 35
- Attack 8
- Attack Range 3 hexes
- Defense 1
- Move Speed 1
- AP 10

Progression strip:
- Per Level: +8 HP | +10 Mana | +4 ATK | +1 DEF
- Milestone icons for Level 6, Level 12, Level 18
- Scepter badge reminder

Ability summary rows to display:

1. The Swarm
- Type: Active
- Target: Point Target
- Unlock: Level 1
- Summary: Release parasitic beetles that latch onto clustered enemies and weaken their Defense.

2. Shukuchi
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 1
- Summary: Turn invisible and surge through enemies, damaging units passed through.

3. Geminate Attack
- Type: Passive
- Unlock: Level 1
- Summary: Weaver's first attack each activation immediately fires a second strike.

4. Time Lapse
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 6
- Summary: Rewind Weaver to his previous position and restore his saved state.

Graphic direction:
- The card should feel like a readable tabletop component first, illustration showcase second
- Use clear panel separation and consistent icon chips
- Emphasize insect silhouette, iridescent chitin, parasite motifs, temporal distortion, darting motion, and elusive ranged pressure
- Keep the layout uncluttered and legible; no fake tracker dials, no board-game counters, no 3D mockup angle
- Present as a straight-on flat card render on a neutral background
- Include subtle hex motifs and tactical board game icon language for area attachment effects, invisibility movement, and rewind timing

Typography direction:
- Large, elegant fantasy title for the hero name
- Clean, compact sans-serif or highly readable game UI font for rules text
- Important values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the stat strip order, typography hierarchy, or four-row ability layout
- Do not introduce new decorative badges, alternate UI systems, or extra card zones
- Do not turn the card into a poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not print full numerical rules text, costs, cooldowns, or scaling values on the hero card
- Do not copy official game splash art
- Do not use a trading card game frame style
- Do not make it look like a mobile game screenshot
- Do not add extra abilities, extra stats, or extra decorative clutter
- Do not place current HP, current Mana, gold, XP, cooldown trackers, or item slots on the card
```

---

## Example Image Prompt — Weaver Abilities Card

Use the following prompt when generating a sample landscape Abilities Card image for Weaver:

```text
Create a polished fantasy board game abilities reference card in landscape orientation, designed for a 15 × 10 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the attached Weaver Hero Card image as the primary visual reference for this Abilities Card. Match its card family exactly: same design language, same frame sensibility, same typography hierarchy, same icon rendering style, same accent palette logic, same material finish, and the same treatment of insectoid chitin, parasitic beetles, temporal distortion, high-speed traversal, and rewind effects. The Abilities Card should look like it was manufactured as a companion component to that exact Hero Card, not merely a related card from a similar set.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the established landscape Abilities Card template for this game. Keep this visually part of the same manufactured product family as the attached Hero Card while clearly functioning as a rules reference.

Overall style: premium tabletop reference component, rules-forward layout, highly readable at print size, temporal insect-skirmisher theme, agility-class visual identity, teal, deep indigo, pale cyan, and iridescent amber accents, clean dividers, restrained temporal texture, crisp iconography, collectible but practical.

This is an Abilities Card, not a Hero Card. The card should prioritize gameplay clarity, full rules readability, and explicit numerical values over portrait space.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, hero header position, summary strip position, and a four-row stacked ability layout with one ability per horizontal row. Preserve the typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view across all Abilities Cards.
- Derive the small hero portrait or crest, ability icons, accent palette, and hero-specific atmospheric details directly from the attached Hero Card so the spell visuals feel like the same hero package.
- Make the beetle swarms, invisibility trails, rapid double-shot motifs, and time-rewind iconography visually consistent with what appears on the attached Hero Card.

Card structure:
- Hero header with the name: WEAVER
- Small crest or portrait accent
- Summary strip listing The Swarm, Shukuchi, Geminate Attack, Time Lapse
- Four clearly separated horizontal ability rows, one per ability, each with icon, type, target, costs, rules text, and scaling
- Upgrade / notes panel for key reminders
- Small footer legend for icon language if needed

Ability data to show exactly:

1. The Swarm
- Type: Active
- Target: Point Target
- Unlock: Level 1
- Mana Cost: 16
- AP Cost: 1
- Cooldown: 3 rounds
- Range: 4 hexes
- Rules: Weaver releases a cluster of parasitic weaverlings at a target hex. Apply a Swarm Beetle token to each enemy hero on the target hex and all adjacent hexes. At the start of each affected hero's activation, that hero takes damage and suffers -1 Defense while the token remains attached.
- Scaling: 1-5: 3 damage per activation, lasts 1 round | 6-11: 4 damage per activation, lasts 2 rounds | 12+: 5 damage per activation, lasts 2 rounds
- Notes: An affected hero may spend 1 Attack action during their activation to remove their own Swarm Beetle token. The Defense reduction does not stack from multiple beetles.

2. Shukuchi
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 1
- Mana Cost: 10
- AP Cost: 1
- Cooldown: 2 rounds
- Duration: Current activation
- Rules: Weaver slips into the folds of reality and becomes Invisible for the rest of his current activation. During that activation, each Move action Weaver takes may move up to 2 hexes instead of 1. The first time Weaver passes through an enemy unit during each Move action, that unit takes damage.
- Scaling: 1-5: 10 damage per pass-through | 6-11: 16 damage per pass-through | 12+: 22 damage per pass-through
- Notes: Weaver must still end each Move action on a legal Open hex. Shukuchi ends immediately if Weaver uses an Attack action or another ability.

3. Geminate Attack
- Type: Passive
- Unlock: Level 1
- Rules: The first time Weaver resolves an Attack action during each activation, he immediately makes a second attack.
- Scaling: 1-5: Second attack deals -2 damage | 6-11: Second attack deals -1 damage | 12+: Second attack deals full damage
- Notes: The second attack must target the same enemy hero, creep, or structure as the first attack.

4. Time Lapse
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 6
- Mana Cost: 25
- AP Cost: 1
- Cooldown: 5 rounds
- Rules: Weaver rewinds himself to the state he had at the start of his previous activation. Move Weaver back to the hex marked by his Time Lapse marker, then restore his HP and Mana to the saved values from that snapshot.
- Scaling: 6-11: Rewind self | 12-17: Rewind self and remove one dispellable debuff | 18+: Rewind self and remove all dispellable debuffs
- Notes: At the start of each Weaver activation, place a Time Lapse marker on Weaver's current hex and note his current HP and Mana with small number tokens on his Hero Board. If the marked hex is no longer a legal Open hex when Time Lapse resolves, place Weaver on the nearest legal Open hex instead.

Upgrade / notes panel:
- Aghanim's Scepter Upgrade: Time Lapse may target an allied hero within 2 hexes instead of Weaver. Use that hero's saved Time Lapse state.

Graphic direction:
- The card should feel like a technical tabletop rules reference first, fantasy illustration second
- Use a wide landscape layout with strong horizontal row separation and consistent icon chips
- Keep the text area bright and readable with minimal texture behind it
- Include subtle insect wing geometry, beetle silhouettes, temporal ripples, segmented chitin patterns, and motion streaks without reducing clarity
- Ensure the color story, border finish, chip styling, and spell-effect rendering clearly match the attached Hero Card reference
- The look of The Swarm, Shukuchi, Geminate Attack, and Time Lapse should feel like direct spell extensions of the attached Hero Card art rather than newly invented visual languages
- Present as a straight-on flat card render on a neutral background

Typography direction:
- Elegant fantasy title for the hero name
- Clear section titles for each ability
- Compact, highly legible game UI font for rules text and numbers
- Costs, timing information, and scaling values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the four-row structure, typography hierarchy, or cost strip order
- Do not arrange the abilities in a 2x2 grid, card quadrant layout, or any multi-column panel system
- Do not turn the card into a hero card, poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not use a large full-card portrait in place of rules text space
- Do not drift away from the attached Hero Card's visual language for spell motifs, icon treatment, palette behavior, or ornamental detailing
- Do not copy official game splash art or spell icons
- Do not add current cooldown markers, current mana trackers, AP trackers, or board-state counters
- Do not invent extra mechanics, extra scaling tiers, or extra decorative clutter
```

---

## Example Image Prompt — Crystal Maiden Abilities Card

Use the following prompt when generating a sample landscape Abilities Card image for Crystal Maiden:

```text
Create a polished fantasy board game abilities reference card in landscape orientation, designed for a 15 × 10 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the attached Crystal Maiden Hero Card image as the primary visual reference for this Abilities Card. Match its card family exactly: same design language, same frame sensibility, same typography hierarchy, same icon rendering style, same accent palette logic, same material finish, and the same treatment of frost magic, spell motifs, and ornamental details. The Abilities Card should look like it was manufactured as a companion component to that exact Hero Card, not merely a related card from a similar set.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the established landscape Abilities Card template for this game. Keep this visually part of the same manufactured product family as the attached Hero Card while clearly functioning as a rules reference.

Overall style: premium tabletop reference component, rules-forward layout, highly readable at print size, elegant icy magical theme, intelligence-class visual identity, blue, silver, frost-white, and pale cyan palette, clean dividers, restrained magical texture, crisp iconography, collectible but practical.

This is an Abilities Card, not a Hero Card. The card should prioritize gameplay clarity, full rules readability, and explicit numerical values over portrait space.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, hero header position, summary strip position, and a four-row stacked ability layout with one ability per horizontal row. Preserve the typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view across all Abilities Cards.
- Derive the small hero portrait or crest, ability icons, accent palette, and hero-specific atmospheric details directly from the attached Hero Card so the spell visuals feel like the same hero package.
- Make the spell iconography, magical effect shapes, rune language, frost textures, and decorative motifs visually consistent with what appears on the attached Hero Card.

Card structure:
- Hero header with the name: CRYSTAL MAIDEN
- Small crest or portrait accent
- Summary strip listing Crystal Nova, Frostbite, Arcane Aura, Freezing Field
- Four clearly separated horizontal ability rows, one per ability, each with icon, type, target, costs, rules text, and scaling
- Upgrade / notes panel for key reminders
- Small footer legend for icon language if needed

Ability data to show exactly:

1. Crystal Nova
- Type: Active
- Target: Ground-Targeted AoE
- Unlock: Level 1
- Mana Cost: 15
- AP Cost: 2
- Cooldown: 2 rounds
- Range: 2 hexes
- Area: 2-hex radius
- Rules: Blast an area with damaging frost, dealing damage to all enemy units within a 2-hex radius and applying a Slow debuff for the specified duration.
- Scaling: 1-5: 20 damage, -2 AP for 10 turns | 6-11: 30 damage, -3 AP for 1 round | 12+: 40 damage, -4 AP for 2 rounds

2. Frostbite
- Type: Active
- Target: Unit Target
- Unlock: Level 1
- Mana Cost: 20
- AP Cost: 2
- Cooldown: 1.5 rounds
- Range: 2 hexes
- Rules: Encase target enemy unit in ice, rooting them in place and dealing damage over time. Rooted units cannot move but may still use abilities.
- Scaling: 1-5: 20 total damage over 10 turns | 6-11: 40 total damage over 20 turns | 12+: 60 total damage over 20 turns

3. Arcane Aura
- Type: Passive (Aura)
- Target: Global allied mana regeneration
- Unlock: Level 1
- Rules: Crystal Maiden and all allied heroes passively regenerate Mana during the Round End Phase.
- Scaling: 1-5: 10 Mana per round, global | 6-11: 20 Mana per round, global | 12+: 30 Mana per round, global

4. Freezing Field
- Type: Channeled
- Target: No Target (Self-Cast)
- Unlock: Level 6
- Mana Cost: 40
- AP Cost: 1
- Cooldown: 5 rounds
- Duration: Channeled
- Area: 2 hex radius
- Rules: Crystal Maiden channels a massive ice storm around her, dealing damage in pulses to all enemy units within range and slowing them. Must remain stationary while channeling. Interrupted by Stun, Silence, forced movement, or voluntary cancellation.
- Scaling: 6-11: 20 damage per pulse, -2 AP | 12-17: 30 damage per pulse, -3 AP | 18+: 40 damage per pulse, -5 AP

Graphic direction:
- The card should feel like a technical tabletop rules reference first, fantasy illustration second
- Use a wide landscape layout with strong horizontal row separation and consistent icon chips
- Keep the text area bright and readable with minimal texture behind it
- Include subtle frost motifs, snowflake geometry, and crystalline accents without reducing clarity
- Ensure the color story, border finish, chip styling, and spell-effect rendering clearly match the attached Hero Card reference
- The look of Crystal Nova, Frostbite, Arcane Aura, and Freezing Field should feel like direct spell extensions of the attached Hero Card art rather than newly invented visual languages
- Present as a straight-on flat card render on a neutral background

Typography direction:
- Elegant fantasy title for the hero name
- Clear section titles for each ability
- Compact, highly legible game UI font for rules text and numbers
- Costs, timing information, and scaling values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the four-row structure, typography hierarchy, or cost strip order
- Do not arrange the abilities in a 2x2 grid, card quadrant layout, or any multi-column panel system
- Do not turn the card into a hero card, poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not use a large full-card portrait in place of rules text space
- Do not drift away from the attached Hero Card's visual language for spell motifs, icon treatment, palette behavior, or ornamental detailing
- Do not copy official game splash art or spell icons
- Do not add current cooldown markers, current mana trackers, AP trackers, or board-state counters
- Do not invent extra mechanics, extra scaling tiers, or extra decorative clutter
```

---

## Example Image Prompt — Pudge Hero Card

Use the following prompt when generating a sample hero card image for Pudge:

```text
Create a polished fantasy board game hero card in portrait orientation, designed for a 10 × 15 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the Mirana example hero card. Keep this visually part of the same manufactured hero-card product family.

Overall style: premium tabletop card design, clean information hierarchy, readable at print size, brutal grotesque butcher theme, strength-class visual identity, sickly green, rusted iron, dark leather, and blood-red accents, grim but still functional as a board game component, crisp iconography, high contrast text panels, collectible but practical.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, name banner position, class ribbon position, attack-type badge position, role tag position, portrait window position and proportions, stat strip position and icon order, progression strip position, four-row ability grid structure, typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view established by the Mirana example.
- Only change the portrait artwork, accent palette, emblem, and hero-specific atmospheric details inside the established frame.

Card structure:
- Top banner with the name: PUDGE
- Strength class band in red
- Attack type badge: Melee
- Role tags: Initiator, Ganker, Durable
- Large central portrait of Pudge as an original grotesque flesh golem butcher: massive bloated body, scarred skin, stitched flesh, iron hooks and chains, cleaver silhouette, toxic fumes, unsettling grin, hulking posture
- Horizontal stat strip below portrait with large readable icons and numbers
- Narrow progression strip
- Bottom half contains four compact ability summary rows with chips for unlock level, type, and target only

Base stats to show exactly:
- HP 115
- Mana 25
- Attack 7
- Attack Range 1 hex
- Defense 3
- Move Speed 1
- AP 10

Progression strip:
- Per Level: +12 HP | +8 Mana | +4 ATK | +1 DEF
- Milestone icons for Level 6, Level 12, Level 18
- Optional small status note: Design in Progress

Ability summary rows to display:

1. Meat Hook
- Type: Active
- Target: Direction/Vector
- Special: Skillshot
- Unlock: Level 1
- Summary: Launch a hook in a straight line to damage and drag the first unit hit.

2. Rot
- Type: Toggle
- Target: No Target (Self-Cast)
- Unlock: Level 1
- Summary: Release toxic gas that damages nearby enemies and Pudge himself.

3. Flesh Heap
- Type: Passive
- Unlock: Level 1
- Summary: Gain permanent bonus HP when nearby enemy heroes die.

4. Dismember
- Type: Channeled
- Target: Unit Target
- Unlock: Level 6
- Summary: Channel on an adjacent enemy hero to damage and fully disable them.

Graphic direction:
- The card should feel like a readable tabletop component first, illustration showcase second
- Use clear panel separation and consistent icon chips
- Emphasize chains, hook silhouette, toxic fumes, stained metal, diseased green glow, and hulking tanky menace
- Keep the layout uncluttered and legible; no fake tracker dials, no board-game counters, no 3D mockup angle
- Present as a straight-on flat card render on a neutral background
- Include subtle hex motifs and tactical board game range icon language

Typography direction:
- Large, heavy fantasy title for the hero name
- Clean, compact sans-serif or highly readable game UI font for rules text
- Important values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the stat strip order, typography hierarchy, or four-row ability layout
- Do not introduce new decorative badges, alternate UI systems, or extra card zones
- Do not turn the card into a poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not print full numerical rules text, costs, cooldowns, or scaling values on the hero card
- Do not copy official game splash art
- Do not use a trading card game frame style
- Do not make it look like a mobile game screenshot
- Do not add extra abilities, extra stats, or extra decorative clutter
- Do not place current HP, current Mana, gold, XP, cooldown trackers, or item slots on the card
```

---

## Example Image Prompt — Pudge Abilities Card

Use the following prompt when generating a sample landscape Abilities Card image for Pudge:

```text
Create a polished fantasy board game abilities reference card in landscape orientation, designed for a 15 × 10 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the attached Pudge Hero Card image as the primary visual reference for this Abilities Card. Match its card family exactly: same design language, same frame sensibility, same typography hierarchy, same icon rendering style, same accent palette logic, same material finish, and the same treatment of grotesque fleshcraft, chains, butcher tools, toxic gas, and brutal physical spell motifs. The Abilities Card should look like it was manufactured as a companion component to that exact Hero Card, not merely a related card from a similar set.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the established landscape Abilities Card template for this game. Keep this visually part of the same manufactured product family as the attached Hero Card while clearly functioning as a rules reference.

Overall style: premium tabletop reference component, rules-forward layout, highly readable at print size, brutal grotesque butcher theme, strength-class visual identity, sickly green, rusted iron, dark leather, stained bone, and blood-red accents, clean dividers, grim toxic texture, crisp iconography, collectible but practical.

This is an Abilities Card, not a Hero Card. The card should prioritize gameplay clarity, full rules readability, and explicit numerical values over portrait space.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, hero header position, summary strip position, and a four-row stacked ability layout with one ability per horizontal row. Preserve the typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view across all Abilities Cards.
- Derive the small hero portrait or crest, ability icons, accent palette, and hero-specific atmospheric details directly from the attached Hero Card so the spell visuals feel like the same hero package.
- Make the hook silhouette, toxic vapor shapes, stitched-flesh motifs, metal textures, and brutal physical spell iconography visually consistent with what appears on the attached Hero Card.

Card structure:
- Hero header with the name: PUDGE
- Small crest or portrait accent
- Summary strip listing Meat Hook, Rot, Flesh Heap, Dismember
- Four clearly separated horizontal ability rows, one per ability, each with icon, type, target, costs, rules text, and scaling
- Upgrade / notes panel for key reminders
- Small footer legend for icon language if needed

Ability data to show exactly:

1. Meat Hook
- Type: Active
- Target: Direction/Vector
- Special: Skillshot
- Unlock: Level 1
- Mana Cost: 14
- AP Cost: 2
- Cooldown: 2.5 rounds
- Range: 5 hexes max
- Rules: Launch a bloody hook in a straight line in the chosen direction. The hook travels up to 5 hexes or until it hits an enemy hero or creep. The first unit struck takes damage and is pulled back to the hex adjacent to Pudge. Enemies may use the Dodge Skillshot reaction to attempt to avoid the hook.
- Scaling: 1-5: 15 damage | 6-11: 25 damage | 12+: 40 damage
- Notes: The hooked unit is forcibly moved to a hex adjacent to Pudge along the line of the hook. If the direct hex is not available, the player being hooked chooses which adjacent hex.

2. Rot
- Type: Toggle
- Target: No Target (Self-Cast)
- Unlock: Level 1
- Mana Cost: 0
- AP Cost: 1 to activate
- Cooldown: None
- Rules: Pudge releases toxic gases around himself, dealing damage per turn to all enemy units within 1 hex and to Pudge himself. Can be toggled on during Pudge's turn and toggled off at any time, even during other heroes' turns, unless Pudge is Silenced. While active, Rot damages all affected units, including Pudge, at the start of each hero's activation if they are within range.
- Scaling: 1-5: 2 damage per activation | 6-11: 3 damage per activation | 12+: 5 damage per activation
- Notes: Per activation means the damage ticks at the start of every hero's turn. Pudge takes the same damage as enemies.

3. Flesh Heap
- Type: Passive
- Unlock: Level 1
- Rules: Pudge gains permanent bonus HP whenever an enemy hero dies within 3 hexes of him. These bonuses stack indefinitely throughout the game and apply retroactively to his current Health total.
- Scaling: 1-5: +8 HP per enemy hero death | 6-11: +12 HP per enemy hero death | 12+: +16 HP per enemy hero death
- Notes: Flesh Heap stacks are permanent and persist through death.

4. Dismember
- Type: Channeled
- Target: Unit Target
- Unlock: Level 6
- Mana Cost: 30
- AP Cost: 2
- Cooldown: 4 rounds
- Duration: Channeled (max 2 rounds)
- Range: 1 hex
- Rules: Pudge channels his ultimate on target enemy hero within 1 hex, dealing damage per turn and disabling the target completely. The target cannot move, attack, or use abilities while Dismembered. Pudge must remain adjacent to the target while channeling. Interrupted by Stun, Silence, forced movement, or voluntary cancellation.
- Scaling: 6-11: 4 damage per activation | 12-17: 6 damage per activation | 18+: 8 damage per activation
- Notes: Per activation means damage is dealt at the start of each hero's turn while the channel is active. Pudge and the target are both effectively locked into the channel.

Upgrade / notes panel:
- Aghanim's Scepter Upgrade: Dismember can be cast on targets up to 2 hexes away, Pudge heals for 50% of damage dealt, and the duration increases to 3 rounds maximum.

Graphic direction:
- The card should feel like a technical tabletop rules reference first, fantasy illustration second
- Use a wide landscape layout with strong horizontal row separation and consistent icon chips
- Keep the text area bright and readable with minimal texture behind it
- Include subtle chain motifs, butcher hooks, stitched seams, toxic vapor shapes, and rusted iron accents without reducing clarity
- Ensure the color story, border finish, chip styling, and spell-effect rendering clearly match the attached Hero Card reference
- The look of Meat Hook, Rot, Flesh Heap, and Dismember should feel like direct spell extensions of the attached Hero Card art rather than newly invented visual languages
- Present as a straight-on flat card render on a neutral background

Typography direction:
- Heavy fantasy title for the hero name
- Clear section titles for each ability
- Compact, highly legible game UI font for rules text and numbers
- Costs, timing information, and scaling values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the four-row structure, typography hierarchy, or cost strip order
- Do not arrange the abilities in a 2x2 grid, card quadrant layout, or any multi-column panel system
- Do not turn the card into a hero card, poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not use a large full-card portrait in place of rules text space
- Do not drift away from the attached Hero Card's visual language for spell motifs, icon treatment, palette behavior, or ornamental detailing
- Do not copy official game splash art or spell icons
- Do not add current cooldown markers, current mana trackers, AP trackers, or board-state counters
- Do not invent extra mechanics, extra scaling tiers, or extra decorative clutter
```

---

## Example Image Prompt — Lion Hero Card

Use the following prompt when generating a sample hero card image for Lion:

```text
Create a polished fantasy board game hero card in portrait orientation, designed for a 10 × 15 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the Mirana example hero card. Keep this visually part of the same manufactured hero-card product family.

Overall style: premium tabletop card design, clean information hierarchy, readable at print size, sinister arcane controller theme, intelligence-class visual identity, deep purple, black, crimson, and arcane gold palette, sharp infernal magical details, crisp iconography, high contrast text panels, collectible but practical.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, name banner position, class ribbon position, attack-type badge position, role tag position, portrait window position and proportions, stat strip position and icon order, progression strip position, four-row ability grid structure, typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view established by the Mirana example.
- Only change the portrait artwork, accent palette, emblem, and hero-specific atmospheric details inside the established frame.

Card structure:
- Top banner with the name: LION
- Intelligence class band in blue
- Attack type badge: Ranged
- Role tags: Support, Control, Nuker
- Large central portrait of Lion as an original demonic spellcaster: gaunt body, horned silhouette, clawed hand, glowing occult eyes, jagged robes, dark magical aura, one hand crackling with lethal energy
- Horizontal stat strip below portrait with large readable icons and numbers
- Narrow progression strip
- Bottom half contains four compact ability summary rows with chips for unlock level, type, and target only

Base stats to show exactly:
- HP 70
- Mana 45
- Attack 7
- Attack Range 3 hexes
- Defense 1
- Move Speed 1
- AP 10

Progression strip:
- Per Level: +10 HP | +12 Mana | +3 ATK | +1 DEF
- Milestone icons for Level 6, Level 12, Level 18
- Optional small status note: Design in Progress

Ability summary rows to display:

1. Earth Spike
- Type: Active
- Target: Direction/Vector
- Special: Skillshot
- Unlock: Level 1
- Summary: Send spikes in a line to damage and stun enemies in the path.

2. Hex
- Type: Active
- Target: Unit Target
- Unlock: Level 1
- Summary: Transform a target enemy into a helpless critter and fully disable them.

3. Mana Drain
- Type: Channeled
- Target: Unit Target
- Unlock: Level 1
- Summary: Channel on an enemy hero to drain Mana while line of sight is maintained.

4. Finger of Death
- Type: Active
- Target: Unit Target
- Unlock: Level 6
- Summary: Blast a single enemy hero with massive dark magic damage.

Graphic direction:
- The card should feel like a readable tabletop component first, illustration showcase second
- Use clear panel separation and consistent icon chips
- Emphasize demonic magic, jagged occult energy, infernal claws, and a fragile but terrifying controller identity
- Keep the layout uncluttered and legible; no fake tracker dials, no board-game counters, no 3D mockup angle
- Present as a straight-on flat card render on a neutral background
- Include subtle hex motifs and tactical board game icon language for line, stun, and control effects

Typography direction:
- Large, elegant but threatening fantasy title for the hero name
- Clean, compact sans-serif or highly readable game UI font for rules text
- Important values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the stat strip order, typography hierarchy, or four-row ability layout
- Do not introduce new decorative badges, alternate UI systems, or extra card zones
- Do not turn the card into a poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not print full numerical rules text, costs, cooldowns, or scaling values on the hero card
- Do not copy official game splash art
- Do not use a trading card game frame style
- Do not make it look like a mobile game screenshot
- Do not add extra abilities, extra stats, or extra decorative clutter
- Do not place current HP, current Mana, gold, XP, cooldown trackers, or item slots on the card
```

---

## Example Image Prompt — Lion Abilities Card

Use the following prompt when generating a sample landscape Abilities Card image for Lion:

```text
Create a polished fantasy board game abilities reference card in landscape orientation, designed for a 15 × 10 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the attached Lion Hero Card image as the primary visual reference for this Abilities Card. Match its card family exactly: same design language, same frame sensibility, same typography hierarchy, same icon rendering style, same accent palette logic, same material finish, and the same treatment of demonic magic, infernal claws, occult glyphs, dark arcane energy, and sinister spell effects. The Abilities Card should look like it was manufactured as a companion component to that exact Hero Card, not merely a related card from a similar set.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the established landscape Abilities Card template for this game. Keep this visually part of the same manufactured product family as the attached Hero Card while clearly functioning as a rules reference.

Overall style: premium tabletop reference component, rules-forward layout, highly readable at print size, sinister arcane controller theme, intelligence-class visual identity, deep purple, black, crimson, and arcane gold palette, clean dividers, restrained magical texture, crisp iconography, collectible but practical.

This is an Abilities Card, not a Hero Card. The card should prioritize gameplay clarity, full rules readability, and explicit numerical values over portrait space.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, hero header position, summary strip position, and a four-row stacked ability layout with one ability per horizontal row. Preserve the typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view across all Abilities Cards.
- Derive the small hero portrait or crest, ability icons, accent palette, and hero-specific atmospheric details directly from the attached Hero Card so the spell visuals feel like the same hero package.
- Make the spike eruptions, hex glyphs, mana siphon effects, infernal finger-beam language, and occult ornamental motifs visually consistent with what appears on the attached Hero Card.

Card structure:
- Hero header with the name: LION
- Small crest or portrait accent
- Summary strip listing Earth Spike, Hex, Mana Drain, Finger of Death
- Four clearly separated horizontal ability rows, one per ability, each with icon, type, target, costs, rules text, and scaling
- Upgrade / notes panel for key reminders
- Small footer legend for icon language if needed

Ability data to show exactly:

1. Earth Spike
- Type: Active
- Target: Direction/Vector
- Special: Skillshot
- Unlock: Level 1
- Mana Cost: 12
- AP Cost: 1
- Cooldown: 2 rounds
- Range: 4 hexes max
- Rules: Send a column of spikes erupting along a line in the chosen direction. The spikes travel up to 4 hexes, stunning and damaging all enemy units in a 1-hex-wide path. Enemies may use the Dodge Skillshot reaction to attempt to avoid the spikes.
- Scaling: 1-5: 15 damage, 8 AP stun | 6-11: 25 damage, 12 AP stun | 12+: 35 damage, 16 AP stun
- Notes: Unlike Sacred Arrow, Earth Spike hits all units along its path, not just the first.

2. Hex
- Type: Active
- Target: Unit Target
- Unlock: Level 1
- Mana Cost: 18
- AP Cost: 1
- Cooldown: 2 rounds
- Range: 3 hexes
- Rules: Transform target enemy hero into a harmless critter, disabling them completely for the duration. Hexed heroes cannot move, attack, use abilities, or use items. The target's Defense is reduced to 0 while Hexed.
- Scaling: 1-5: 10 turns duration | 6-11: 15 turns duration | 12+: 20 turns (1 round) duration
- Notes: Hex is a full disable, not just an AP reduction effect.

3. Mana Drain
- Type: Channeled
- Target: Unit Target
- Unlock: Level 1
- Mana Cost: 0
- AP Cost: 1 to activate
- Cooldown: 1 round
- Rules: Lion channels on target enemy hero within range, draining their Mana and transferring it to himself. The drain continues at the start of each hero's activation while the channel is active. Lion must maintain Line of Sight to the target. Interrupted by Stun, Silence, forced movement, target moving out of range or LoS, or voluntary cancellation.
- Scaling: 1-5: Drain 3 Mana per activation, max 1 round channel | 6-11: Drain 4 Mana per activation, max 1.5 rounds channel | 12+: Drain 5 Mana per activation, max 2 rounds channel
- Notes: Per activation means Mana is drained at the start of every hero's turn while the channel is active. Lion cannot move or take other actions while channeling.

4. Finger of Death
- Type: Active
- Target: Unit Target
- Unlock: Level 6
- Mana Cost: 40
- AP Cost: 2
- Cooldown: 3 rounds
- Range: 4 hexes
- Rules: Lion channels dark magic to instantly deal massive damage to a single target enemy hero. This is Lion's signature burst damage ability, capable of eliminating low-HP heroes or finishing fleeing enemies.
- Scaling: 6-11: 60 damage | 12-17: 90 damage | 18+: 120 damage
- Notes: Finger of Death deals pure instant damage, not damage over time.

Upgrade / notes panel:
- Aghanim's Scepter Upgrade: Earth Spike erupts in a T-shape pattern, the original line plus perpendicular spikes extending 2 hexes to each side at the endpoint. All affected units are stunned and damaged.
- Additional Scepter Note: Finger of Death cooldown is reduced to 2 rounds, damage increases by 30 at all levels, and if Finger of Death kills the target Lion gains a permanent stack granting +3 Mana and +2 Attack.
- Additional Scepter Note: Mana Drain becomes an AoE channel affecting all enemy heroes within 3 hexes of Lion. Each affected hero is drained separately, and Lion receives Mana from all of them.

Graphic direction:
- The card should feel like a technical tabletop rules reference first, fantasy illustration second
- Use a wide landscape layout with strong horizontal row separation and consistent icon chips
- Keep the text area bright and readable with minimal texture behind it
- Include subtle infernal sigils, demonic claw shapes, dark magical veins, occult geometry, and arcane burst motifs without reducing clarity
- Ensure the color story, border finish, chip styling, and spell-effect rendering clearly match the attached Hero Card reference
- The look of Earth Spike, Hex, Mana Drain, and Finger of Death should feel like direct spell extensions of the attached Hero Card art rather than newly invented visual languages
- Present as a straight-on flat card render on a neutral background

Typography direction:
- Elegant but threatening fantasy title for the hero name
- Clear section titles for each ability
- Compact, highly legible game UI font for rules text and numbers
- Costs, timing information, and scaling values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the four-row structure, typography hierarchy, or cost strip order
- Do not arrange the abilities in a 2x2 grid, card quadrant layout, or any multi-column panel system
- Do not turn the card into a hero card, poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not use a large full-card portrait in place of rules text space
- Do not drift away from the attached Hero Card's visual language for spell motifs, icon treatment, palette behavior, or ornamental detailing
- Do not copy official game splash art or spell icons
- Do not add current cooldown markers, current mana trackers, AP trackers, or board-state counters
- Do not invent extra mechanics, extra scaling tiers, or extra decorative clutter
```

---

## Example Image Prompt — Mirana Hero Card

Use the following prompt when generating a sample hero card image for Mirana:

```text
Create a polished fantasy board game hero card in portrait orientation, designed for a 10 × 15 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the Mirana example hero card. Keep this visually part of the same manufactured hero-card product family.

Overall style: premium tabletop card design, clean information hierarchy, readable at print size, moonlit huntress theme, agility-class visual identity, midnight blue, silver, moon-white, and teal accents, elegant celestial motifs, crisp iconography, high contrast text panels, collectible but practical.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, name banner position, class ribbon position, attack-type badge position, role tag position, portrait window position and proportions, stat strip position and icon order, progression strip position, four-row ability grid structure, typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view established by this Mirana example.
- Only change the portrait artwork, accent palette, emblem, and hero-specific atmospheric details inside the established frame.

Card structure:
- Top banner with the name: MIRANA
- Agility class band in green
- Attack type badge: Ranged
- Role tags: Roamer, Core, Initiator
- Large central portrait of Mirana as an original moon huntress: poised archer-priestess riding or posed with a sleek lunar beast, moonlit cloak, silver bow, starfall magic, agile and regal silhouette, wind-swept movement
- Horizontal stat strip below portrait with large readable icons and numbers
- Narrow progression strip
- Bottom half contains four compact ability summary rows with chips for unlock level, type, and target only

Base stats to show exactly:
- HP 85
- Mana 40
- Attack 8
- Attack Range 3 hexes
- Defense 2
- Move Speed 1
- AP 10

Progression strip:
- Per Level: +10 HP | +10 Mana | +4 ATK | +1 DEF
- Milestone icons for Level 6, Level 12, Level 18
- Scepter badge reminder

Ability summary rows to display:

1. Starfall
- Type: Active
- Target: Unit-Targeted AoE
- Unlock: Level 1
- Summary: Call down meteors around a target enemy, with a stronger hit at close range.

2. Sacred Arrow
- Type: Active
- Target: Direction/Vector
- Special: Skillshot
- Unlock: Level 1
- Summary: Fire a long-range arrow that damages and stuns based on travel distance.

3. Leap
- Type: Active
- Target: Direction/Vector
- Unlock: Level 1
- Summary: Leap forward over obstacles and gain a temporary Attack boost.

4. Moonlight Shadow
- Type: Active
- Target: No Target (Global)
- Unlock: Level 6
- Summary: Grant invisibility to Mirana and all allied heroes on the board.

Graphic direction:
- The card should feel like a readable tabletop component first, illustration showcase second
- Use clear panel separation and consistent icon chips
- Emphasize moonlight, stars, elegant movement, archer precision, feline speed, and a graceful high-skill huntress identity
- Keep the layout uncluttered and legible; no fake tracker dials, no board-game counters, no 3D mockup angle
- Present as a straight-on flat card render on a neutral background
- Include subtle hex motifs and tactical board game icon language for skillshots, leap movement, and invisibility

Typography direction:
- Large, elegant fantasy title for the hero name
- Clean, compact sans-serif or highly readable game UI font for rules text
- Important values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the stat strip order, typography hierarchy, or four-row ability layout
- Do not introduce new decorative badges, alternate UI systems, or extra card zones
- Do not turn the card into a poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not print full numerical rules text, costs, cooldowns, or scaling values on the hero card
- Do not copy official game splash art
- Do not use a trading card game frame style
- Do not make it look like a mobile game screenshot
- Do not add extra abilities, extra stats, or extra decorative clutter
- Do not place current HP, current Mana, gold, XP, cooldown trackers, or item slots on the card
```

---

## Example Image Prompt — Mirana Abilities Card

Use the following prompt when generating a sample landscape Abilities Card image for Mirana:

```text
Create a polished fantasy board game abilities reference card in landscape orientation, designed for a 15 × 10 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the attached Mirana Hero Card image as the primary visual reference for this Abilities Card. Match its card family exactly: same design language, same frame sensibility, same typography hierarchy, same icon rendering style, same accent palette logic, same material finish, and the same treatment of moonlight, celestial motifs, archer iconography, feline elegance, and luminous magical spell effects. The Abilities Card should look like it was manufactured as a companion component to that exact Hero Card, not merely a related card from a similar set.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the established landscape Abilities Card template for this game. Keep this visually part of the same manufactured product family as the attached Hero Card while clearly functioning as a rules reference.

Overall style: premium tabletop reference component, rules-forward layout, highly readable at print size, moonlit huntress theme, agility-class visual identity, midnight blue, silver, moon-white, and teal accents, elegant celestial motifs, clean dividers, restrained magical texture, crisp iconography, collectible but practical.

This is an Abilities Card, not a Hero Card. The card should prioritize gameplay clarity, full rules readability, and explicit numerical values over portrait space.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, hero header position, summary strip position, and a four-row stacked ability layout with one ability per horizontal row. Preserve the typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view across all Abilities Cards.
- Derive the small hero portrait or crest, ability icons, accent palette, and hero-specific atmospheric details directly from the attached Hero Card so the spell visuals feel like the same hero package.
- Make the arrow silhouette, moon sigils, starfall motifs, leap motion language, and invisibility iconography visually consistent with what appears on the attached Hero Card.

Card structure:
- Hero header with the name: MIRANA
- Small crest or portrait accent
- Summary strip listing Starfall, Sacred Arrow, Leap, Moonlight Shadow
- Four clearly separated horizontal ability rows, one per ability, each with icon, type, target, costs, rules text, and scaling
- Upgrade / notes panel for key reminders
- Small footer legend for icon language if needed

Ability data to show exactly:

1. Starfall
- Type: Active
- Target: Unit-Targeted AoE
- Unlock: Level 1
- Mana Cost: 12
- AP Cost: 1
- Cooldown: 2 rounds
- Range: 3 hexes
- Area: 2 hexes around the target
- Rules: Summon a wave of meteors around target enemy unit, dealing damage to all enemy units within 2 hexes of the target. If Mirana is within 2 hexes of the primary target, that unit takes a second instance of Starfall damage.
- Scaling: 1-5: 15 damage per instance | 6-11: 25 damage per instance | 12+: 35 damage per instance

2. Sacred Arrow
- Type: Active
- Target: Direction/Vector
- Special: Skillshot
- Unlock: Level 1
- Mana Cost: 15
- AP Cost: 2
- Cooldown: 2.5 rounds
- Range: 5 hexes max
- Rules: Fire an arrow in a straight line in the chosen direction. The arrow travels up to 5 hexes or until it hits an enemy hero. The first enemy hero struck takes damage and is stunned. Stun duration increases based on how far the arrow traveled before impact. Enemies may use the Dodge Skillshot reaction to attempt to avoid the arrow.
- Scaling: 1-5: 20 damage, +3 AP stun per hex traveled | 6-11: 30 damage, +4 AP stun per hex traveled | 12+: 40 damage, +5 AP stun per hex traveled
- Notes: At max range the stun reaches 15 AP at levels 1-5, 20 AP at levels 6-11, and 25 AP at levels 12+.

3. Leap
- Type: Active
- Target: Direction/Vector
- Unlock: Level 1
- Mana Cost: 8
- AP Cost: 1
- Cooldown: 1.5 rounds
- Rules: Mirana leaps forward up to 3 hexes in a straight line to an unoccupied hex, passing over obstacles, walls, and terrain. After landing, Mirana gains bonus Attack for a short duration.
- Scaling: 1-5: +2 Attack for 10 turns | 6-11: +3 Attack for 1 round | 12+: +4 Attack for 1 round
- Notes: Leap can pass over Tree hexes and Buildings but cannot pass through Impassable terrain. If the destination hex is occupied, Mirana lands on the nearest open hex on the path.

4. Moonlight Shadow
- Type: Active
- Target: No Target (Global)
- Unlock: Level 6
- Mana Cost: 20
- AP Cost: 2
- Cooldown: 6 rounds
- Duration: 20 turns (1 round)
- Rules: Grant Invisibility to Mirana and all allied heroes on the board, regardless of position. Each hero receives their own Invisibility Cloud as per standard Invisibility rules. The invisibility lasts for the specified duration or until each hero attacks or uses a revealing ability.
- Scaling: 6-11: 20 turns (1 round) duration | 12-17: 30 turns (1.5 rounds) duration | 18+: 40 turns (2 rounds) duration

Upgrade / notes panel:
- Aghanim's Scepter Upgrade: The current level of Starfall is applied to all enemy units along the path of Sacred Arrow and 1 hex adjacent.

Graphic direction:
- The card should feel like a technical tabletop rules reference first, fantasy illustration second
- Use a wide landscape layout with strong horizontal row separation and consistent icon chips
- Keep the text area bright and readable with minimal texture behind it
- Include subtle moon sigils, star patterns, celestial arcs, arrow-flight motifs, and wind-swept movement accents without reducing clarity
- Ensure the color story, border finish, chip styling, and spell-effect rendering clearly match the attached Hero Card reference
- The look of Starfall, Sacred Arrow, Leap, and Moonlight Shadow should feel like direct spell extensions of the attached Hero Card art rather than newly invented visual languages
- Present as a straight-on flat card render on a neutral background

Typography direction:
- Elegant fantasy title for the hero name
- Clear section titles for each ability
- Compact, highly legible game UI font for rules text and numbers
- Costs, timing information, and scaling values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the four-row structure, typography hierarchy, or cost strip order
- Do not arrange the abilities in a 2x2 grid, card quadrant layout, or any multi-column panel system
- Do not turn the card into a hero card, poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not use a large full-card portrait in place of rules text space
- Do not drift away from the attached Hero Card's visual language for spell motifs, icon treatment, palette behavior, or ornamental detailing
- Do not copy official game splash art or spell icons
- Do not add current cooldown markers, current mana trackers, AP trackers, or board-state counters
- Do not invent extra mechanics, extra scaling tiers, or extra decorative clutter
```

---

## Reusable Prompt — Mirana-Style Hero Card Look

Use the following prompt when you want to reproduce the overall hero-card layout and finish shown by the Mirana example, while changing the hero identity and data:

```text
Create a polished fantasy board game hero card in portrait orientation, designed for a 10 × 15 cm printed card. Use the exact same overall layout logic, spacing rhythm, readability standards, and premium finish as the Mirana example card style.

This is a Dota-inspired board game component, but all artwork must be original and should not copy official Valve or Dota 2 art.

Use the Mirana example as the locked manufacturing template. Preserve the same card architecture, typography hierarchy, icon order, panel spacing, and straight-on flat component view. Only change portrait artwork, accent palette, emblem, and hero-specific atmospheric details.

Style target:
- Premium tabletop card design with a clean, modern fantasy UI
- Deep navy-blue outer frame with soft gradients and thin silver border lines
- Rounded corners and elegant beveled panel dividers
- Strong readability at print size
- Straight-on flat card render, not a 3D mockup
- Clear separation between portrait area, stat strip, progression strip, and four ability rows
- Refined, slightly luminous fantasy finish rather than gritty realism
- Consistent icon language across stats and abilities

Match the Mirana example's layout structure:
- Large top name banner spanning full width
- Circular emblem space in the top left and top right corners
- Small class ribbon below the name banner on the left
- Small attack-type badge below that
- Role tags aligned at the top of the portrait panel on the right
- Large illustrated portrait window occupying the upper half of the card
- Wide stat strip beneath the portrait with bold icon + number columns
- Narrow progression strip beneath the stats showing per-level scaling and level milestones
- Four horizontal ability panels stacked vertically in the lower half
- Each ability panel uses a left-side ability icon medallion and a clean text box to the right

Visual characteristics to preserve:
- Crisp white or off-white text on dark blue headers
- White rules text areas with subtle cool tinting
- Blue ability panel headers and separators
- Elegant serif or fantasy title font for hero name
- Compact readable game UI font for rules text
- Bright, high-contrast stat icons
- Thin dividers and a premium board-game graphic design feel
- Slight celestial / magical glow treatment without becoming noisy

Composition rules:
- The card should feel like a readable tabletop component first, illustration showcase second
- Portrait art should be large and dramatic but must not overpower the rules layout
- Text should be aligned cleanly and consistently with minimal clutter
- Ability rows should be symmetrical and easy to scan quickly
- Stats should read instantly from left to right

Do preserve these specific style signals from the Mirana example:
- Dark blue overall frame
- Silver trim and panel outlines
- Top banner with centered hero name
- Class ribbon and role tags as compact badges
- Portrait framed inside a soft-edged rectangular illustration window
- White stat numbers paired with colorful icons on a dark stat bar
- Slim progression bar with level milestone icons
- Ability rows with icon on the left, key numbers on the top line, and summary/scaling below

Do not preserve Mirana-specific content unless explicitly provided:
- Do not keep Mirana's name, portrait, stats, class, or abilities by default
- Do not keep moon symbols, lunar motifs, or her color storytelling unless requested
- Replace all hero-specific art and text with the supplied hero data

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the stat strip order, typography hierarchy, or four-row ability layout
- Do not introduce new decorative badges, alternate UI systems, or extra card zones
- Do not turn the card into a poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not use a trading card game frame style
- Do not make it look like a mobile game screenshot
- Do not create fake foil glare, lens flare, or heavy texture noise
- Do not overdecorate the text areas
- Do not add tracker dials, counters, or board-state tokens on the card
- Do not copy the Mirana artwork directly; only match the design language and layout system
```

---

## Reusable Prompt Template — Mirana-Style Hero Card Generation

Use the following prompt to generate a blank hero card template in the same style as the Mirana example, with all hero-specific content areas intentionally left empty for later manual fill-in:

```text
Create a polished fantasy board game hero card in portrait orientation, designed for a 10 × 15 cm printed card. Use the same visual style, layout structure, spacing, and readability standard as the Mirana example hero card: premium navy-blue frame, silver trim, elegant fantasy UI, strong panel hierarchy, crisp icons, and flat straight-on presentation.

This is a Dota-inspired board game component, but all artwork must be original and should not copy official Valve or Dota 2 art.

Treat the Mirana example as a locked manufacturing template. Preserve the frame, panel layout, typography hierarchy, icon order, spacing rhythm, and overall card architecture exactly while leaving hero-specific content blank.

Overall visual style:
- Premium tabletop component first, fantasy illustration second
- Dark navy frame with silver borders and clean panel separators
- Centered hero name banner at top
- Class ribbon, attack-type badge, and role tags in compact badge format
- Large portrait window in the upper half
- Dark stat strip with bright icon-and-number columns
- Narrow progression strip with per-level scaling and milestone icons
- Four stacked ability rows in the lower half, each with an icon medallion on the left and rules text to the right
- High contrast, readable at print size, elegant but controlled magical finish

Template requirement:
- Do not fill in any hero-specific text or numbers
- Leave all hero-specific information areas blank so they can be filled in later by hand or in a separate design pass
- Preserve the full layout structure and visual hierarchy even when the fields are empty

Leave these sections blank:
- Hero name banner
- Class ribbon text
- Attack type badge text
- Role tag text
- Portrait window content
- Base stat values
- Per-level stat gain text
- Scepter reminder area
- All four ability names
- Ability type, target, and special tags
- Unlock values
- Mana, AP, cooldown, range, and duration values
- Ability summaries
- Scaling lines

Portrait direction:
- Leave the portrait window empty or use a very subtle neutral placeholder frame with no character art
- Do not insert a generic hero illustration
- The portrait area should clearly remain reserved for future art

Base stats area:
- Keep the stat strip structure intact
- Show the icon positions and panel divisions
- Leave the numerical values blank
- Do not substitute zeros, dashes, or fake sample numbers unless absolutely needed for layout readability

Progression strip:
- Keep the per-level text area blank
- Keep milestone icons for Level 6, Level 12, and Level 18 visible as part of the template structure
- Keep the Scepter badge space present but unlabeled or blank

Ability rows:
- Include four stacked ability panels
- Keep the icon medallion space on the left of each row
- Keep all text boxes and chip positions visible
- Leave the ability names blank
- Leave the type, target, unlock, and special-tag areas blank
- Leave mana, AP, cooldown, range, and duration fields blank
- Leave summary and scaling text areas blank
- Do not populate the rows with fake ability names or lorem ipsum

Graphic direction:
- Preserve the Mirana example's overall card architecture exactly
- Keep the card visually complete as a premium template, but content-empty
- Use clear panel separation and consistent icon chips
- Keep the card uncluttered and legible
- Present as a straight-on flat card render on a neutral background
- Include subtle tactical board game icon language such as hex motifs, range markers, and clean ability chips

Typography direction:
- Large elegant fantasy title for the hero name
- Clean compact sans-serif or readable game UI font for rules text
- Important values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the stat strip order, typography hierarchy, or four-row ability layout
- Do not introduce new decorative badges, alternate UI systems, or extra card zones
- Do not turn the card into a poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not copy official game splash art
- Do not use a trading card game frame style
- Do not make it look like a mobile game screenshot
- Do not add extra abilities, extra stats, or extra decorative clutter
- Do not place current HP, current Mana, gold, XP, cooldown trackers, or item slots on the card
- Do not fill blank fields with sample values, placeholder names, lorem ipsum, or random symbols
- Do not change the Mirana example's layout logic; only convert it into a clean blank template
```

---

## Example Image Prompt — Sven Hero Card

Use the following prompt when generating a sample hero card image for Sven:

```text
Create a polished fantasy board game hero card in portrait orientation, designed for a 10 × 15 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the Mirana example hero card. Keep this visually part of the same manufactured hero-card product family.

Overall style: premium tabletop card design, clean information hierarchy, readable at print size, heavy knight-warrior theme, strength-class visual identity, steel blue, crimson, bronze, and storm-lit highlights, crisp iconography, high contrast text panels, collectible but practical.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, name banner position, class ribbon position, attack-type badge position, role tag position, portrait window position and proportions, stat strip position and icon order, progression strip position, four-row ability grid structure, typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view established by the Mirana example.
- Only change the portrait artwork, accent palette, emblem, and hero-specific atmospheric details inside the established frame.

Card structure:
- Top banner with the name: SVEN
- Strength class band in red
- Attack type badge: Melee
- Role tags: Carry, Durable, Initiator
- Large central portrait of Sven as an original armored rogue knight: imposing greatsword, heavy plate armor, horned helm or masked face, storm-charged atmosphere, broad stance, disciplined but brutal presence
- Horizontal stat strip below portrait with large readable icons and numbers
- Narrow progression strip
- Bottom half contains four compact ability summary rows with chips for unlock level, type, and target only

Base stats to show exactly:
- HP 100
- Mana 30
- Attack 10
- Attack Range 1 hex
- Defense 3
- Move Speed 1
- AP 10

Progression strip:
- Per Level: +10 HP | +10 Mana | +5 ATK | +1 DEF
- Milestone icons for Level 6, Level 12, Level 18
- Scepter badge reminder

Ability summary rows to display:

1. Storm Hammer
- Type: Active
- Target: Unit Target
- Unlock: Level 1
- Summary: Hurl a magical hammer that damages the target and stuns nearby enemies.

2. Great Cleave
- Type: Passive
- Unlock: Level 1
- Summary: Sven's attacks cleave in a cone for efficient wave damage.

3. Warcry
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 1
- Summary: Grant Sven and nearby allies bonus Defense and Move Speed.

4. God's Strength
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 6
- Summary: Gain a massive Attack boost that also increases Great Cleave damage.

Graphic direction:
- The card should feel like a readable tabletop component first, illustration showcase second
- Use clear panel separation and consistent icon chips
- Emphasize heavy armor, giant sword silhouette, storm energy, martial discipline, and a late-game powerhouse identity
- Keep the layout uncluttered and legible; no fake tracker dials, no board-game counters, no 3D mockup angle
- Present as a straight-on flat card render on a neutral background
- Include subtle hex motifs and tactical board game icon language for stun, buff aura, and cone attacks

Typography direction:
- Large, bold fantasy title for the hero name
- Clean, compact sans-serif or highly readable game UI font for rules text
- Important values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the stat strip order, typography hierarchy, or four-row ability layout
- Do not introduce new decorative badges, alternate UI systems, or extra card zones
- Do not turn the card into a poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not print full numerical rules text, costs, cooldowns, or scaling values on the hero card
- Do not copy official game splash art
- Do not use a trading card game frame style
- Do not make it look like a mobile game screenshot
- Do not add extra abilities, extra stats, or extra decorative clutter
- Do not place current HP, current Mana, gold, XP, cooldown trackers, or item slots on the card
```

---

## Example Image Prompt — Sven Abilities Card

Use the following prompt when generating a sample landscape Abilities Card image for Sven:

```text
Create a polished fantasy board game abilities reference card in landscape orientation, designed for a 15 × 10 cm printed card. This is a Dota-inspired board game component, but the artwork must be original and should not copy official Valve or Dota 2 art.

Use the attached Sven Hero Card image as the primary visual reference for this Abilities Card. Match its card family exactly: same design language, same frame sensibility, same typography hierarchy, same icon rendering style, same accent palette logic, same material finish, and the same treatment of storm energy, knightly steel, heavy weapon silhouettes, martial buffs, and explosive impact effects. The Abilities Card should look like it was manufactured as a companion component to that exact Hero Card, not merely a related card from a similar set.

Use the same card architecture, typography hierarchy, icon order, spacing rhythm, and panel system as the established landscape Abilities Card template for this game. Keep this visually part of the same manufactured product family as the attached Hero Card while clearly functioning as a rules reference.

Overall style: premium tabletop reference component, rules-forward layout, highly readable at print size, heavy knight-warrior theme, strength-class visual identity, steel blue, crimson, bronze, and storm-lit highlights, clean dividers, restrained magical texture, crisp iconography, collectible but practical.

This is an Abilities Card, not a Hero Card. The card should prioritize gameplay clarity, full rules readability, and explicit numerical values over portrait space.

Locked layout instruction:
- Preserve the exact outer frame shape, border treatment, hero header position, summary strip position, and a four-row stacked ability layout with one ability per horizontal row. Preserve the typography system, divider thickness, corner treatment, panel spacing, and straight-on flat component view across all Abilities Cards.
- Derive the small hero portrait or crest, ability icons, accent palette, and hero-specific atmospheric details directly from the attached Hero Card so the spell visuals feel like the same hero package.
- Make the hammer silhouette, cleave arcs, war-banner buff motifs, storm glow, and heavy melee impact language visually consistent with what appears on the attached Hero Card.

Card structure:
- Hero header with the name: SVEN
- Small crest or portrait accent
- Summary strip listing Storm Hammer, Great Cleave, Warcry, God's Strength
- Four clearly separated horizontal ability rows, one per ability, each with icon, type, target, costs, rules text, and scaling
- Upgrade / notes panel for key reminders
- Small footer legend for icon language if needed

Ability data to show exactly:

1. Storm Hammer
- Type: Active
- Target: Unit Target
- Unlock: Level 1
- Mana Cost: 10
- AP Cost: 1
- Cooldown: 2 rounds
- Range: 2 hexes
- Rules: Hurl a magical hammer at target unit, dealing damage and stunning all enemy units within 1 hex of the target. Can be disjointed by Blink and similar displacement effects using a reaction.
- Scaling: 1-5: 20 damage, stun (10 AP loss) | 6-11: 30 damage, stun (15 AP loss) | 12+: 40 damage, stun (20 AP loss)

2. Great Cleave
- Type: Passive
- Unlock: Level 1
- Rules: Sven's attacks cleave in a 2-hex cone in front of him, dealing damage to all units in the area. When Sven uses Farm on a creep wave, he only needs to farm twice to clear the entire wave and receives the gold and XP for all creeps.
- Scaling: 1-5: 2 cleave damage | 6-11: 4 cleave damage | 12+: 6 cleave damage

3. Warcry
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 1
- Mana Cost: 1
- AP Cost: 1
- Cooldown: 3 rounds
- Duration: 1 round
- Range: 3 hex aura to allies
- Rules: Sven and all allied heroes within 3 hexes gain bonus Defense and Move Speed for the duration. Does not affect creeps.
- Scaling: 1-5: +5 Defense, +1 Move Speed | 6-11: +10 Defense, +1 Move Speed | 12+: +10 Defense, +2 Move Speed

4. God's Strength
- Type: Active
- Target: No Target (Self-Cast)
- Unlock: Level 6
- Mana Cost: 2
- AP Cost: 2
- Cooldown: 4 rounds
- Duration: 1 round
- Rules: Sven channels his rogue knight's fury, gaining bonus Attack for the duration. Great Cleave damage is also increased by the same amount.
- Scaling: 6-11: +10 Attack | 12-17: +20 Attack | 18+: +40 Attack

Upgrade / notes panel:
- Aghanim's Scepter Upgrade: Sven may choose to travel with Storm Hammer, arriving at the impact location. Impact damage increases to 60.

Graphic direction:
- The card should feel like a technical tabletop rules reference first, fantasy illustration second
- Use a wide landscape layout with strong horizontal row separation and consistent icon chips
- Keep the text area bright and readable with minimal texture behind it
- Include subtle hammer motifs, storm arcs, knightly trim, cleave sweeps, and martial insignia without reducing clarity
- Ensure the color story, border finish, chip styling, and spell-effect rendering clearly match the attached Hero Card reference
- The look of Storm Hammer, Great Cleave, Warcry, and God's Strength should feel like direct spell extensions of the attached Hero Card art rather than newly invented visual languages
- Present as a straight-on flat card render on a neutral background

Typography direction:
- Bold fantasy title for the hero name
- Clear section titles for each ability
- Compact, highly legible game UI font for rules text and numbers
- Costs, timing information, and scaling values should be instantly scannable

Negative constraints:
- Do not redesign the frame or reposition any major card elements
- Do not change the four-row structure, typography hierarchy, or cost strip order
- Do not arrange the abilities in a 2x2 grid, card quadrant layout, or any multi-column panel system
- Do not turn the card into a hero card, poster, splash art, mobile UI, TCG variant, 3D mockup, or photographed object
- Do not use a large full-card portrait in place of rules text space
- Do not drift away from the attached Hero Card's visual language for spell motifs, icon treatment, palette behavior, or ornamental detailing
- Do not copy official game splash art or spell icons
- Do not add current cooldown markers, current mana trackers, AP trackers, or board-state counters
- Do not invent extra mechanics, extra scaling tiers, or extra decorative clutter
```
