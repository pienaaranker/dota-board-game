# DOTA 2: THE BOARD GAME — HERO CARDS

This document contains the full card designs for heroes in the board game. Each entry includes base stats, abilities, and all information needed to play that hero.

For hero selection and draft rules, see `Mechanics.md §2`. For ability mechanics and targeting types, see `Mechanics.md §17`.

---

## Sven
**Class:** Strength | **Attack Type:** Melee | **Status:** 🔲 Design in Progress

### Base Stats

| Stat | Value |
|------|-------|
| **Health (HP)** | 100 |
| **Mana** | 30 |
| **Attack** | 10 |
| **Attack Range** | 1 hex |
| **Defense** | 3 |
| **Move Speed** | 1 |
| **Action Points (AP)** | 10 |

### Stat Scaling
- **Per Level:** +10 HP, +10 Mana, +5 Attack, +1 Defense

### Abilities

---

#### Storm Hammer
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 1

**Mana Cost:** 10 | **AP Cost:** 1 | **Cooldown:** 2 rounds | **Range:** 2 hexes

**Effect:**  
Hurl a magical hammer at target unit, dealing damage and stunning all enemy units within 1 hex of the target. Can be disjointed by Blink and similar displacement effects using a reaction.

**Level Progression:**
- **Level 1-5:** 20 damage, stun (10 AP loss)
- **Level 6-11:** 30 damage, stun (15 AP loss)
- **Level 12+:** 40 damage, stun (20 AP loss)

**Aghanim's Scepter Upgrade:**  
Sven may choose to travel with the hammer, arriving at the impact location. Impact damage increased to 60.

---

#### Great Cleave
**Type:** Passive | **Unlock:** Level 1

**Effect:**  
Sven's attacks cleave in a 2-hex cone in front of him, dealing damage to all units in the area. When Sven uses Farm on a creep wave, he only needs to farm twice to clear the entire wave and receives the gold and XP for all creeps.

**Level Progression:**
- **Level 1-5:** 2 cleave damage
- **Level 6-11:** 4 cleave damage  
- **Level 12+:** 6 cleave damage

---

#### Warcry
**Type:** Active | **Targeting:** No Target (Self-Cast) | **Unlock:** Level 1

**Mana Cost:** 1 | **AP Cost:** 1 | **Cooldown:** 3 rounds | **Duration:** 1 round

**Effect:**  
Sven and all allied heroes within 3 hexes gain bonus Defense and Move Speed for the duration. Does not affect creeps.

**Level Progression:**
- **Level 1-5:** +5 Defense, +1 Move Speed
- **Level 6-11:** +10 Defense, +1 Move Speed
- **Level 12+:** +10 Defense, +2 Move Speed

---

#### God's Strength
**Type:** Active | **Targeting:** No Target (Self-Cast) | **Unlock:** Level 6

**Mana Cost:** 2 | **AP Cost:** 2 | **Cooldown:** 4 rounds | **Duration:** 1 round

**Effect:**  
Sven channels his rogue knight's fury, gaining bonus Attack for the duration. Great Cleave damage is also increased by the same amount.

**Level Progression:**
- **Level 6-11:** +10 Attack
- **Level 12-17:** +20 Attack
- **Level 18+:** +40 Attack

---

### Design Notes

**Role:** Sven is a Strength melee carry with strong teamfight presence through cleave damage and an ultimate that turns him into a late-game damage dealer. Storm Hammer provides initiation and crowd control. Warcry offers utility through armor and movement buffs for the team.

**Playstyle Considerations:**
- High HP and Defense make Sven durable in extended fights
- Cleave requires positioning to maximize damage across multiple targets
- God's Strength timing windows are critical — must be used when Sven can freely attack
- Warcry can enable allied hero engagements or escapes

**Balance Considerations:**
- Cleave damage should be significant enough to encourage farming multiple creeps/fighting in waves, but not so high it trivializes AoE damage dealers
- Storm Hammer stun duration must be calibrated against other stuns in the game (typical range: 1-3 AP loss)
- God's Strength duration should be long enough to get value but short enough to create tension (typical range: 2-4 rounds)
- All mana costs should ensure Sven has limited early-game spell usage without mana items

**Thematic Identity:**
Sven embodies the classic Strength hero archetype: tanky, hits hard, scales into late game, provides utility through buffs and stuns. His design should reward good positioning (cleave), timing (God's Strength windows), and team coordination (Warcry).

---

## Crystal Maiden
**Class:** Intelligence | **Attack Type:** Ranged | **Status:** 🔲 Design in Progress

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

## Mirana
**Class:** Agility | **Attack Type:** Ranged | **Status:** 🔲 Design in Progress

### Base Stats

| Stat | Value |
|------|-------|
| **Health (HP)** | 85 |
| **Mana** | 40 |
| **Attack** | 8 |
| **Attack Range** | 3 hexes |
| **Defense** | 2 |
| **Move Speed** | 1 |
| **Action Points (AP)** | 10 |

### Stat Scaling
- **Per Level:** +10 HP, +10 Mana, +4 Attack, +1 Defense

### Abilities

---

#### Starfall
**Type:** Active | **Targeting:** Unit-Targeted AoE | **Unlock:** Level 1

**Mana Cost:** 12 | **AP Cost:** 1 | **Cooldown:** 2 rounds | **Range:** 3 hexes

**Effect:**  
Summons a wave of meteors around target enemy unit, dealing damage to all enemy units within 2 hexes of the target. If Mirana is within 2 hexes of the primary target, that unit takes a second instance of Starfall damage (double damage total).

**Level Progression:**
- **Level 1-5:** 15 damage per instance
- **Level 6-11:** 25 damage per instance
- **Level 12+:** 35 damage per instance

---

#### Sacred Arrow
**Type:** Active | **Targeting:** Direction/Vector | **Special:** Skillshot | **Unlock:** Level 1

**Mana Cost:** 15 | **AP Cost:** 2 | **Cooldown:** 2.5 rounds | **Range:** 5 hexes max

**Effect:**  
Fires an arrow in a straight line in the chosen direction. The arrow travels up to 5 hexes or until it hits an enemy hero. The first enemy hero struck takes damage and is stunned. Stun duration increases based on how far the arrow traveled before impact. Enemies may use the Dodge Skillshot reaction to attempt to avoid the arrow.

**Level Progression:**
- **Level 1-5:** 20 damage, +3 AP stun per hex traveled (3 AP at 1 hex, 6 AP at 2 hexes, 9 AP at 3 hexes, 12 AP at 4 hexes, 15 AP at max range)
- **Level 6-11:** 30 damage, +4 AP stun per hex traveled (4 AP at 1 hex, 8 AP at 2 hexes, 12 AP at 3 hexes, 16 AP at 4 hexes, 20 AP at max range)
- **Level 12+:** 40 damage, +5 AP stun per hex traveled (5 AP at 1 hex, 10 AP at 2 hexes, 15 AP at 3 hexes, 20 AP at 4 hexes, 25 AP at max range)

**Aghanim's Scepter Upgrade:**  
The current level of starfall is applied to all enemy units along the path and 1 hex adjacent.

---

#### Leap
**Type:** Active | **Targeting:** Direction/Vector | **Unlock:** Level 1

**Mana Cost:** 8 | **AP Cost:** 1 | **Cooldown:** 1.5 rounds

**Effect:**  
Mirana leaps forward up to 3 hexes in a straight line to an unoccupied hex, passing over obstacles, walls and terrain. After landing, Mirana gains bonus Attack Speed for a short duration.

**Level Progression:**
- **Level 1-5:** +2 Attack for 10 turns
- **Level 6-11:** +3 Attack for 1 round (20 turns)
- **Level 12+:** +4 Attack for 1 round (20 turns)

**Notes:**  
Leap can pass over Tree hexes and Buildings but cannot pass through Impassable terrain. The destination hex must be unoccupied. If it is not Mirana falls on the nearest open hex on the path.

---

#### Moonlight Shadow
**Type:** Active | **Targeting:** No Target (Global) | **Unlock:** Level 6

**Mana Cost:** 20 | **AP Cost:** 2 | **Cooldown:** 6 rounds | **Duration:** 20 turns (1 round)

**Effect:**  
Grants Invisibility to Mirana and all allied heroes on the board, regardless of their position. Each hero receives their own Invisibility Cloud as per standard Invisibility rules (see Mechanics.md §14). The invisibility lasts for the specified duration or until each hero attacks or uses a revealing ability.

**Level Progression:**
- **Level 6-11:** 20 turns (1 round) duration
- **Level 12-17:** 30 turns (1.5 rounds) duration
- **Level 18+:** 40 turns (2 rounds) duration

---

### Design Notes

**Role:** Mirana is an Agility ranged hero who excels as a versatile core or roaming support. She provides long-range initiation through Sacred Arrow, burst damage with Starfall, exceptional mobility via Leap, and team-wide utility through Moonlight Shadow.

**Playstyle Considerations:**
- Sacred Arrow is her signature ability — landing long-range arrows is game-changing but requires prediction and timing
- Starfall's double-proc mechanic rewards aggressive positioning (being close to targets)
- Leap provides both initiation and escape, can be used to traverse terrain for ganks or jukes
- Moonlight Shadow enables team-wide invisibility for coordinated ganks, escapes, or Roshan attempts
- Moderate HP and Defense make her less fragile than Crystal Maiden but not as tanky as Sven
- Ranged attack type keeps her safer in teamfights than melee heroes

**Balance Considerations:**
- Sacred Arrow stun scaling must reward long-range hits without being oppressive at close range
- Starfall's double damage proc should encourage risk-taking (moving close to targets) but not be guaranteed
- Leap cooldown and mobility distance must balance her escape/initiation power with counterplay windows
- Moonlight Shadow's global team invisibility is extremely powerful — long cooldown and high mana cost are necessary
- All mana costs should ensure Mirana needs mana items for sustained ability usage

**Thematic Identity:**
Mirana embodies the high-skill-cap Agility hero: mobile, versatile, rewarding of precision (Arrow), and enabling for her team (Moonlight Shadow). Her design should reward mechanical skill (landing Arrows, positioning for Starfall procs), map awareness (roaming with Leap), and team coordination (using Moonlight Shadow for synchronized plays).

---
