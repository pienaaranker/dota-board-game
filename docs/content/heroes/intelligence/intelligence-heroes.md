# DOTA 2: THE BOARD GAME — INTELLIGENCE HERO CARDS

This document contains the current full card designs for Intelligence heroes.

For draft rules and class-wide roster status, see [../hero-shortlist.md](../hero-shortlist.md). For the full hero card index, see [../roster.md](../roster.md).

---

## Crystal Maiden
**Class:** Intelligence | **Attack Type:** Ranged 

### Base Stats

| Stat | Value |
|------|-------|
| **Health (HP)** | 75   |
| **Mana** | 50 |
| **Attack** | 6 |
| **Attack Range** | 3 hexes |
| **Defense** | 1 |
| **Move Speed** | 1 |
| **Action Points (AP)** | 10 |

### Stat Scaling
- **Per Level:** +10 HP, +10 Mana, +3 Attack, +1 Defense

### Abilities

---

#### Crystal Nova
**Type:** Active | **Targeting:** Ground-Targeted AoE | **Unlock:** Level 1

**Mana Cost:** 15 | **AP Cost:** 2 | **Cooldown:** 2 rounds | **Range:** 2 hexes

**Effect:**  
Blast an area with damaging frost, dealing damage to all enemy units within a 2-hex radius and applying a Slow debuff for the specified duration. Slowed enemies have their AP reduced when planning their next activation.

**Level Progression:**
- **Level 1-5:** 20 damage, -2 AP for 10 turns
- **Level 6-11:** 30 damage, -3 AP for 1 round (20 turns)
- **Level 12+:** 40 damage, -4 AP for 2 rounds (40 turns)

---

#### Frostbite
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 1

**Mana Cost:** 20 | **AP Cost:** 2 | **Cooldown:** 1.5 rounds | **Range:** 2 hexes

**Effect:**  
Encases target enemy unit in ice, rooting them in place and dealing damage over time. Rooted units cannot move but may still use abilities.

**Level Progression:**
- **Level 1-5:** 20 total damage, 10 turns, 2 damage per turn.
- **Level 6-11:** 40 total damage, 20 turns, 2 damage per turn.
- **Level 12+:** 60 total damage, 20 turns, 3 damage per turn.

---

#### Arcane Aura
**Type:** Passive (Aura) | **Unlock:** Level 1

**Effect:**  
Crystal Maiden and all allied heroes within range passively regenerate Mana. This regeneration occurs during the Round End Phase (after all 20 turns are complete).

**Level Progression:**
- **Level 1-5:** 10 Mana per round, global
- **Level 6-11:** 20 Mana per round, global
- **Level 12+:** 30 Mana per round, global

---

#### Freezing Field
**Type:** Channeled | **Targeting:** No Target (Self-Cast) | **Unlock:** Level 6

**Mana Cost:** 40 | **AP Cost:** 1 | **Cooldown:** 5 rounds | **Duration:** Channeled (TBD rounds max)

**Effect:**  
Crystal Maiden channels a massive ice storm around her, dealing damage in pulses to all enemy units within range and slowing them. Must remain stationary while channeling. Interrupted by Stun, Silence, forced movement, or voluntary cancellation.

**Level Progression:**
- **Level 6-11:** 20 damage per pulse, 1 pulse every 2nd turn, 2 hex radius, -2 AP while in range
- **Level 12-17:** 30 damage per pulse, 1 pulse every 2nd turn, 2 hex radius, -3 AP while in range
- **Level 18+:** 40 damage per pulse, 1 pulse every 2nd turn, 2 hex radius, -5 AP while in range

---

### Design Notes

**Role:** Crystal Maiden is an Intelligence ranged support with exceptional team utility through mana regeneration. She provides strong early-game harassment and crowd control, with a high-impact channeled ultimate that demands careful positioning and team protection.

**Playstyle Considerations:**
- Low HP and Defense make Crystal Maiden vulnerable to ganks and burst damage
- Arcane Aura enables team spell usage — Crystal Maiden's presence increases team-wide ability frequency
- Crystal Nova and Frostbite provide strong zoning and pick-off potential in lane
- Freezing Field requires positioning behind allies and ideally BKB or other defensive items
- Slow Move Speed makes escape difficult — positioning and map awareness critical

**Balance Considerations:**
- Crystal Nova cooldown and mana cost should allow frequent harassment without being oppressive
- Frostbite root duration must balance disable power against its single-target nature
- Arcane Aura mana regeneration must be meaningful but not eliminate mana as a resource constraint
- Freezing Field damage must reward full channel duration but not be overwhelming if interrupted early
- All abilities should synergize (Nova slows enemies into Field range, Frostbite holds key targets)

**Thematic Identity:**
Crystal Maiden is the quintessential Intelligence support: fragile, mana-efficient, team-oriented, and high-impact when protected. Her design rewards smart positioning, resource management, and coordination with allies who can leverage her mana aura and protect her during ultimate channeling.

---

## Lion
**Class:** Intelligence | **Attack Type:** Ranged | **Status:** 🔲 Design in Progress

### Base Stats

| Stat | Value |
|------|-------|
| **Health (HP)** | 70 |
| **Mana** | 45 |
| **Attack** | 7 |
| **Attack Range** | 3 hexes |
| **Defense** | 1 |
| **Move Speed** | 1 |
| **Action Points (AP)** | 10 |

### Stat Scaling
- **Per Level:** +10 HP, +12 Mana, +3 Attack, +1 Defense

### Abilities

---

#### Earth Spike
**Type:** Active | **Targeting:** Direction/Vector | **Special:** Skillshot | **Unlock:** Level 1

**Mana Cost:** 12 | **AP Cost:** 1 | **Cooldown:** 2 rounds | **Range:** 4 hexes max

**Effect:**  
Sends a column of spikes erupting along a line in the chosen direction. The spikes travel up to 4 hexes, stunning and damaging all enemy units in a 1-hex-wide path. Enemies may use the Dodge Skillshot reaction to attempt to avoid the spikes.

**Level Progression:**
- **Level 1-5:** 15 damage, 8 AP stun
- **Level 6-11:** 25 damage, 12 AP stun
- **Level 12+:** 35 damage, 16 AP stun

**Notes:**  
Unlike Sacred Arrow, Earth Spike hits all units along its path (not just the first), making it excellent for controlling grouped enemies.

**Aghanim's Scepter Upgrade:**  
Earth Spike now erupts in a T-shape pattern: the original line plus perpendicular spikes extending 2 hexes to each side at the endpoint. All affected units are stunned and damaged.

---

#### Hex
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 1

**Mana Cost:** 18 | **AP Cost:** 1 | **Cooldown:** 2 rounds | **Range:** 3 hexes

**Effect:**  
Transforms target enemy hero into a harmless critter, disabling them completely for the duration. Hexed heroes cannot move, attack, use abilities, or use items. The target's Defense is reduced to 0 while Hexed.

**Level Progression:**
- **Level 1-5:** 10 turns duration
- **Level 6-11:** 15 turns duration
- **Level 12+:** 20 turns (1 round) duration

**Notes:**  
Hex is one of the strongest disables in the game — the target is completely helpless and vulnerable. Unlike stuns (which only reduce AP), Hex prevents all actions and removes defensive stats.

---

#### Mana Drain
**Type:** Channeled | **Targeting:** Unit Target | **Unlock:** Level 1

**Mana Cost:** 0 | **AP Cost:** 1 to activate | **Cooldown:** 1 round

**Effect:**  
Lion channels on target enemy hero within range, draining their Mana and transferring it to himself. The drain continues at the start of each hero's activation while the channel is active. Lion must maintain Line of Sight to the target. Interrupted by Stun, Silence, forced movement (Lion or target), target moving out of range/LoS, or if Lion voluntarily cancels.

**Level Progression:**
- **Level 1-5:** Drain 3 Mana per activation (max 1 round channel)
- **Level 6-11:** Drain 4 Mana per activation (max 1.5 rounds channel)
- **Level 12+:** Drain 5 Mana per activation (max 2 rounds channel)

**Notes:**  
"Per activation" means Mana is drained at the start of every hero's turn while the channel is active (up to 20 drains per round in a 10-hero game). Over a full channel, this can completely drain an enemy's Mana pool while fully restoring Lion's. Lion cannot move or take other actions while channeling.

**Aghanim's Scepter Upgrade:**  
Mana Drain becomes an AoE channel affecting all enemy heroes within 3 hexes of Lion. Each affected hero is drained separately, and Lion receives Mana from all of them.

---

#### Finger of Death
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 6

**Mana Cost:** 40 | **AP Cost:** 2 | **Cooldown:** 3 rounds | **Range:** 4 hexes

**Effect:**  
Lion channels dark magic to instantly deal massive damage to a single target enemy hero. This is Lion's signature burst damage ability, capable of eliminating low-HP heroes or finishing fleeing enemies.

**Level Progression:**
- **Level 6-11:** 60 damage
- **Level 12-17:** 90 damage
- **Level 18+:** 120 damage

**Notes:**  
Finger of Death deals pure instant damage — no damage over time, just a single massive hit. This makes it excellent for securing kills on heroes trying to escape or finishing off heroes who survive Lion's disable combo.

**Aghanim's Scepter Upgrade:**  
Finger of Death cooldown reduced to 2 rounds. Damage increased by 30 at all levels. If Finger of Death kills the target, Lion gains a permanent stack granting +3 Mana and +2 Attack (stacks indefinitely).

---

### Design Notes

**Role:** Lion is an Intelligence ranged support specializing in disables and burst damage. He excels at controlling enemy heroes through stuns and transformation, draining their resources, and eliminating priority targets with massive single-target damage.

**Playstyle Considerations:**
- Extremely fragile (lowest HP in current roster) — positioning and safety are critical
- Strong disable chaining: Earth Spike into Hex can lock down a hero for extended periods
- Mana Drain provides sustain and resource denial — can keep Lion's mana high while starving enemies
- Finger of Death is a true "delete button" for low-HP heroes but has long cooldown
- High mana costs mean Lion needs careful resource management despite having good base mana
- Ranged attack keeps him safer than melee supports

**Balance Considerations:**
- Hex duration must be powerful enough to justify its high mana cost but not so long it feels unfair
- Earth Spike's multi-target stun is stronger than single-target stuns — damage and stun duration calibrated accordingly
- Mana Drain channel duration must balance resource gain against vulnerability while channeling
- Finger of Death damage must be high enough to threaten kills but not guarantee kills on full-HP targets
- Low HP makes Lion extremely vulnerable to ganks and burst damage — counterplay exists through focusing him

**Thematic Identity:**
Lion embodies the hard-disable Intelligence support archetype: fragile but with devastating control and burst potential. His design rewards precise ability usage (landing Earth Spike on multiple targets, choosing correct Hex timing), resource management (using Mana Drain to sustain spell casting), and target prioritization (saving Finger for high-value kills). He's the quintessential "glass cannon" support — immense impact when protected, easy kill when caught out of position.

---

## Rubick
**Class:** Intelligence | **Attack Type:** Ranged | **Status:** 🔲 Design in Progress

### Base Stats

| Stat | Value |
|------|-------|
| **Health (HP)** | 72 |
| **Mana** | 55 |
| **Attack** | 6 |
| **Attack Range** | 3 hexes |
| **Defense** | 1 |
| **Move Speed** | 1 |
| **Action Points (AP)** | 10 |

### Stat Scaling
- **Per Level:** +10 HP, +12 Mana, +3 Attack, +1 Defense

### Abilities

---

#### Telekinesis
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 1

**Mana Cost:** 18 | **AP Cost:** 2 | **Cooldown:** 2 rounds | **Range:** 3 hexes

**Effect:**  
Rubick lifts target enemy hero into the air, removing them from their hex until they land. While lifted, the target cannot move, attack, use abilities, use items, or react. Rubick then places that hero on any Open hex within 2 hexes of the original target hex. When the target lands, all enemy units within 1 hex of the landing hex are stunned.

**Level Progression:**
- **Level 1-5:** Landing stun 3 AP loss
- **Level 6-11:** Landing stun 4 AP loss
- **Level 12+:** Landing stun 5 AP loss

**Notes:**  
The lifted hero is not targetable while airborne. Rubick may throw the target onto high-value terrain positions, out of cover, or into allied follow-up range, but the target must land on a legal Open hex.

---

#### Fade Bolt
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 1

**Mana Cost:** 14 | **AP Cost:** 1 | **Cooldown:** 2 rounds | **Range:** 4 hexes

**Effect:**  
Rubick fires a bolt of unstable magic at target enemy unit. The bolt deals damage, then jumps to up to 2 additional enemy units within 2 hexes of the last target. A unit can only be hit once per cast. Heroes hit by Fade Bolt deal reduced Attack damage until the end of their next activation.

**Level Progression:**
- **Level 1-5:** 16 damage per hit, -2 Attack
- **Level 6-11:** 24 damage per hit, -3 Attack
- **Level 12+:** 32 damage per hit, -4 Attack

**Notes:**  
Fade Bolt may jump between heroes, creeps, and neutral units, but the Attack reduction only affects heroes.

---

#### Arcane Supremacy
**Type:** Passive | **Unlock:** Level 1

**Effect:**  
Rubick amplifies stolen and cast magic with unnerving precision. Whenever Rubick deals damage with an ability, increase that damage. When Rubick applies a stun, silence, root, slow, or other non-passive debuff with an ability, extend its duration.

**Level Progression:**
- **Level 1-5:** +4 ability damage, +2 turns to applied debuffs
- **Level 6-11:** +8 ability damage, +3 turns to applied debuffs
- **Level 12+:** +12 ability damage, +4 turns to applied debuffs

**Notes:**  
Arcane Supremacy affects Rubick's native abilities and any ability currently copied by Spell Steal. It does not increase damage from basic attacks or items unless an item explicitly counts as an ability effect.

---

#### Spell Steal
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 6

**Mana Cost:** 20 | **AP Cost:** 2 | **Cooldown:** 2 rounds | **Range:** 4 hexes

**Effect:**  
Rubick targets an enemy hero and copies the last non-passive hero ability that hero successfully used. Rubick may commit and use that stolen ability as if it were printed on his own card until Spell Steal expires, he steals a different spell, or he dies.

**Level Progression:**
- **Level 6-11:** Stolen spell lasts 1 round
- **Level 12-17:** Stolen spell lasts 2 rounds
- **Level 18+:** Stolen spell lasts 3 rounds

**Rules for Stolen Spells:**
- Rubick may only hold **one** stolen spell at a time.
- Rubick comes with **3 Spell Steal tracking tokens**: **1 cooldown token** for his own hero board and **2 stolen-spell marker tokens** for marking copied abilities.
- Rubick also has **2 hero-specific planning tokens**: **Stolen Spell 1** and **Stolen Spell 2**.
- When Rubick casts Spell Steal, place the **cooldown token** in the appropriate **Ability Cooldowns** row on Rubick's **Hero Board**.
- Place **1 stolen-spell marker token** on the copied ability on the target hero's Abilities Card to show exactly which spell Rubick currently holds.
- During the **Planning Phase**, Rubick places **Stolen Spell 1** or **Stolen Spell 2** face-down in his **Action Queue** to commit the stolen spell linked to that marker.
- After Rubick resolves a stolen spell, place the matching **Stolen Spell 1** or **Stolen Spell 2** token in the appropriate **Ability Cooldowns** row on Rubick's **Hero Board** for that copied spell's normal cooldown. Use the **Turns** or **Rounds** section that the copied spell normally uses. When that cooldown expires, return the token to Rubick's available planning token pool.
- If Rubick has **Aghanim's Scepter**, he may hold **two** stolen spells at once. Place **1 stolen-spell marker token** on each copied ability.
- **Stolen Spell 1** corresponds to Rubick's first stolen-spell marker. **Stolen Spell 2** corresponds to his second stolen-spell marker and is only usable while Rubick has Aghanim's Scepter and a second copied spell.
- If Rubick steals a new spell while already at his stolen-spell limit, remove the existing stolen-spell marker in a first-in-first-out order.
- If Rubick dies, remove all Spell Steal marker tokens immediately. Any stolen-spell planning tokens on his Hero Board return to his available token pool when he respawns.
- Rubick uses the stolen spell's normal AP cost, mana cost, range, and targeting rules.
- Rubick uses the stolen spell at the stolen spell's **current level scaling** based on the target hero's level bracket when it was stolen.
- If the stolen spell depends on a token, marker, or state unique to the original hero, Rubick copies only the cast effect, not that hero's entire subsystem.
- Passive abilities, item abilities, and ultimates modified by Aghanim's Scepter cannot be stolen unless the printed ability itself is the one being copied.
- Arcane Supremacy applies to the stolen spell.

**Aghanim's Scepter Upgrade:**  
Spell Steal cooldown reduced to 1/2 round. Rubick may hold **two** stolen spells at once.

---

### Design Notes

**Role:** Rubick is an Intelligence ranged support-disabler built around repositioning, spell disruption, and stealing the enemy's strongest play pattern. He excels at punishing predictable initiations and converting enemy power spikes into his own.

**Playstyle Considerations:**
- Telekinesis is his primary setup and save-denial tool — it creates positional chaos more than raw damage
- Fade Bolt gives Rubick reliable poke and soft teamfight mitigation without turning him into a pure nuker
- Arcane Supremacy makes Rubick's spells and stolen spells feel sharper than the originals without changing their core identity
- Spell Steal rewards matchup knowledge and timing — Rubick is strongest when he steals the right spell from the right hero at the right moment
- Low durability means Rubick must play from range and from vision rather than frontline positions

**Balance Considerations:**
- Telekinesis should be strong because of repositioning, not because it fully removes a hero for too long
- Fade Bolt must stay efficient utility damage rather than becoming a board-wiping chain nuke
- Arcane Supremacy should enhance clarity and payoff without forcing constant cross-referencing during play
- Spell Steal needs hard limits on duration, slot count, and eligible spell types so Rubick remains exciting but administratively manageable
- Rubick should scale with enemy roster complexity, which makes him naturally high-skill without needing inflated base stats

**Thematic Identity:**
Rubick embodies the theatrical spell-thief fantasy: clever positioning, magical disruption, and turning enemy signature tools back against them. His design should make the opposing team feel unsafe using their best abilities carelessly, while rewarding the Rubick player for timing, rules fluency, and tactical opportunism.

---