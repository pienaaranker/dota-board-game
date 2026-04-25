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
Fires an arrow in a straight line in the chosen direction. The arrow travels up to 5 hexes or until it hits an enemy hero. The first enemy hero struck takes damage and is stunned. Stun duration increases based on how far the arrow traveled before impact. Enemies may attempt to dodge the arrow by using a committed 1 AP movement action or 1 AP movement ability as a reaction.

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

## Juggernaut
**Class:** Agility | **Attack Type:** Melee

### Base Stats

| Stat | Value |
|------|-------|
| **Health (HP)** | 95 |
| **Mana** | 30 |
| **Attack** | 9 |
| **Attack Range** | 1 hex |
| **Defense** | 2 |
| **Move Speed** | 1 |
| **Action Points (AP)** | 10 |

### Stat Scaling
- **Per Level:** +10 HP, +8 Mana, +4 Attack, +1 Defense

### Abilities

---

#### Blade Fury
**Type:** Active | **Targeting:** No Target (Self-Cast) | **Unlock:** Level 1

**Mana Cost:** 15 | **AP Cost:** 2 | **Cooldown:** 3 rounds | **Duration:** Current activation

**Effect:**  
Juggernaut enters a spinning bladestorm for the rest of his current activation. While Blade Fury is active, Juggernaut gains **Spell Immunity**, cannot use **Attack** actions, and cannot use other abilities or items. When Blade Fury is activated, and each time Juggernaut moves into a new hex during that activation, deal damage to all enemy units within 1 hex.

**Level Progression:**
- **Level 1-5:** 12 damage per hit
- **Level 6-11:** 18 damage per hit
- **Level 12+:** 24 damage per hit

**Notes:**  
Blade Fury is intended to convert Juggernaut's Move actions into area pressure. If Juggernaut does not move after activating Blade Fury, only the initial damage instance is applied.

---

#### Healing Ward
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 1

**Mana Cost:** 12 | **AP Cost:** 1 | **Cooldown:** 4 rounds | **Range:** 1 hex

**Effect:**  
Place a **Healing Ward token** on an adjacent Open hex. At the start of each allied hero's activation, that hero restores HP if they are within 2 hexes of the Healing Ward. At the start of each of Juggernaut's activations, he may move the Healing Ward up to 2 hexes. Only one Healing Ward may be on the board for Juggernaut at a time.

**Level Progression:**
- **Level 1-5:** Heal 8 HP per activation, lasts 1 round
- **Level 6-11:** Heal 12 HP per activation, lasts 2 rounds
- **Level 12+:** Heal 16 HP per activation, lasts 2 rounds

**Notes:**  
The Healing Ward is a fragile summon. Any enemy hero adjacent to the ward may spend 1 **Attack** action to destroy it immediately.

---

#### Blade Dance
**Type:** Passive | **Unlock:** Level 1

**Effect:**  
Juggernaut's swordsmanship makes his strikes exceptionally lethal. The first **Attack** action Juggernaut resolves during each activation deals bonus damage.

**Level Progression:**
- **Level 1-5:** +4 bonus damage
- **Level 6-11:** +6 bonus damage
- **Level 12+:** +9 bonus damage

**Notes:**  
Blade Dance also applies to the first slash of **Omnislash** each time Juggernaut uses that ability.

---

#### Omnislash
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 6

**Mana Cost:** 30 | **AP Cost:** 2 | **Cooldown:** 4 rounds | **Range:** 2 hexes

**Effect:**  
Juggernaut targets an enemy hero within range and immediately begins Omnislash. Resolve the listed number of slashes one at a time.

For the **first slash**, Juggernaut hits the chosen target. For each **later slash**, the Juggernaut player chooses an enemy hero within 1 hex of the hero hit by the previous slash. If there is no other enemy hero within 1 hex, Juggernaut may hit that same hero again instead.

Each slash deals damage equal to Juggernaut's current **Attack**. While Omnislash is resolving, Juggernaut cannot be targeted by enemy attacks or abilities. After the final slash, place Juggernaut on any Open hex adjacent to the hero hit by the last slash.

**Level Progression:**
- **Level 6-11:** 3 slashes
- **Level 12-17:** 4 slashes
- **Level 18+:** 5 slashes

**Aghanim's Scepter Upgrade:**  
Omnislash gains +1 slash at all levels and its cooldown is reduced to 3 rounds.

---

### Design Notes

**Role:** Juggernaut is an Agility melee carry who combines reliable self-sufficiency with explosive kill windows. He brings lane pressure through Blade Fury, sustain through Healing Ward, and late-game dueling power through Blade Dance and Omnislash.

**Playstyle Considerations:**
- Blade Fury lets Juggernaut fight early without relying entirely on basic attacks
- Healing Ward gives him and nearby allies staying power during sieges, Roshan attempts, and drawn-out skirmishes
- Blade Dance rewards careful sequencing so Juggernaut opens each activation with his strongest strike
- Omnislash is his signature execution tool and is strongest when enemies are isolated or clustered tightly enough for repeated slashes
- Moderate durability and low mana pool mean he can frontline briefly, but still needs timing and positioning to avoid being collapsed on after his burst window ends

**Balance Considerations:**
- Blade Fury must feel threatening during the early game without becoming a guaranteed kill button against slower heroes
- Healing Ward should create meaningful sustain value, but its fragility must give opponents a clear answer
- Blade Dance should make Juggernaut's attacks feel elite without introducing too much random swinginess
- Omnislash should be devastating against isolated targets while still offering counterplay through positioning and nearby allied bodies
- Mana costs should force Juggernaut to choose between sustain and aggression in the early game

**Thematic Identity:**
Juggernaut embodies the disciplined masked swordsman: relentless forward pressure, elegant sustain, and terrifying burst once he commits. His design should feel simple to understand, difficult to stop at the right moment, and unmistakably centered on bladework mastery.

---

## Weaver
**Class:** Agility | **Attack Type:** Ranged

### Base Stats

| Stat | Value |
|------|-------|
| **Health (HP)** | 72 |
| **Mana** | 35 |
| **Attack** | 8 |
| **Attack Range** | 3 hexes |
| **Defense** | 1 |
| **Move Speed** | 1 |
| **Action Points (AP)** | 10 |

### Stat Scaling
- **Per Level:** +8 HP, +10 Mana, +4 Attack, +1 Defense

### Abilities

---

#### The Swarm
**Type:** Active | **Targeting:** Point Target | **Unlock:** Level 1

**Mana Cost:** 16 | **AP Cost:** 1 | **Cooldown:** 3 rounds | **Range:** 4 hexes

**Effect:**  
Weaver releases a cluster of parasitic weaverlings at a target hex. Apply a **Swarm Beetle token** to each enemy hero on the target hex and all adjacent hexes. At the start of each affected hero's activation, that hero takes damage and suffers -1 Defense while the token remains attached.

**Level Progression:**
- **Level 1-5:** 3 damage per activation, lasts 1 round
- **Level 6-11:** 4 damage per activation, lasts 2 rounds
- **Level 12+:** 5 damage per activation, lasts 2 rounds

**Notes:**  
An affected hero may spend 1 **Attack** action during their activation to remove their own **Swarm Beetle token**. The Defense reduction does not stack from multiple beetles.

---

#### Shukuchi
**Type:** Active | **Targeting:** No Target (Self-Cast) | **Unlock:** Level 1

**Mana Cost:** 10 | **AP Cost:** 1 | **Cooldown:** 2 rounds | **Duration:** Current activation

**Effect:**  
Weaver slips into the folds of reality and becomes **Invisible** for the rest of his current activation. During that activation, each **Move** action Weaver takes may move up to 2 hexes instead of 1. The first time Weaver passes through an enemy unit during each Move action, that unit takes damage.

**Level Progression:**
- **Level 1-5:** 10 damage per pass-through
- **Level 6-11:** 16 damage per pass-through
- **Level 12+:** 22 damage per pass-through

**Notes:**  
Weaver must still end each Move action on a legal Open hex. Shukuchi ends immediately if Weaver uses an **Attack** action or another ability.

---

#### Geminate Attack
**Type:** Passive | **Unlock:** Level 1

**Effect:**  
The first time Weaver resolves an **Attack** action during each activation, he immediately makes a second attack.

**Level Progression:**
- **Level 1-5:** Second attack deals -2 damage
- **Level 6-11:** Second attack deals -1 damage
- **Level 12+:** Second attack deals full damage

**Notes:**  
The second attack must target the same enemy hero, creep, or structure as the first attack.

---

#### Time Lapse
**Type:** Active | **Targeting:** No Target (Self-Cast) | **Unlock:** Level 6

**Mana Cost:** 25 | **AP Cost:** 1 | **Cooldown:** 5 rounds

**Effect:**  
Weaver rewinds himself to the state he had at the start of his previous activation. Move Weaver back to the hex marked by his **Time Lapse marker**, then restore his HP and Mana to the saved values from that snapshot.

**Level Progression:**
- **Level 6-11:** Rewind self
- **Level 12-17:** Rewind self and remove one dispellable debuff
- **Level 18+:** Rewind self and remove all dispellable debuffs

**Notes:**  
At the start of each Weaver activation, place a **Time Lapse marker** on Weaver's current hex and note his current HP and Mana with small number tokens on his Hero Board. If the marked hex is no longer a legal Open hex when Time Lapse resolves, place Weaver on the nearest legal Open hex instead.

**Aghanim's Scepter Upgrade:**  
Time Lapse may target an allied hero within 2 hexes instead of Weaver. Use that hero's saved Time Lapse state.

---

### Design Notes

**Role:** Weaver is an Agility ranged skirmisher who relies on mobility, chip damage, and temporal escape tools to stay alive while constantly pressuring enemies. He excels at being difficult to pin down and punishing heroes who cannot finish him quickly.

**Playstyle Considerations:**
- The Swarm pressures clustered heroes and taxes their actions if they want to remove the beetles
- Shukuchi turns Weaver's movement into offense and lets him reposition aggressively without committing to a full fight
- Geminate Attack gives Weaver consistent ranged harassment and farming efficiency without adding much rules weight
- Time Lapse is Weaver's signature survival tool and rewards careful timing after he has already baited enemy commitment
- Low HP and Defense mean Weaver still dies quickly if caught without Time Lapse or Shukuchi available

**Balance Considerations:**
- The Swarm should feel annoying and valuable, but not lock heroes into spending every activation removing beetles
- Shukuchi must reward pathing and positioning without making Weaver impossible to interact with
- Geminate Attack should be reliable, not swingy, so Weaver's baseline output stays readable
- Time Lapse should create dramatic saves, but its cooldown and snapshot timing should keep it from feeling unconditional
- Weaver should win by attrition and evasion more often than by raw burst damage

**Thematic Identity:**
Weaver embodies the untouchable time-skirmisher: darting through the fight, leaving parasites in his wake, and undoing the damage that should have killed him. His design should feel slippery, irritating, and defined by perfect timing.

---