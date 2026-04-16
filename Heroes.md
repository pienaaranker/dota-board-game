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
| **Defense** | 3 |
| **Move Speed** | 1 |
| **Action Points (AP)** | 10 |

### Stat Scaling
- **Per Level:** +10 HP, +10 Mana, +5 Attack, +1 Defense

### Abilities

---

#### Storm Hammer
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 1

**Mana Cost:** 3 | **AP Cost:** 1 | **Cooldown:** 2 rounds | **Range:** 2 hexes

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
