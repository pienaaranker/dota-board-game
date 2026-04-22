# DOTA 2: THE BOARD GAME — AGILITY HERO CARDS

This document contains the current full card designs for Agility heroes.

For draft rules and class-wide roster status, see [../hero-shortlist.md](../hero-shortlist.md). For the full hero card index, see [../roster.md](../roster.md).

---

## Mirana
**Class:** Agility | **Attack Type:** Ranged 

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
Grants Invisibility to Mirana and all allied heroes on the board, regardless of their position. Each hero receives their own Invisibility Cloud as per standard Invisibility rules in [../../../rulebook/mechanics/Mechanics.md](../../../rulebook/mechanics/Mechanics.md). The invisibility lasts for the specified duration or until each hero attacks or uses a revealing ability.

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