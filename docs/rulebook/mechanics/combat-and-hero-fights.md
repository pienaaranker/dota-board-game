# DOTA 2: THE BOARD GAME — COMBAT AND HERO FIGHTS

This document collects combat resolution, status effects, and the shared targeting language used by hero abilities.

---

## Combat

### Damage Resolution
All combat uses the formula:

> **Damage − Defense = Health Lost**

The attacker's Damage and the defender's Defense are taken from their Hero Cards, modified by any active items and abilities.

### Line of Sight (LoS)
- **Melee Attacks** target an adjacent hex and do **not** require clear LoS.
- **Ranged Attacks and targeted Abilities** require an unobstructed line between the attacker's hex and the target's hex.
- To check LoS: draw a straight line between the two hex centres. If that line passes through any **Tree hex** or **Impassable hex**, LoS is blocked and the attack or ability cannot be used from that position.
- **AoE abilities** apply the same check per hex — only hexes with clear LoS from the caster are affected, unless the hero's Abilities Card states otherwise.

### Attack Range
- **Melee** heroes must be on a hex **adjacent** to their target to attack. No LoS required.
- **Ranged** heroes use the **attack range printed on their Hero Card** and require **clear Line of Sight** (see above).
- If a card effect changes a hero's attack range, use the modified value for as long as that effect applies.

### Crowd Control (CC)
| Status Effect | Mechanical Effect |
|---|---|
| **Stun** | Target loses AP equal to the stun value from their *next* turn. |
| **Silence** | Target cannot use abilities for the remainder of the current round and their next turn. |
| **Slow** | Defined per card — typically reduces effective movement areas per AP. |
| **DoT (Damage over Time)** | See below. |

### Damage over Time (DoT)

A DoT is a debuff token placed on a hero. At the **start of that hero's activation** (when their turn begins), the DoT deals its damage and decrements its duration by 1. When the duration reaches 0, the token is removed.

**DoT rules:**
- Each DoT token specifies: damage per tick, tick frequency (every activation or every round), and total duration.
- Most DoTs tick **once per activation** — meaning twice per round since each hero activates twice.
- Some DoTs may tick **once per round** instead — this will be clearly marked on the hero's Abilities Card or the relevant item entry.
- Multiple different DoT tokens can be active on a hero simultaneously; each ticks independently.
- The same DoT type does **not** stack — applying it again refreshes the duration instead.
- Most DoTs are **dispellable**: they can be removed by items or abilities that cleanse debuffs (e.g. Eul's Scepter of Divinity, Guardian Greaves). The relevant item entry or hero's Abilities Card will state if it dispels debuffs.
- Some DoTs are marked **undispellable** on the card or item entry — these cannot be removed early.

**Named DoT types used in this game:**

| DoT Type | Damage | Frequency | Notes |
|---|---|---|---|
| **Bleed** | X physical damage | Once per activation | Applied by Blood Grenade. Dispellable. |

### Death
When a hero's Health reaches 0 they are removed from the board and enter a respawn countdown (see Economy and Progression).

---

## Ability Types & Targeting

Hero abilities use different targeting and activation methods. This section defines how each type works in the board game context. All entries are pending design discussion.

### Activation Methods

**Passive** — Always active; no mana cost or activation required. Effect is continuous as long as the hero is alive.

**Active** — Manually cast during a hero's turn. Costs Mana and AP as printed on the hero's Abilities Card.

**Toggle** — Can only be **activated** during the hero's own turn (costs Mana and AP as printed). Once active, can be **toggled off at any time** — even during another player's turn — unless the hero is Silenced. While active, may drain Mana or Health per round. Examples: Rot, Mana Shield.

**Channeled** — Can be **activated** during the hero's own turn (costs Mana and AP as printed on the hero's Abilities Card). Once active, the hero must remain stationary and the effect persists across subsequent turns until interrupted or cancelled. **Interrupted by:** Stun, Silence, forced movement, or the target moving out of range. The casting player may **cancel the channel at any time** (like a toggle). Examples: Freezing Field, Black Hole.

### Targeting Types

**No Target (Self-Cast)** — Instant effect centered on or affecting only the caster. No targeting step required. Examples: God's Strength, Battle Hunger.

**Unit Target (Single Target)** — Targets a specific unit (ally, enemy, creep, or structure) within range and LoS. Must declare target before resolving.

**Point Target** — Player declares a specific hex within range as the target location. The effect occurs at that hex. Whether the effect is instant or has travel time is specified on the hero's Abilities Card. Examples: Light Strike Array, Ice Path.

**Direction/Vector Target** — Player declares a direction or line from the caster by specifying a target hex. How the ability resolves along that direction (instant movement, projectile, persistent zone, etc.) is specified on the hero's Abilities Card. Examples: Swashbuckle (movement + attack along direction), Macropyre (line of fire).

### Effect Shapes

**Circular AoE** — Affects all units within a fixed radius (measured in hexes) from the center point.

**Linear/Line** — Straight line from caster extending outward. Hits all units along the path.

**Cone** — Wedge-shaped area in front of the caster. Hits all units in the cone.

**Global** — Affects all enemy or allied heroes (as specified on the card) on the entire board, regardless of range or Line of Sight. No targeting step required — all valid targets are affected simultaneously. Balance is handled through the ability's damage values, mana cost, cooldown, and other printed parameters. Examples: Thundergod's Wrath, Nature's Call.

### Special Mechanics

**Skillshot** — Abilities that travel in a line from the caster to a target location and can be dodged. **Whether an ability is a skillshot must be explicitly marked on the hero's Abilities Card.** Only abilities marked as Skillshot may be dodged using the Dodge Skillshot reaction — all other abilities resolve instantly and too quickly to dodge. The caster declares a direction by specifying a target hex (using Direction/Vector targeting). The ability creates a line effect from the caster's hex toward the target hex. Any hero in the path of the skillshot (including at the end position) may use the **Dodge Skillshot** reaction (see Turn Structure) to attempt to avoid being hit. The dodge reaction costs 2 AP from the hero's next turn, requires a die roll to determine success, and forces the hero to immediately move to an adjacent hex regardless of the roll's outcome. Examples: Sacred Arrow, Meat Hook.

**Ground-Targeted AoE** — Combination of Point Target + Circular AoE. Player picks a hex; all units within the radius are affected.

**Unit-Targeted AoE** — Targets a unit; effect radiates from that unit to nearby hexes. Examples: Poison Nova, Thundergod's Wrath (per-hero basis).

**Aura** — Passive effect that continuously radiates from the hero to all allied or enemy units (as specified on the card) within a fixed range measured in hexes. The aura's radius, which units are affected (allies/enemies/both), and the specific effect are all printed on the hero's Abilities Card. Auras are always active while the hero is alive and do not require activation. Examples: Precision Aura, Vampiric Aura.
