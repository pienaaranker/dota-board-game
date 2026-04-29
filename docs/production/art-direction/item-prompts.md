# Item Prompts

This file defines a reusable prompt system for generating **item card physical-design images** for the project.

The goal is to make item prompts easy to reuse across a large item pool without the layout drifting from one card to the next.

Use this file when generating:
- full item card concept images
- final item card art-direction prompts
- print-facing item card mock reference images

Do **not** use this file for token sheets. Token prompts belong in [token-prompts.md](token-prompts.md).

---

## Prompt Strategy

For item cards, use the same discipline already used for hero-card prompts:

1. **Locked System Layer**
2. **Controlled Flavor Layer**
3. **Anti-Drift Layer**

This keeps every item card inside one manufactured product family instead of becoming a set of unrelated fantasy posters.

---

## 1. Locked System Layer

These elements should stay effectively identical across all item cards:

- card size and orientation
- front and back use the exact same physical dimensions
- front and back share the same product-family frame language
- outer frame shape and border treatment
- name banner position and scale
- cost badge position
- type line position
- illustration window position and proportions
- rules-text panel position and proportions
- icon chip position for AP, cooldown, charges, range, duration, or other standard item metadata
- typography hierarchy
- divider thickness, corner treatment, and spacing rhythm
- overall render angle: always straight-on, flat component view

Think of this as the item's manufactured card frame. The prompt should not invite the model to redesign it.

### Recommended Physical Card Size

Use one consistent physical size across the entire item set.

- **Recommended format:** standard landscape item card
- **Recommended size:** **63 × 41 mm** (**W × H**)
- **Front purpose:** fast table readability during play
- **Back purpose:** full mechanical detail and reminder text
- **Board orientation:** cards are printed and used in **landscape orientation** on the Hero Board

If you later choose a different production size, update the prompts once and keep that new size locked across all future item cards.

---

## 2. Controlled Flavor Layer

These elements may vary from item to item, but only inside the locked frame:

- the item illustration itself
- accent palette
- material identity: glass, iron, rune-stone, cloth, bone, gold, crystal, smoke, paper, etc.
- magical effect treatment around the object
- subtle background motif behind the illustration
- rarity or power mood, if that exists in the final item system

The layout should stay fixed while the object's silhouette, materials, and magical identity do the differentiation work.

---

## 3. Anti-Drift Layer

Every reusable item prompt should explicitly forbid these kinds of drift:

- redesigning the card frame
- moving major zones around
- changing the typography hierarchy
- inventing extra badges, meters, or UI panels
- turning the card into a poster, splash art, or mobile-game UI
- turning the card into a photographed object or 3D mockup
- copying official Dota 2 item art, logos, or Valve UI
- filling the layout with decorative clutter that reduces print readability

---

## Recommended Item Flavor Budget

To keep the set cohesive, constrain each item prompt to:

- **1 primary material identity**
- **1 accent palette**
- **1 magical effect family**
- **1 subtle background motif**

That is enough to make items distinct without letting the frame mutate.

---

## Item-Type Direction

Use the same card system for every item, but adjust the flavor emphasis slightly by item type.

| Item Type | Visual Emphasis |
|---|---|
| **Consumable** | Clear object silhouette, immediate usability, bright readable effect, lighter visual density |
| **Passive** | Stable equipment identity, craftsmanship, readability, less motion |
| **Active** | Stronger magical activation cues, more energy or glow around the object |
| **Consumable (Placeable)** | Object plus deployment identity; ward, totem, beacon, trap, or placed utility feel |
| **Channeled** | Object plus sustained magical state; active energy, ritual lines, or ongoing beam / portal cue |
| **Passive / Active** | Equipment identity first, activated state second |

---

## Recommended Prompt Formula

Build item prompts in this order:

1. **Component family instruction**
2. **Physical size and double-sided instruction**
3. **Locked layout instruction**
4. **Front or back data block**
5. **Flavor instruction**
6. **Negative constraints**

That order matters. If flavor comes too early, the model starts redesigning the card instead of dressing the existing system.

---

## Reusable Master Constraint Block

Use this near the end of every item prompt:

```text
Keep this double-sided item card in the exact same product family as the approved item-card template or reference card. Preserve the front/back frame language, panel layout, typography hierarchy, metadata-chip system, spacing rhythm, and overall card architecture. Only vary the item illustration, accent palette, material identity, and item-specific atmospheric details. Do not redesign the structure.
```

---

## Front vs Back Design Roles

The two faces should have different jobs.

### Front Face

The front is for **immediate tabletop scanning**.

Keep only the information a player needs to identify and use the item quickly:

- item name
- item cost
- item type
- cooldown or charge information when immediately relevant
- 1 short rules summary or a few short effect bullets
- object illustration
- small metadata chips for AP, cooldown, charges, range, or duration

The front should avoid long paragraphs.

### Back Face

The back is for a **blank styled reverse side**.

It should preserve the same manufactured family identity as the front while remaining intentionally empty so text can be added later in layout software.

Keep only the structural and decorative elements that help it read as the reverse side of the same card:

- matching outer border and corner treatment
- matching ornament language
- matching palette family
- optional faint watermark or subtle background motif
- large clean central empty area for later text placement

The back should look visually related to the front, but it should not pre-print rules text, section labels, headers, or dense information blocks.

---

## Reusable Item Card Front Prompt Template

Copy this block and replace the bracketed fields.

```text
Create the **front face** of a polished double-sided fantasy board game item card in landscape orientation, designed for **63 × 41 mm** print size. This is a Dota-inspired board game component, but the artwork must be original and must not copy official Valve or Dota 2 item art, logos, UI, or splash imagery.

ATTACHMENTS PROVIDED
- Attachment 1: approved item-card wireframe or item-card layout reference
- Attachment 2: approved hero card or component for product-family style reference only
- Attachment 3: optional additional style reference for material finish and ornament language only

Use the attached references only as product-family guidance for layout discipline, ornament restraint, material finish, icon quality, typography hierarchy, and overall tabletop cohesion. Do not copy any copyrighted symbols, portraits, logos, or official item artwork.

PRIMARY GOAL
Generate a clean, print-ready **front face** for [ITEM NAME].

OVERALL STYLE
- premium fantasy board game component
- readable at print size
- clean information hierarchy
- elegant manufactured card frame
- high-contrast text panels
- collectible but practical
- original art only
- designed for quick table scanning during play

LOCKED LAYOUT REQUIREMENTS
- Preserve the attached **front-face** item-card architecture exactly.
- Keep the same physical card proportions, outer frame shape, border treatment, name banner position, cost badge position, type line position, illustration window position and proportions, short-rules panel position, metadata-chip positions, divider rhythm, corner treatment, and overall straight-on flat component view.
- Do not redesign the page architecture.
- Do not add new card zones.
- Only change the item illustration, accent palette, material identity, and item-specific atmospheric details inside the established frame.

FRONT-FACE DATA
- Item name: [ITEM NAME]
- Cost: [COST]
- Type: [TYPE]
- Immediately relevant info to show on front: [SHORT RULES TEXT OR 1 TO 3 SHORT EFFECT BULLETS]
- Standard metadata chips to show if relevant: [AP cost] | [Cooldown] | [Charges] | [Range] | [Duration]
- Optional subtype or keyword chips: [Placeable] | [Channeled] | [Aura] | [Passive] | [Consumable]

ITEM ILLUSTRATION DIRECTION
- Show [ITEM NAME] as an original fantasy object, not as copied game art.
- Primary object identity: [SHORT OBJECT DESCRIPTION]
- Primary material identity: [GLASS / STEEL / GOLD / CLOTH / CRYSTAL / STONE / SMOKE / PAPER / ETC.]
- Accent palette: [PALETTE]
- Magical effect family: [ARCANE GLOW / HOLY LIGHT / SHADOW MIST / FROST ENERGY / LIGHTNING / WARP / ETC.]
- Background motif: [SUBTLE PATTERN OR ENVIRONMENTAL SHAPE]
- Mood: [UTILITY / VIOLENT / MYSTICAL / DIVINE / TACTICAL / STEALTH / ETC.]

GRAPHIC DIRECTION
- The card should feel like a readable tabletop component first and a fantasy illustration second.
- Keep the object silhouette immediately legible.
- Use clean panel separation and crisp metadata chips.
- Keep front-face text intentionally limited.
- The front should prioritize fast recognition over full rules explanation.
- Let the illustration sit inside the manufactured card system rather than breaking out of it.
- Present as a straight-on flat card render on a neutral background.
- Keep iconography, numerals, and text highly readable.

TYPOGRAPHY DIRECTION
- Large readable fantasy title for the item name.
- Clean compact game-ui text for rules text.
- Important numeric values should be instantly scannable.

MANUFACTURING MINDSET
- This should look like a final tabletop product component, not concept art pasted onto a card.
- The front and back are a matched printed pair.
- The frame is standardized across the entire item set.
- The object illustration and accent treatment are the custom layer on the front.

MASTER CONSTRAINT
Keep this double-sided item card in the exact same product family as the approved item-card template or reference card. Preserve the front/back frame language, panel layout, typography hierarchy, metadata-chip system, spacing rhythm, and overall card architecture. Only vary the item illustration, accent palette, material identity, and item-specific atmospheric details. Do not redesign the structure.

NEGATIVE CONSTRAINTS
- Do not redesign the frame.
- Do not move major card elements.
- Do not add extra stats, extra panels, fake rarity systems, or decorative UI clutter.
- Do not turn the card into a poster, splash art, mobile UI, trading card, photographed object, angled mockup, or 3D render presentation.
- Do not copy official Dota 2 item art, icons, logos, or Valve UI.
- Do not use muddy low-contrast effects that reduce print legibility.
- Do not let special effects overpower the object silhouette.
- Do not place the card in an environment or tabletop scene.

FINAL OUTPUT TARGET
The final image should look like a production-quality printable **front face** for a premium fantasy board game item card: clean, aligned, readable, visually cohesive with the rest of the product line, and optimized for fast tabletop scanning.
```

---

## Reusable Item Card Back Prompt Template

Copy this block and replace the bracketed fields.

```text
Create the **back face** of a polished double-sided fantasy board game item card in landscape orientation, designed for **63 × 41 mm** print size. This is a Dota-inspired board game component, but the artwork must be original and must not copy official Valve or Dota 2 UI, logos, or official art.

ATTACHMENTS PROVIDED
- Attachment 1: approved item-card wireframe or item-card layout reference
- Attachment 2: approved front-face item card from the same item set for style matching
- Attachment 3: optional additional component reference for typography or ornament language only

Use the attached references only as product-family guidance for layout discipline, ornament restraint, typography hierarchy, frame language, and overall tabletop cohesion. Do not copy any copyrighted symbols, logos, or official item art.

PRIMARY GOAL
Generate a clean, print-ready **back face** for [ITEM NAME] that matches the front-face design system while remaining completely blank apart from the border, frame language, and very subtle supporting style details.

OVERALL STYLE
- premium fantasy board game component
- readable at print size
- same product family as the front face
- cleaner and more minimal than the front
- original art only

LOCKED LAYOUT REQUIREMENTS
- Preserve the attached **back-face** item-card architecture exactly.
- Keep the same physical card proportions and same manufactured family identity as the front.
- Use a matching border treatment, matching ornament system, matching typography hierarchy, and matching color-family logic.
- Preserve a large clean empty interior area for later manual text placement.
- Do not redesign the page architecture.
- Do not overload the back with illustration, labels, or printed information.

BACK-FACE DATA
- Do not print any rules text on the generated back.
- Do not print section headers.
- Do not print item metadata unless explicitly requested later.
- Leave the central content area blank for later layout insertion.

BACK-FACE ART DIRECTION
- Use only subtle art support on the back.
- Include a faint watermark, emblem, rune pattern, item silhouette ghost, or decorative motif related to [ITEM NAME].
- Keep the back primarily optimized as a blank styled surface for later text insertion.
- Accent palette: [PALETTE]
- Motif: [SUBTLE MOTIF]
- Mood: [MOOD]

GRAPHIC DIRECTION
- The back should feel like a blank production-ready reverse face, not a populated rules reference.
- Leave generous, clearly bounded empty space.
- Make it easy to overlay or insert text later without fighting the art.
- Avoid printed separators, labels, or text scaffolding inside the empty area.
- Present as a straight-on flat card render on a neutral background.

TYPOGRAPHY DIRECTION
- Preserve the same typography family as the front only where tiny decorative lettering is required by the frame.
- Do not pre-populate the back with item name, rules text, or body text blocks.

MANUFACTURING MINDSET
- The back must look like the reverse side of the same printed card, not a separate product.
- The back exists as a styled blank template, not a finished rules surface.
- Ornament should frame the empty area, not compete with future inserted text.

MASTER CONSTRAINT
Keep this double-sided item card in the exact same product family as the approved item-card template or reference card. Preserve the front/back frame language, panel layout, typography hierarchy, metadata-chip system, spacing rhythm, and overall card architecture. Only vary the subtle motif, accent palette, and item-specific atmospheric details. Do not redesign the structure.

NEGATIVE CONSTRAINTS
- Do not redesign the frame.
- Do not move major card elements.
- Do not fill the back with large illustration that reduces usable blank space.
- Do not create a poster-like composition.
- Do not add fake parchment clutter, unreadable texture, section headers, rules text, labels, or busy effects inside the blank area.
- Do not turn the card into a photographed object, angled mockup, or 3D render presentation.
- Do not copy official Dota 2 UI, logos, or item art.

FINAL OUTPUT TARGET
The final image should look like a production-quality printable **back face** for a premium fantasy board game item card: clean, aligned, clearly related to the front face, and intentionally blank apart from the frame, border, and subtle style treatment so text can be added later.
```

---

## Short Front Fill-In Template

Use this shorter version when you already have a stable card system and just need to swap item data quickly.

```text
Create a print-ready **front face** for [ITEM NAME]. Use the exact same double-sided item-card architecture, front-face frame, typography hierarchy, metadata-chip system, spacing rhythm, and physical size as the approved template. Only change the item illustration, accent palette, material identity, and item-specific atmospheric details.

Front data:
- Name: [ITEM NAME]
- Cost: [COST]
- Type: [TYPE]
- Short front text: [SHORT RULES TEXT]
- Metadata chips: [AP] [Cooldown] [Charges] [Range] [Duration]

Art direction:
- Object identity: [OBJECT DESCRIPTION]
- Materials: [MATERIALS]
- Palette: [PALETTE]
- Effect family: [EFFECT]
- Background motif: [MOTIF]
- Mood: [MOOD]

Constraints:
- Original art only
- No frame redesign
- No extra UI systems
- No official Dota 2 art or logos
- Straight-on flat component render
- Readable at print size
- Fast tabletop scanning
```

---

## Short Back Fill-In Template

Use this when you want the reverse side quickly.

```text
Create a print-ready **back face** for [ITEM NAME]. Use the exact same double-sided item-card architecture, back-face frame language, typography hierarchy, spacing rhythm, and physical size as the approved template. Match the front-face style, but keep the back completely blank apart from the border, frame, and subtle decorative treatment.

Back data:
- No printed text
- No section labels
- Leave clean blank space for later insertion

Back art direction:
- Accent palette: [PALETTE]
- Subtle motif or watermark: [MOTIF]
- Mood: [MOOD]

Constraints:
- Original art only
- No frame redesign
- No printed rules text or labels
- No busy illustration in the blank area
- Same product family as the front
- Straight-on flat component render
- Optimized as a styled blank reverse side for easy later text insertion
```

---

## Example Front Template Fill — Bottle

Use this as a model for how much detail to give the system.

```text
Create the **front face** of a polished double-sided fantasy board game item card in landscape orientation, designed for **63 × 41 mm** print size. This is a Dota-inspired board game component, but the artwork must be original and must not copy official Valve or Dota 2 item art, logos, UI, or splash imagery.

ATTACHMENTS PROVIDED
- Attachment 1: approved item-card wireframe or item-card layout reference
- Attachment 2: approved hero card or component for product-family style reference only

PRIMARY GOAL
Generate a clean, print-ready **front face** for Bottle.

OVERALL STYLE
- premium fantasy board game component
- readable at print size
- clean information hierarchy
- elegant manufactured card frame
- high-contrast text panels
- collectible but practical
- original art only
- designed for quick table scanning during play

LOCKED LAYOUT REQUIREMENTS
- Preserve the attached **front-face** item-card architecture exactly.
- Keep the same physical card proportions, outer frame shape, border treatment, name banner position, cost badge position, type line position, illustration window position and proportions, short-rules panel position, metadata-chip positions, divider rhythm, corner treatment, and overall straight-on flat component view.
- Only change the item illustration, accent palette, material identity, and item-specific atmospheric details inside the established frame.

FRONT-FACE DATA
- Item name: Bottle
- Cost: 70 Gold
- Immediately relevant info to show on front:
	- 3 Charges (use charges icon)
	- +10hp (use healh icon)
	- +6mp (use mana icon)
	- per 1/2 round (use half round indicator icon)

ITEM ILLUSTRATION DIRECTION
- Show Bottle as an original fantasy glass flask designed for a tactical board game economy item.
- Primary object identity: compact potion bottle with a rune-lock stopper and visible glowing liquid reserve
- Primary material identity: blue-tinted glass, silver neck fittings, arcane cork or metal seal
- Accent palette: aqua, sapphire, silver, faint rune-white highlights
- Magical effect family: contained liquid glow and subtle rune resonance
- Background motif: gentle circular rune rings and faint river-energy pattern
- Mood: practical, magical, versatile, valuable utility item

GRAPHIC DIRECTION
- The card should feel like a readable tabletop component first and a fantasy illustration second.
- Keep the bottle silhouette instantly legible.
- Use clean panel separation and crisp metadata chips.
- Keep front-face text intentionally limited.
- Present as a straight-on flat card render on a neutral background.

MASTER CONSTRAINT
Keep this double-sided item card in the exact same product family as the approved item-card template or reference card. Preserve the front/back frame language, panel layout, typography hierarchy, metadata-chip system, spacing rhythm, and overall card architecture. Only vary the item illustration, accent palette, material identity, and item-specific atmospheric details. Do not redesign the structure.

NEGATIVE CONSTRAINTS
- Do not redesign the frame.
- Do not move major card elements.
- Do not add extra stats, extra panels, fake rarity systems, or decorative UI clutter.
- Do not turn the card into a poster, splash art, mobile UI, photographed object, angled mockup, or 3D render presentation.
- Do not copy official Dota 2 item art, icons, logos, or Valve UI.

FINAL OUTPUT TARGET
The final image should look like a production-quality printable **front face** for a premium fantasy board game item card: clean, aligned, readable, visually cohesive with the rest of the product line, and optimized for fast tabletop scanning.
```

---

## Example Back Template Fill — Bottle

Use this as a model for a matching reverse side.

```text
Create the **back face** of a polished double-sided fantasy board game item card in landscape orientation, designed for **63 × 41 mm** print size. This is a Dota-inspired board game component, but the artwork must be original and must not copy official Valve or Dota 2 UI, logos, or official art.

ATTACHMENTS PROVIDED
- Attachment 1: approved item-card wireframe or item-card layout reference
- Attachment 2: approved front-face Bottle card for style matching

PRIMARY GOAL
Generate a clean, print-ready **back face** for Bottle that matches the front-face design system while remaining completely blank apart from the border, frame language, and very subtle supporting style details.

OVERALL STYLE
- premium fantasy board game component
- readable at print size
- same product family as the front face
- cleaner and more minimal than the front
- original art only

LOCKED LAYOUT REQUIREMENTS
- Preserve the attached **back-face** item-card architecture exactly.
- Keep the same physical card proportions and same manufactured family identity as the front.
- Use a matching border treatment, matching ornament system, matching typography hierarchy, and matching color-family logic.
- Preserve a large clean empty interior area for later manual text placement.
- Do not overload the back with illustration, labels, or printed information.

BACK-FACE DATA
- Do not print any rules text on the generated back.
- Do not print section headers.
- Leave the central content area blank for later layout insertion.

BACK-FACE ART DIRECTION
- Use only subtle art support on the back.
- Include a faint bottle silhouette watermark, gentle circular rune rings, and a soft river-energy motif.
- Accent palette: aqua, sapphire, silver, faint rune-white highlights
- Mood: practical, magical, versatile utility item

GRAPHIC DIRECTION
- The back should feel like a blank production-ready reverse face, not a populated rules reference.
- Leave generous, clearly bounded empty space.
- Make it easy to overlay or insert text later without fighting the art.
- Present as a straight-on flat card render on a neutral background.

MASTER CONSTRAINT
Keep this double-sided item card in the exact same product family as the approved item-card template or reference card. Preserve the front/back frame language, panel layout, typography hierarchy, metadata-chip system, spacing rhythm, and overall card architecture. Only vary the subtle motif, accent palette, and item-specific atmospheric details. Do not redesign the structure.

NEGATIVE CONSTRAINTS
- Do not redesign the frame.
- Do not move major card elements.
- Do not fill the back with large illustration that reduces text space.
- Do not create a poster-like composition.
- Do not add fake parchment clutter, unreadable texture, or busy effects behind the text area.
- Do not turn the card into a photographed object, angled mockup, or 3D render presentation.

FINAL OUTPUT TARGET
The final image should look like a production-quality printable **back face** for a premium fantasy board game item card: clean, aligned, clearly related to the front face, and intentionally blank apart from the frame, border, and subtle style treatment so text can be added later.
```

---

## Usage Notes

- If the item is mechanically simple, keep the art direction short and let the object silhouette carry the card.
- If the item is information-dense, keep the front minimal and push detail to the back.
- If you generate many items in a row, keep the same attachment set and only swap the item-data and item-illustration sections.
- Reuse the same front and back template pair for the whole MVP item set.
- If a model starts drifting, strengthen the Locked Layout Requirements and Master Constraint sections rather than adding more flavor text.