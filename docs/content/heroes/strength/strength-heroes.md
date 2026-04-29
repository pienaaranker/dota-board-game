# DOTA 2: THE BOARD GAME — STRENGTH HERO CARDS

This document contains the current full card designs for Strength heroes.

For draft rules and class-wide roster status, see [../hero-shortlist.md](../hero-shortlist.md). For the full hero card index, see [../roster.md](../roster.md).

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
Sven's attacks cleave in a 2-hex cone in front of him, dealing damage to all units in the area. Against a normal lane wave, this lets Sven clear the full wave in 2 successful attacks if his cone covers both melee tokens and the ranged token, and he receives the normal gold and XP for each creep killed.

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
Launches a bloody hook in a straight line in the chosen direction. The hook travels up to 5 hexes or until it hits an enemy hero or creep. The first unit struck takes damage and is pulled back to the hex adjacent to Pudge. Enemies may attempt to dodge the hook by using a committed 1 AP movement action or 1 AP movement ability as a reaction.

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
Pudge channels his ultimate on target enemy hero within 1 hex, dealing damage per turn and disabling the target completely. **Dismember pierces spell immunity.** The target cannot move, attack, or use abilities while Dismembered. Pudge must remain adjacent to the target while channeling. Interrupted by Stun, Silence, forced movement (Pudge or target), or if Pudge voluntarily cancels.

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

## Magnus
**Class:** Strength | **Attack Type:** Melee

### Base Stats

| Stat | Value |
|------|-------|
| **Health (HP)** | 105 |
| **Mana** | 35 |
| **Attack** | 9 |
| **Attack Range** | 1 hex |
| **Defense** | 3 |
| **Move Speed** | 1 |
| **Action Points (AP)** | 10 |

### Stat Scaling
- **Per Level:** +12 HP, +8 Mana, +4 Attack, +1 Defense

### Abilities

---

#### Shockwave
**Type:** Active | **Targeting:** Direction/Vector | **Unlock:** Level 1

**Mana Cost:** 12 | **AP Cost:** 1 | **Cooldown:** 2 rounds | **Range:** 4 hexes

**Effect:**  
Magnus sends a wave of force in a straight line up to 4 hexes. Enemy units in the path take damage and are pulled 1 hex toward Magnus, if a legal Open hex is available. Enemy heroes hit by Shockwave are also **Slowed 1 AP until the end of their next activation**.

**Level Progression:**
- **Level 1-5:** 16 damage
- **Level 6-11:** 24 damage
- **Level 12+:** 32 damage

**Notes:**  
For Shockwave, **Slowed** means the affected hero is **Slowed 1 AP until the end of their next activation**.

---

#### Empower
**Type:** Active | **Targeting:** Unit Target | **Unlock:** Level 1

**Mana Cost:** 10 | **AP Cost:** 1 | **Cooldown:** 3 rounds | **Range:** 2 hexes | **Duration:** 1 round

**Effect:**  
Magnus empowers an allied hero or himself with crushing momentum. The empowered hero gains bonus Attack, and their **Attack** actions cleave in a 2-hex cone in front of them, dealing bonus damage to all other enemy units in the cone.

**Level Progression:**
- **Level 1-5:** +3 Attack, 2 cleave damage
- **Level 6-11:** +5 Attack, 3 cleave damage
- **Level 12+:** +7 Attack, 4 cleave damage

---

#### Skewer
**Type:** Active | **Targeting:** Direction/Vector | **Unlock:** Level 1

**Mana Cost:** 16 | **AP Cost:** 2 | **Cooldown:** 3 rounds | **Range:** Up to 3 hexes

**Effect:**  
Magnus charges in a straight line up to 3 hexes. Enemy heroes in his path take damage and are dragged with him. After Magnus finishes moving, place each dragged hero on a legal Open hex adjacent to Magnus.

**Level Progression:**
- **Level 1-5:** 15 damage
- **Level 6-11:** 25 damage
- **Level 12+:** 35 damage

**Notes:**  
Magnus may move through occupied hexes during Skewer, but must end on a legal Open hex. If multiple heroes are dragged, the Magnus player chooses the order in which they are placed adjacent to Magnus.

---

#### Reverse Polarity
**Type:** Active | **Targeting:** No Target (Self-Cast) | **Unlock:** Level 6

**Mana Cost:** 30 | **AP Cost:** 2 | **Cooldown:** 5 rounds | **Radius:** 2 hexes

**Effect:**  
Magnus violently reverses the battlefield's pull. **Reverse Polarity pierces spell immunity.** All enemy heroes within 2 hexes are pulled onto the single hex directly in front of Magnus, take damage, and are stunned. For the rest of Magnus's current activation, those heroes may temporarily share that hex so Magnus can follow up with abilities such as Skewer.

**Level Progression:**
- **Level 6-11:** 20 damage, stun (3 AP loss)
- **Level 12-17:** 30 damage, stun (4 AP loss)
- **Level 18+:** 40 damage, stun (5 AP loss)

**Notes:**  
When Magnus's activation ends, all heroes stacked by Reverse Polarity are immediately dispersed to legal Open hexes adjacent to Magnus. The Magnus player chooses the placement order if multiple legal hexes are available.

**Aghanim's Scepter Upgrade:**  
Reverse Polarity radius increases to 3 hexes.

---

### Design Notes

**Role:** Magnus is a Strength melee initiator who controls fights through forced movement and teamfight setup. He enables allied carries with Empower, isolates enemies with Skewer and Shockwave, and punishes clustered teams with Reverse Polarity.

**Playstyle Considerations:**
- Shockwave gives Magnus safe reach and small-scale displacement before he commits
- Empower lets Magnus support an allied core or turn himself into a stronger wave-clear threat
- Skewer is his key repositioning tool, allowing him to start fights, peel for allies, or drag enemies into danger
- Reverse Polarity is his signature teamfight swing and should reward patience, angle-finding, and enemy clumping
- Magnus is durable enough to engage first, but he still relies on timing and allied follow-up to convert positioning wins into kills

**Balance Considerations:**
- Shockwave should be useful poke and setup, not a full initiation by itself
- Empower needs to feel worth casting on allies without invalidating other damage-buff heroes or items
- Skewer should be threatening because of its displacement value more than its raw damage
- Reverse Polarity must be game-changing when it catches multiple heroes, but its radius and cooldown should leave room for counterplay
- Magnus should feel like an initiator first and a carry second, even when Empowering himself

**Thematic Identity:**
Magnus embodies the horned battlefield controller: a brutal frontliner who bends enemy positioning to his will and creates perfect openings for his team. His design should feel forceful, deliberate, and defined by decisive initiation moments.

---