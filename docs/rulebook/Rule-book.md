# DOTA 2: THE BOARD GAME — RULEBOOK

## Objective
Destroy the enemy team's **Ancient**, located inside their base. To reach the Ancient, a team must destroy all Towers in at least one lane in sequence. The first team to destroy the enemy Ancient wins.

---

## Game Components

- **Hero Boards** — One player mat per hero (approx. 30 × 40 cm) containing the Action Queue for planning tokens, reaction slots, an AP-spent track (0–10), a dual duration tracking system (Turns and Rounds), 6 numbered active item slots and 3 backpack slots, and a status effect grid.
- **Stat Trackers** — Separate 3D-printed trackers per hero for live numeric values: Health, Mana, XP (doubles as Level — see Leveling), Gold, and AP.
- **Hero Cards** — Each hero's printed reference statistics: Attack, Defense, Health, Mana, Move Speed, Attack Range, and AP.
- **Abilities Cards** — One landscape card per hero containing all four abilities, their costs, effects, and upgrade breakpoints.
- **The Board** — A 46 × 46 hex-grid map featuring three lanes (Top, Mid, Bottom), the River, the Jungle, two Bases, Secret Shops, and Roshan's Pit.
- **Shared Game Board** — A central tracking board with a round counter, half-round flip token, Round Start Token, turn order tracker, lane creep wave sliders, tower and barracks hit counters, ward log, Roshan status, and rune tracker.
- **Planning Tokens** — Move, Attack, Pass, 6 numbered item-slot tokens (matching the 6 active item slots on your Hero Board), and hero-specific ability tokens.
- **Tokens** — Creeps, wards, runes, Barracks, invisibility clouds, Smoke clouds, dropped items, status markers, stat modifier tokens (+1/+5/+10), and creep camp tokens.
- **Dice** — D6, D10, and D20 for combat contests, deny attempts, skillshot dodging, and tracking.

Heroes are divided into three classes: **Agility**, **Strength**, and **Intelligence** (Universal heroes are not a separate class in this game).

---

## Game Setup & Draft

### Coin Flip
Flip a coin between the two teams. The winner chooses to either **pick a hero first** or **take the first turn**; the loser gets the other option.

### Draft Modes
Players agree on a mode before setup.

**All Pick (Default):** All Hero Cards are laid face-up.
1. **Ban Phase** — Teams alternate banning one hero at a time (3 bans per team, 6 total). Banned cards are removed face-down. Bans start with the team that lost the coin flip.
2. **Pick Phase** — Teams alternate picking heroes from the remaining pool until each player has selected a hero.

**Single Draft:** Hero Cards are separated by class into three face-down piles (Agility, Strength, Intelligence). Each player draws one card from each pile and chooses one. No ban phase.

**All Random:** All Hero Cards are shuffled. Each player is dealt one card at random. No picks or bans.

### Game Start
All heroes begin with **3× their normal AP** for the first round only, representing the run from the Fountain. Creeps do not spawn during Round 1, so available actions are limited to Move and pre-creep fights.

---

## Game Loop

The game is played in **Rounds**. Each Round consists of **20 turns** — every hero activates twice.

- **Turn** — One hero's activation.
- **Round** — 20 turns (all heroes activate twice).
- **Half-Round** — 10 turns (each hero activates once).
- **Duration** — Effects measured in **rounds** (complete 20-turn cycles) or **turns** (individual activations). The Abilities Card or item entry specifies which. Track durations on your Hero Board's dual tracking system: turn-based effects tick down at the start of that hero's activation; round-based effects tick down during the Round End Phase.

Each Round has three phases: **Planning Phase**, **Turn Phase**, and **Round End Phase**.

---

### Planning Phase

Before each half-round (10 turns), all players simultaneously plan for each hero they control using their **Hero Board**:

1. **Action Queue** — Select **Planning Tokens** (Move, Attack, numbered item-slot tokens 1–6, and hero-specific ability tokens) up to the hero's AP total and place them **face-down** in the **Action Queue** on your Hero Board, laid out left-to-right in execution order.
2. **Reaction Slots** — Commit up to **2 reactions** per hero by placing a token in the dedicated **reaction slots** (physically separate from the Action Queue on your Hero Board). Each reserves 1 AP from the hero's budget and cannot also be used in normal activation.
3. Once all players are ready, the Turn Phase begins.

Tokens remain face-down until that hero's activation. On reveal, actions are executed **left to right** through the Action Queue. Specific targets or destinations are declared at that moment.

**Important rules:**
- Only the **type** of action is committed during planning (e.g. "Move", "Attack", "Storm Hammer", "Item Slot 2"). Specific targets or destinations are declared when the token is revealed during execution.
- Item use is committed by **numbered slot** (matching the 6 labeled active item slots on your Hero Board), not by a generic "Use Item" token. If the slot is empty or holds a freshly swapped item, the action fails.
- Backpack items cannot be committed or used directly. Items swapped from the backpack into an active slot are not usable until the next round.
- Reactions are committed using the dedicated reaction slots on your Hero Board. Any action costing exactly 1 AP may be committed as a reaction. AP reserved for reactions cannot be used in the hero's normal activation. Unused reaction AP is lost at the end of the half-round.
- If a hero loses AP before their activation (e.g. from a stun), remove committed tokens from the Action Queue **left to right** until the removed total equals or exceeds the AP lost. Those actions are lost.

**Strategic note:** Committing action types (not specific targets) gives you flexibility to adapt when your turn arrives, but carries risk — if a target dies before your activation, you must either retarget or cancel.

---

### Turn Phase

Heroes execute their committed actions one at a time, spending all their AP before the next hero activates.

**Turn Order — Pendulum Rotation:**
A **Round Start Token** determines which hero activates first. It cycles through the full hero list in a circular rotation, moving to the next hero at the start of each new round.

Once the starting hero is determined, teams **alternate** (Radiant → Dire → Radiant → ...). The direction flips after 10 turns, creating a pendulum pattern. Turn order alternates by **hero**, not by player — if you control multiple heroes, they are interspersed with enemy heroes.

**Example with 10 heroes (5v5):**
Turns 1–10 (forward): A → V → B → W → C → X → D → Y → E → Z
Turns 11–20 (backward): Z → E → Y → D → X → C → W → B → V → A

Round 2 starts with the next hero in the circular sequence (V), then follows the same pattern.

**General rules:**
- Each hero activates twice per round (once per half-round).
- AP does not carry over between activations or rounds.
- If a committed action cannot be executed, the player may **cancel** (no AP spent, token returned) or **retarget** to a valid alternative. If no valid alternative exists, the action is automatically cancelled.
- Actions that fail due to status effects (stun, silence), insufficient resources, or invalid item slots cannot be retargeted and are simply cancelled.

---

### Reactions

Reactions are pre-committed out-of-turn actions that interrupt an enemy's activation. Only heroes **directly affected** by the triggering action may react — those who are targeted, within the affected area or skillshot path, or eligible to contest a creep kill with a committed Attack reaction.

**How reactions work:**
- A hero normally has **1 reaction slot** per half-round.
- **Observer Ward bonus:** If the acting enemy hero is in an area covered by an allied Observer Ward, each directly affected defender may use **2 reactions** instead of 1.
- Reactions are triggered **after targeting is declared** and **before** the action resolves.
- If multiple defenders react to the same trigger, they resolve in turn order.
- Any committed action costing exactly 1 AP may be used as a reaction.

**Common Reactions:**

| Reaction | Effect |
|---|---|
| **Move (1 AP)** | Reposition 1 hex. If this breaks adjacency or LoS, the triggering action misses. |
| **Defensive Item (1 AP)** | Activate a defensive item immediately. |
| **Attack — Deny (1 AP)** | Commit an Attack token to contest an enemy Attack that would kill an allied lane creep. Both players roll a die — higher roll lands the kill (see Economy). |

**Skillshot Dodging:** A hero may dodge a Skillshot (marked on the Abilities Card) by using a 1 AP movement action or movement ability as a reaction. Both players roll a die — if the reacting hero rolls higher, the Skillshot misses.

> **Example:** Crystal Maiden commits Move into a reaction slot. Juggernaut attacks her from melee range. After targeting, she triggers Move to an adjacent hex. Juggernaut is no longer adjacent — the attack misses.

---

### Round End Phase

After all 20 turns complete, resolve in order. The shared game board tracks round number, half-round direction (forward/backward), and creep wave states.

1. **Creep Spawning** — New waves spawn at the Creep Meeting Point in each lane. The Meeting Point shifts toward the enemy base for each tower destroyed in that lane. Update the creep wave slider on the shared board as needed.
2. **Passive Income** — Every hero receives 10 gold.
3. **Power Rune Spawn** — Every 4th round, a new rune appears (see Runes). Track on the shared board's rune tracker.
4. **Neutral Respawns** — Every even-numbered round, flip all cleared camp tokens back to Populated.
5. **Duration Ticks** — All round-based duration effects on Hero Boards tick down by 1.

---

## Action Points (AP) and Actions

Each hero has a fixed AP value printed on their Hero Card, refreshed at the start of each activation. Track AP spent this activation using the **AP track (0–10)** on your Hero Board — move the marker forward as each action resolves, then reset at the start of your next activation.

| Action | AP Cost | Description |
|--------|---------|-------------|
| **Move** | 1 | Move to an adjacent hex. |
| **Attack** | 1 | Initiate combat against a lane creep, neutral camp, Tower, or enemy hero in range. No separate Farm action. |
| **Attack (Deny)** | 1 (Reaction) | Commit an Attack token to a reaction slot to contest an enemy Attack removing a lane creep's last Hit. |
| **Use Item** | Varies | Activate an item in one of the 6 active item slots (labeled 1–6 on your Hero Board). |
| **Use Ability** | Varies | Activate a hero ability (costs Mana in addition to AP). |

---

## Map & Movement

### Hex Grid & Terrain
The board is a **hex grid**. Each hex belongs to one of these terrain types:

| Terrain | Movement | Line of Sight | Notes |
|---------|----------|---------------|-------|
| **Open** | Passable | Clear | Default — no restrictions. |
| **Tree** | Blocked | Blocked | Can be destroyed by abilities/items. Regrows every 4th round. |
| **Impassable** | Blocked | Blocked | Permanent walls, cliffs, water. Cannot be altered. |
| **Building** | Blocked | Clear | Can be destroyed (becomes Open). |
| **Obstacle** | Blocked | Clear | Permanent — cannot be destroyed. |

Buildings and Obstacles block movement but **do not** block Line of Sight — ranged attacks and abilities can target through them.

Tree clusters contain **Open juke paths** that wind through them — a hero on a juke-path hex is hard to target because surrounding trees block LoS.

**Tree Destruction:** Specific abilities and items (e.g. Tangos) can destroy tree hexes, converting them to Open. All destroyed trees regrow at the end of every 4th round.

### Movement
Each **Move** action costs 1 AP and moves the hero 1 hex to any adjacent hex. Heroes may take multiple Move actions per turn. The **Haste Rune** doubles move efficiency (1 AP = 2 hexes) for its duration.

### Key Areas
- **Fountain** — Instantly restores all Health and Mana to heroes in this area.
- **Lanes** — Three lanes (Top, Mid, Bottom) connecting the bases. Each has a series of Tower positions and Creep Meeting Points.
- **Creep Meeting Points** — Where lane creep waves clash. Marked on the board with 3 positions per team (2 front melee, 1 rear ranged).
- **River** — Central strip between the two sides. Power Runes spawn here.
- **Jungle** — Wilderness between lanes containing Neutral Camps and Ancient Camps. Each team's jungle has 3 safe-lane camps (Easy, Medium, Hard) and 2 off-lane camps (Medium, Ancient).
- **Secret Shops** — One per team, located near the Ancient Camp in each off-lane jungle. Any hero (from either team) may purchase from a Secret Shop by moving into its area, though the item pool is limited to a subset of the full Fountain catalogue.
- **Roshan's Pit** — A fixed area on the Dire side of the river-jungle border. Single entrance facing Radiant. Home to Roshan.

---

## Combat & Status Effects

### Damage Resolution
> **Damage − Defense = Health Lost**

The attacker's Damage and defender's Defense come from their Hero Cards, modified by items and abilities. Lane creeps are an exception — they use the **Hit** system instead (see Creeps).

### Line of Sight
- **Melee attacks** target an adjacent hex — no LoS required.
- **Ranged attacks and targeted abilities** require clear LoS. Draw a straight line between hex centres — if it passes through a Tree or Impassable hex, LoS is blocked.
- **AoE abilities** check LoS per hex unless the Abilities Card says otherwise.

### Attack Range
- **Melee** heroes attack adjacent hexes.
- **Ranged** heroes use the range printed on their Hero Card.

### Status Effects

| Status | Effect |
|--------|--------|
| **Stun** | Removes AP, a turn, or a round. AP stuns remove committed tokens left-to-right until the cost is met. Turn stuns skip the next activation entirely. |
| **Silence** | Prevents ability use. Interrupts channels. Cannot toggle abilities on/off. |
| **Slow** | Taxes movement: the first X AP of Move actions each turn produce 0 hexes of movement. |
| **Root** | Prevents voluntary movement. Other actions allowed normally. |
| **Hex** | Hard disable: cannot attack, use abilities, or use items. Slowed 7 AP. Defense becomes 0. |
| **Disarm** | Prevents Attack actions (including creep/ camp clear). |
| **Break** | Disables passive abilities only. |
| **Ethereal** | Cannot make Attack actions. Physical attacks cannot target you. Magic damage taken is increased. |
| **Spell Immunity** | Blocks enemy abilities and debuffs unless they explicitly **pierce spell immunity**. |
| **DoT** | Deals damage at the start of each activation, then decrements duration. Multiple DoTs stack independently. Same DoT type refreshes duration instead of stacking. Most are dispellable. |

### Ability Types & Targeting

**Activation Methods:**
- **Passive** — Always active. No cost.
- **Active** — Manually cast. Costs Mana and AP.
- **Toggle** — Activated on your turn; can be toggled off at any time unless Silenced.
- **Channeled** — Activated on your turn. Effect persists across turns until interrupted (Stun, Silence, forced movement) or cancelled. Caster must remain stationary.

**Targeting Types:**
- **No Target (Self-Cast)** — Affects only the caster.
- **Unit Target** — Specific unit within range and LoS.
- **Point Target** — A specific hex within range.
- **Direction/Vector Target** — A direction from the caster.

**Effect Shapes:** Circular AoE, Line, Cone, Global.

**Special:**
- **Skillshot** — A line-travel ability that can be dodged (see Reactions). Must be marked on the Abilities Card.
- **Aura** — Continuous passive effect radiating from the hero within a fixed range. Always active while alive.

### Summons
Some abilities create controlled units. Summons have their own stat line (Hits, AP, Attack, Defense, Move Speed) tracked on the Abilities Card. They act during their controller's activation using their own AP. Summon durability is tracked in **Hits** (lose 1 Hit per successful attack or damaging effect; removed at 0 Hits). Summons persist until killed or their duration expires. If the controlling hero dies, their summons are removed unless stated otherwise.

---

## Creeps, Towers & Objectives

### Lane Creeps
Creep waves spawn each Round End Phase and meet at the Creep Meeting Point in each lane. Each wave consists of **2 melee tokens** and **1 ranged token** per team.

- **Melee tokens** are double-sided: one side shows 2 creeps, the other shows 1. Flip on kill. Remove when empty.
- **Ranged tokens** represent 1 ranged creep each.
- Lane creeps use **Hits**, not numeric HP. A successful attack removes 1 Hit.
- **Normal Creeps:** 1 Hit. **Super Creeps:** 2 Hits. **Mega Creeps:** 2 Hits.
- When a Super or Mega creep has taken 1 Hit but is still alive, mark it with a **Creep Damage Marker** (max 1 per token).
- AoE and cleave effects remove 1 Hit from each affected creep separately. Resolve one creep at a time.

### Lane Creep States
When a team's Barracks is destroyed, the **opposing team's** creeps in that lane become **Super Creeps** (3 gold, 1 XP to closest hero). If all 3 Barracks fall, all lanes produce **Mega Creeps** (3 gold, 1 XP, and basic attacks against them deal 5 retaliation damage — once per attack regardless of how many Mega Creeps are hit).

### Barracks
Three Barracks per team (one per lane), located behind the Tier 3 Tower. They have fixed HP, deal no retaliation damage, and follow the same siege requirement as Towers. Destroying a Barracks awards **50 gold** to every allied hero and upgrades the enemy's creeps in that lane to Super Creeps.

### Towers & Siege
Towers must be destroyed in sequence per lane: **Tier 1 → Tier 2 → Tier 3 → Tier 4 → Ancient**. Each tower has Hits — a successful Attack removes 1 Hit.

| Tower | Hits |
|---|---|
| **Tier 1** | 10 |
| **Tier 2** | 15 |
| **Tier 3** | 18 |
| **Tier 4** | 20 |
| **Ancient** | 30 |

- A Tower can only be attacked if the **enemy creep wave in that lane is exhausted** for the round. Mark this on the shared board's creep wave exhausted checkbox.
- Towers deal **5 damage** to the attacker per hit (reduced by the number of allied creeps present).
- **Tower aggro — allied creeps alive:** Whenever an enemy hero enters within **3 hexes** of a tower while allied creeps are alive in that lane, the tower immediately deals **5 damage** (diving penalty). Fires again each activation the conditions hold.
- **Tower aggro — hero protection:** If all allied creeps are dead, proximity alone does not trigger aggro. But attacking an allied hero within 3 hexes of the tower draws 5 damage from the tower.
- Destroying a tower awards gold to every hero on the destroying team: **Tier 1 — 30g, Tier 2 — 50g, Tier 3 — 75g, Tier 4 — 100g**.
- The **Ancient** cannot be attacked until both Tier 4 Towers are destroyed.

### Neutral & Ancient Camps
Located in the Jungle. Attack them using normal Attack actions. Neutrals deal Health damage back. Camps respawn every even-numbered round if cleared. Ancient Camps are stronger, deal more damage, and award more gold and XP.

### Roshan & Aegis
Roshan resides in Roshan's Pit. He is a powerful neutral — attacks deal significant damage. On death, he drops the **Aegis of the Immortal** and awards **50 gold** and **10 XP** to every allied hero. If both teams are present at his death, a die roll determines which team claims the rewards.

**Aegis of the Immortal:** The holder revives in place with full Health and Mana upon death, consuming the Aegis. This bypasses the normal respawn timer and Buyback cost.

Roshan respawns after a fixed number of rounds. His current HP is tracked on the Roshan track printed on the board.

---

## Economy & Progression

### Gold

**Creep Kills:**
- **Normal Lane Creep:** 5 gold to the killer. 2 shared XP to allied heroes within 4 hexes (split between the 2 closest eligible heroes).
- **Super/Mega Creep:** 3 gold to the killer. 1 XP to the closest allied hero within 4 hexes.
- **Neutral/Ancient Camps:** Gold and XP as printed on the camp. Hero loses Health (neutrals fight back).

**Hero Kills:**
- **Killer:** 10 × killed hero's level gold.
- **Assisters:** killed hero's level gold each. A hero is counted as an assister if they damaged the killed hero or applied a debuff to them during the current round.

**Passive Income:** Every hero receives 10 gold each Round End Phase.

**Deny:** There is no dedicated Deny token. An allied hero commits an **Attack** token to a reaction slot during planning. When an enemy attacks a lane creep on its last remaining Hit, the ally may trigger their Attack reaction against the same creep. Both players roll a die — the higher roll lands the kill. If the denier wins, the attacker gets no gold and only 1 XP goes to the closest eligible attacker.

**Gold Uses:** Purchase items at the Fountain shop or pay the Buyback fee.

### XP & Leveling
Heroes gain XP when an enemy unit dies within **4 hexes** of them. **Level = XP ÷ 10** (rounded down). Each level grants the per-level stat increase printed on the Hero Card.

Hero kills grant **5 + killed hero's level** XP, split equally among allies in range (closest receives any remainder). Creep kills: 2 XP for normal, 1 XP for Super/Mega.

**Example:**
```
A level 8 hero dies with 3 allies in range. Total XP = 13. 
13 / 3 = 4 and a remainder of 1. 
So the closest hero gets 5 XP, the other two heroes get 4 XP each.
```
Heroes start with one ability unlocked. Each level from 2–4 unlocks an additional ability. At level 5 the hero gains stats only. Level 6 unlocks the ultimate and upgrades all abilities. Further upgrades at levels 12 and 18.

| XP | Level | Milestone |
|---|---|---|
| **60** | **6** | Ultimate unlocked. All abilities upgrade. |
| **120** | **12** | Abilities upgrade. |
| **180** | **18** | Final ability upgrade. |

### Items & the Shop

**Purchasing:** Items are bought at the Fountain. A hero must be at the Fountain to purchase directly, or use the Courier for remote delivery.

**Inventory:** Each hero has **6 active item slots** (labeled 1–6 on your Hero Board, matching your numbered planning tokens) and **3 backpack slots** (also on the Hero Board). Only active slots provide passive bonuses and can be activated with item-slot tokens. Backpack items are storage only — they cannot be used or provide bonuses. Items swapped from the backpack into an active slot become usable at the **start of the next round**.

**The Courier:** A shared team token that delivers items from the Fountain to heroes in the field. Delivery takes 1–2 rounds. The Courier can be killed by enemy heroes — any items being carried are lost.

**Aghanim's Scepter:** A high-cost item that permanently upgrades one ability (marked on the Abilities Card). The upgrade is immediate upon purchase and requires no activation.

---

## Respawn & Buyback

### Respawn
When a hero dies, they are removed from the board. The respawn timer equals their **current level in turns** (counted across all players). On the respawn turn, the hero returns to the Fountain with full Health and Mana at the start of that turn.

### Buyback
A dead hero may pay a gold fee (scaling with level) to respawn immediately at the Fountain. Buyback bypasses the respawn timer. After use, the hero cannot Buyback again for a set number of rounds (tracked with the hero's Buyback token on the round cooldown track). If a hero buybacks during a half-round they haven't yet activated in, they return immediately and can participate in that half-round's Planning Phase.

---

## Vision & Invisibility

### Default Visibility
All units are visible unless they have the **Invisibility** status.

### Observer Wards
A consumable placed on any Open hex. Covers a radius of hexes (see Item Card). While active:
- If an enemy hero in a warded area attacks or uses an ability, each directly affected allied hero may use **2 reactions** during that half-round instead of 1.
- Observer Wards do **not** reveal invisible units — use Sentry Wards or Dust for detection.
- They can be destroyed by enemy heroes (1 AP while adjacent).

Observer Wards last for a set number of rounds. Track their location and remaining duration on the shared board's ward log grid.

### Sentry Wards & Dust of Appearance
- **Sentry Wards:** A consumable that reveals any Invisibility Cloud entering its area.
- **Dust of Appearance:** A consumable that creates a mobile Reveal radius around the using hero for the current round.

### Invisibility Mechanics
When a hero becomes invisible:
1. Replace the hero token with an **Invisibility Cloud** (multi-hex token with numbered spaces).
2. Secretly record which numbered space the hero occupies on a hidden counter.
3. The cloud moves as a single unit. Update the hidden number each time it moves.
4. The cloud cannot be targeted by single-target attacks or abilities.
5. **AoE abilities** may target specific cloud hexes. If the hex matches the hidden number, the hero is revealed. If it misses, the owner may choose a new hidden number.
6. **Attacking from Invisibility:** Defending heroes cannot use reactions against the attack. The attacker is revealed immediately after the attack resolves.

### Smoke of Deceit
A consumable granting **group invisibility** to the user and all allied heroes within a fixed radius. Affected heroes move together under a single **Smoke Cloud** token.

- Each hero secretly records their own numbered space within the cloud.
- The hero who activates Smoke **cannot attack or use offensive abilities** for the remainder of that turn.
- Smoke **dispels** if any affected hero moves within 3 hexes of an enemy, enters a Tower's area of control, or attacks.
- Heroes under Smoke are invisible to Observer Wards and do not trigger the reaction bonus.

---

## Runes

Every **4th round**, a Power Rune spawns at one of two River positions. Determine the type, then flip a coin for which side. A hero claims the rune by moving into its area. Only one rune exists at a time.

| Rune | Effect |
|------|--------|
| **Illusion** | Creates 3 controlled Illusion tokens. Deal reduced damage, take increased damage. |
| **Haste** | Move actions move 2 hexes per AP for the duration. |
| **Invisibility** | Grants Invisibility status. |
| **Regeneration** | Restores full Health and Mana. Can be interrupted by enemy attack. |
| **Double Damage** | All attacks deal double Damage value for the duration. |

---

*Document version aligned with mechanics reference. All rules default to the detailed mechanics documents where conflicts arise.*
