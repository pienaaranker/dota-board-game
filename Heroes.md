# DOTA 2: THE BOARD GAME — HERO CARDS

This document contains the full card designs for heroes in the board game. Each entry includes base stats, abilities, and all information needed to play that hero.

For hero selection and draft rules, see `Mechanics.md §2`. For ability mechanics and targeting types, see `Mechanics.md §17`.

---

## Sven
**Class:** Strength | **Attack Type:** Melee 

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

## Pudge
**Class:** Strength | **Attack Type:** Melee | **Status:** 🔲 Design in Progress

### Base Stats

| Stat | Value |
|------|-------|
| **Health (HP)** | 115 |
| **Mana** | 25 |
| **Attack** | 7 |
| **Attack Range** | 1 hex |
| **Defense** | 3 |
| **Move Speed** | 1 |
| **Action Points (AP)** | 10 |

### Stat Scaling
- **Per Level:** +12 HP, +8 Mana, +4 Attack, +1 Defense

### Abilities

---

#### Meat Hook
**Type:** Active | **Targeting:** Direction/Vector | **Special:** Skillshot | **Unlock:** Level 1

**Mana Cost:** 14 | **AP Cost:** 2 | **Cooldown:** 2.5 rounds | **Range:** 5 hexes max

**Effect:**  
Launches a bloody hook in a straight line in the chosen direction. The hook travels up to 5 hexes or until it hits an enemy hero or creep. The first unit struck takes damage and is pulled back to the hex adjacent to Pudge. Enemies may use the Dodge Skillshot reaction to attempt to avoid the hook.

**Level Progression:**
- **Level 1-5:** 15 damage
- **Level 6-11:** 25 damage
- **Level 12+:** 40 damage

**Notes:**  
The hooked unit is forcibly moved to a hex adjacent to Pudge along the line of the hook (if the direct hex is not available the player being hooked chooses which adjacent hex). If the target is a hero, this forced movement can be used to isolate enemies or pull them into dangerous positions.

---

#### Rot
**Type:** Toggle | **Targeting:** No Target (Self-Cast) | **Unlock:** Level 1

**Mana Cost:** 0 | **AP Cost:** 1 to activate | **Cooldown:** None

**Effect:**  
Pudge releases toxic gases around himself, dealing damage per turn to all enemy units within 1 hex and to Pudge himself. Can be toggled on during Pudge's turn and toggled off at any time (even during other heroes' turns) unless Pudge is Silenced. While active, Rot damages all affected units (including Pudge) at the start of each hero's activation if they are within range.

**Level Progression:**
- **Level 1-5:** 2 damage per activation
- **Level 6-11:** 3 damage per activation
- **Level 12+:** 5 damage per activation

**Notes:**  
"Per activation" means the damage ticks at the start of every hero's turn (20 times per round total in a 10-hero game). This creates significant damage output over time but also drains Pudge's Health rapidly. Pudge takes the same damage as enemies.

---

#### Flesh Heap
**Type:** Passive | **Unlock:** Level 1

**Effect:**  
Pudge gains permanent bonus HP whenever an enemy hero dies within 3 hexes of him. These bonuses stack indefinitely throughout the game and apply retroactively to his current Health total (if Pudge is at full HP when he gains a stack, his maximum and current HP both increase).

**Level Progression:**
- **Level 1-5:** +8 HP per enemy hero death
- **Level 6-11:** +12 HP per enemy hero death
- **Level 12+:** +16 HP per enemy hero death

**Notes:**  
Flesh Heap rewards aggressive positioning and kill participation. Stacks are permanent and persist through death — Pudge respawns with all accumulated Flesh Heap bonus HP intact.

---

#### Dismember
**Type:** Channeled | **Targeting:** Unit Target | **Unlock:** Level 6

**Mana Cost:** 30 | **AP Cost:** 2 | **Cooldown:** 4 rounds | **Duration:** Channeled (max 2 rounds)

**Effect:**  
Pudge channels his ultimate on target enemy hero within 1 hex, dealing damage per turn and disabling the target completely. The target cannot move, attack, or use abilities while Dismembered. Pudge must remain adjacent to the target while channeling. Interrupted by Stun, Silence, forced movement (Pudge or target), or if Pudge voluntarily cancels.

**Level Progression:**
- **Level 6-11:** 4 damage per activation (80 damage over full 2-round channel in 10-hero game)
- **Level 12-17:** 6 damage per activation (120 damage over full 2-round channel)
- **Level 18+:** 8 damage per activation (160 damage over full 2-round channel)

**Notes:**  
"Per activation" means damage is dealt at the start of each hero's turn while the channel is active (20 times per round in a 10-hero game). Pudge and the target are both effectively disabled for the duration — Pudge cannot take other actions or move (except to follow if target is forcibly moved), and the target is completely locked down.

**Aghanim's Scepter Upgrade:**  
Dismember can be cast on targets up to 2 hexes away (no longer requires adjacency). Pudge heals for 50% of damage dealt. Duration increased to 3 rounds maximum.

---

### Design Notes

**Role:** Pudge is a Strength melee initiator and ganker who excels at isolating and eliminating priority targets. Meat Hook provides unparalleled pick-off potential, Rot deals sustained AoE damage at the cost of self-harm, Flesh Heap makes him progressively tankier, and Dismember locks down single targets for extended periods.

**Playstyle Considerations:**
- Extremely high HP pool (highest base HP + Flesh Heap scaling) makes Pudge one of the tankiest heroes
- Meat Hook is game-defining — landing hooks on key targets can win fights instantly
- Rot's self-damage creates interesting risk/reward decisions (high damage output vs. killing yourself)
- Flesh Heap rewards aggressive roaming and kill participation — Pudge gets stronger as the game progresses
- Dismember requires Pudge to commit fully to a target (can't act while channeling) but guarantees a long disable
- Low mana pool means Pudge must carefully manage spell usage early game

**Balance Considerations:**
- Meat Hook range and damage must be balanced against its Skillshot nature and high skill requirement
- Rot self-damage must be significant enough to prevent mindless toggle-on gameplay
- Flesh Heap stacks should be meaningful but not allow infinite HP scaling to break the game
- Dismember's long disable duration is balanced by Pudge being unable to take other actions and vulnerability to interruption
- Low starting mana and moderate mana scaling ensure Pudge can't spam spells without itemization

**Thematic Identity:**
Pudge embodies the tanky Strength ganker archetype: high HP, high-risk/high-reward abilities (Hook + Rot self-damage), and brutal single-target lockdown (Dismember). His design rewards mechanical skill (landing Hooks), positioning (Rot radius, Flesh Heap proximity, Dismember adjacency), and calculated aggression (managing Rot self-damage, committing to Dismember channels).

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
