# DOTA 2: THE BOARD GAME — MECHANICS REFERENCE

This document is the single source of truth for how every mechanic in the game works. It is organized by system, not by design priority.

Entries marked **🔄 Pending Discussion** have their broad intent defined but need a specific ruling before they are final. All other entries are settled and reflect the current design.

---

## 1. Objective

Destroy the enemy team's **Ancient**, located inside their base. To reach the Ancient, a team must destroy all Towers in at least one lane in sequence. The first team to destroy the enemy Ancient wins.

---

## 2. Game Setup & Draft

### Hero Classes
Heroes are divided into two stat-based classes: **Agility** and **Strength** and **Intelligence**. **Universal heroes are not included in this game.**

### Coin Flip
Before drafting, a coin is flipped between the two teams. The winner chooses to either **pick a hero first** or **take the first turn**; the loser receives the other option.

### Draft Modes
Three draft modes are available. Players agree on a mode before setup.

---

#### All Pick (Default)
All Hero Cards are laid face-up. Each team takes turns **banning** heroes before any picks are made.

**Ban Phase:**
1. Teams alternate banning one hero at a time — **3 bans per team**, 6 bans total.
2. Banned hero cards are removed from the pool face-down for the duration of the game.
3. Bans alternate starting with the team that **did not** win the coin flip.

**Pick Phase:**
After all bans are resolved, teams alternate picking heroes from the remaining pool — one hero per team per pick — until each player has selected their hero.

---

#### Single Draft
Hero Cards are separated into three face-down piles by class: **Agility**, **Strength**, and **Intelligence**. Each pile is shuffled.

1. One card is drawn from **each pile** for every player on both teams.
2. Each player is presented with their 3 drawn cards (one of each class) and chooses one.
3. Unchosen cards are returned to the bottom of their respective piles.
4. There is no ban phase in Single Draft.

---

#### All Random
All Hero Cards are shuffled together into a single face-down deck.

1. Each player is dealt **one card** at random — that is their hero for the game.
2. No picks, no bans. Players must play the hero they receive.

---

### Game Start — Bonus AP
All heroes begin with **3× their normal AP** for the first round only. This represents the run-out-of-fountain period. Creeps do not spawn during Round 1, so available actions are limited to **Move** and level-1 fights.

---

## 3. Game Loop

The game is played in **Rounds**. Each Round has two phases.

### Turn Phase
Heroes activate one at a time within a round. Each hero spends all their AP before the next hero activates.

**Turn Order — Pendulum Rotation:**
The **Round Start Token** determines who goes first each round, then players activate in alternating team order. The direction (forward or backward through the player sequence) alternates each round, creating a "pendulum" pattern.

- **Round 1:** Player with the Round Start Token goes first. Play proceeds forward (e.g., Player 1 → Player 2 → Player 3 → Player 4 → Player 5 → Player 6).
- **Round 2:** The last player to act in Round 1 goes first. Play proceeds backward (e.g., Player 6 → Player 5 → Player 4 → Player 3 → Player 2 → Player 1).
- **Round 3:** The Round Start Token moves to the next player in sequence (e.g., Player 2). Play proceeds forward (e.g., Player 2 → Player 3 → Player 4 → Player 5 → Player 6 → Player 1, wrapping around).
- **Round 4:** The last player to act in Round 3 goes first. Play proceeds backward (e.g., Player 1 → Player 6 → Player 5 → Player 4 → Player 3 → Player 2).
- **Round 5:** The Round Start Token moves to the next player in sequence (e.g., Player 3), and so on.

This ensures positional fairness over time — no player is always first or always last.

**General Rules:**
- A player may pass their remaining AP at any time, ending that hero's turn early.
- AP does not carry over between rounds.

### Reactions
When an active hero targets your hero with an attack or ability, you may **React** before the effect resolves. Reactions interrupt the active hero's turn, are resolved immediately, and then the active hero continues.

**Rules:**
- A hero may only **react once** per opposing hero's turn (not once per round — once per activation).
- **Exception — Observer Ward Coverage:** If the attacking hero is standing in an area covered by an enemy **Observer Ward**, the defending team's heroes may react **twice** during that hero's activation instead of once. This represents the tactical advantage of having vision and awareness of enemy positioning.
- Reactions are **always paid from the reacting hero's next turn AP**. The cost is deducted at the start of that hero's next turn — they simply have that many fewer AP to spend.
- Only the **targeted hero** may react, not teammates.

**Reaction Types:**

| Reaction | AP Cost (from next turn) | Effect |
|---|---|---|
| **Flee** | 2 AP | Move 1 hex in any direction before the attack or ability resolves. If the attacker required adjacency or LoS, the attack misses entirely. |
| **Activate Defensive Item** | 1 AP | Immediately trigger a held defensive Item Card (e.g. BKB equivalent) before damage is applied. The item's effect takes place before resolution. |
| **Deny** | 1 AP | Contest an allied creep's last hit to deny the enemy gold and XP. See §8 for full rules. |
| **Dodge Skillshot** | 2 AP | Roll a die to attempt to dodge an incoming Skillshot ability. On success, the ability misses. On failure, the ability hits normally. Regardless of outcome, the hero must immediately move to an adjacent hex. Only usable against abilities marked as Skillshot. |

> **Example:** Juggernaut (4 AP) attacks Crystal Maiden. She reacts with **Flee** (costs 2 AP from her next turn), moving 1 hex away. Juggernaut is melee — he no longer has adjacency — so the attack misses. On Crystal Maiden's next turn she has 2 fewer AP to spend.

### Round End Phase
After all heroes on both sides have completed their turns, the following occur in order:

1. **Creep Spawning** — A new creep wave appears at the Creep Meeting Point in each lane (skipped during Round 1).
2. **Passive Income** — Every hero receives a fixed amount of gold regardless of activity.
3. **Power Rune Spawn** — On every 4th round, any player rolls the custom Rune Die and flips a coin simultaneously to determine the rune type and which river position it spawns at. See §13.
4. **Neutral Respawns** — On every even-numbered round, all cleared jungle camps are replenished.

---

## 4. The Board

The board represents the battlefield, divided into named areas. Heroes, creeps, and tokens occupy these areas.

### Hex Grid & Terrain
The entire map is built on a **hex grid**. Every hex is one of three terrain types, and some hexes contain structures that further restrict movement:

| Terrain Type | Movement | Line of Sight | Notes |
|---|---|---|---|
| **Open** | Passable | Clear | Default hex — no restrictions. |
| **Tree** | **Blocked** | **Blocked** | Impassable unless an ability says otherwise; blocks LoS; can be destroyed. |
| **Impassable** | **Blocked** | **Blocked** | Permanent walls, cliffs, and water. Cannot be entered or seen through under any circumstances. |

The key difference between **Tree** and **Impassable**: trees can be destroyed and converted to Open hexes; impassable terrain is permanent.

### Buildings & Obstacles
Some hexes contain **structures** that block movement but **do not block Line of Sight**. Heroes can see through them but cannot enter them.

| Structure Type | Movement | Line of Sight | Notes |
|---|---|---|---|
| **Building** | **Blocked** | Clear | Blocks movement; does **not** block LoS. Can be destroyed — once destroyed the hex becomes Open. Examples: base interior walls, reinforcing structures near objectives. |
| **Obstacle** | **Blocked** | Clear | Blocks movement; does **not** block LoS. **Permanent** — cannot be destroyed or removed under any circumstances. Examples: rock formations, fountain pillars, decorative terrain features. |

The key difference between **Building** and **Obstacle**: Buildings can be destroyed through combat (removing the movement block permanently); Obstacles are fixed features of the map.

Neither Buildings nor Obstacles affect LoS — ranged attacks and abilities can target units on the far side of them freely.

Tree clusters contain **Open hexes that wind through them** — these are juke paths. A hero on an Open hex inside a tree cluster is hard to chase because surrounding tree hexes block the enemy's Line of Sight, even though the hero is not inside a tree themselves.

**Named areas** (Jungle Camps, Creep Meeting Points, Roshan's Pit, etc.) are clusters of hexes identified on the board art. When rules reference "being in an area," the hero's token must be on any **Open hex** within that area.

### Tree Destruction
Trees are **mutable terrain** — specific Ability Cards and Item Cards can remove them.

- When a tree hex is destroyed it immediately becomes an **Open hex**.
- **All** destroyed trees regrow simultaneously at the end of every **4th Round** (Rounds 4, 8, 12, …), regardless of when they were destroyed during that interval.
- **Tangos** (Item Card): A hero consumes a Tango charge while **adjacent to** a tree hex — that tree is destroyed and the hero restores a fixed amount of Health.
- Other tree-removing effects (e.g., Whirling Death) specify their area of destruction on the Ability Card.
- An ability that allows a hero to **pass through** tree hexes must explicitly state it on the card.

---

### Lanes
Three lanes run between the two bases: **Top**, **Mid**, and **Bottom**. Each lane has a series of Tower positions and Creep Meeting Points.

### Bases
Each team has a base containing:
- The **Fountain** — restores full Health and Mana to any hero that enters.
- The **Ancient** — the win condition structure.
- **Tier 4 Towers** — two towers guarding the Ancient directly.
- **Barracks** — three buildings inside the base, one corresponding to each lane. Barracks can be sieged once the Tier 3 Tower in their lane has been destroyed.

### River
The central horizontal strip of the map. The **Power Rune** spawns here. Used as a travel and gank corridor.

### Jungle
Unclaimed wilderness areas between lanes on each side of the map. Contains **Neutral Camps** and **Ancient Camps**. Heroes may enter to farm or contest objectives.

### Roshan's Pit
A dedicated area in the river-jungle region. Home to Roshan (see §12).

---

## 5. Action Points (AP) & Actions

Each hero has a fixed AP value printed on their Hero Card. All AP is refreshed at the start of that hero's turn each round.

| Action | AP Cost | Description |
|---|---|---|
| **Move** | 1 | Move the hero token to one adjacent area on the board. |
| **Attack** | 1 | Initiate combat against a Creep, Tower, or Enemy Hero in range. |
| **Farm** | 1 | Secure gold and XP from a creep wave or neutral camp in the hero's current area. |
| **Deny** | Reaction | Spend 1 AP from your *next* turn to contest an enemy Farm action. Requires a die roll. See §8. |
| **Use Item** | Varies | Activate an Item Card's effect. Cost listed on the card. |
| **Use Ability** | Varies | Activate a hero Ability Card. Costs Mana and any AP listed on the card. |

---

## 6. Movement

- Each **Move** action costs 1 AP and moves the hero **1 hex** to any of the 6 adjacent hexes.
- Heroes may take multiple Move actions in a turn to travel farther.
- **Tree hexes and Impassable hexes** cannot be entered. Heroes must navigate around them or through Open juke paths within tree clusters.
- Certain Ability Cards explicitly allow a hero to blink or pass through tree hexes — this must be stated on the card.
- Melee and Ranged heroes move identically; hero type only affects attack range and Line of Sight requirements.
- The **Haste Rune** doubles move efficiency — 1 AP moves the hero **2 hexes** — for its duration.

---

## 7. Combat

### Damage Resolution
All combat uses the formula:

> **Damage − Defense = Health Lost**

The attacker's Damage and the defender's Defense are taken from their Hero Cards, modified by any active items and abilities.

### Line of Sight (LoS)
- **Melee Attacks** target an adjacent hex and do **not** require clear LoS.
- **Ranged Attacks and targeted Abilities** require an unobstructed line between the attacker's hex and the target's hex.
- To check LoS: draw a straight line between the two hex centres. If that line passes through any **Tree hex** or **Impassable hex**, LoS is blocked and the attack or ability cannot be used from that position.
- **AoE abilities** apply the same check per hex — only hexes with clear LoS from the caster are affected, unless the Ability Card states otherwise.

### Attack Range
- **Melee** heroes must be on a hex **adjacent** to their target to attack. No LoS required.
- **Ranged** heroes may attack a target up to **2 hexes** away but require **clear Line of Sight** (see above).

### Crowd Control (CC)
| Status Effect | Mechanical Effect |
|---|---|
| **Stun** | Target loses AP equal to the stun value from their *next* turn. |
| **Silence** | Target cannot use Ability Cards for the remainder of the current round and their next turn. |
| **Slow** | Defined per card — typically reduces effective movement areas per AP. |
| **DoT (Damage over Time)** | See below. |

### Damage over Time (DoT)

A DoT is a debuff token placed on a hero. At the **start of that hero's turn**, the DoT deals its damage and decrements its duration by 1. When the duration reaches 0, the token is removed.

**DoT rules:**
- Each DoT token specifies: damage per tick, tick frequency (every turn or every round), and total duration.
- Multiple different DoT tokens can be active on a hero simultaneously; each ticks independently.
- The same DoT type does **not** stack — applying it again refreshes the duration instead.
- Most DoTs are **dispellable**: they can be removed by items or abilities that cleanse debuffs (e.g. Eul's Scepter of Divinity, Guardian Greaves). The item or ability card will state if it dispels debuffs.
- Some DoTs are marked **undispellable** on the card or item entry — these cannot be removed early.

**Named DoT types used in this game:**

| DoT Type | Damage | Frequency | Notes |
|---|---|---|---|
| **Bleed** | X physical damage | Once per turn | Applied by Blood Grenade. Dispellable. |

### Death
When a hero's Health reaches 0 they are removed from the board and enter a respawn countdown (see §15).

---

## 8. Farming & Economy

### Farm Action
A hero in the same area as a creep wave or neutral camp spends 1 AP to **Farm**.

- **Lane Creeps:** Remove 1 creep counter from the wave. The hero receives **gold and XP** for that creep.
- **Neutral/Ancient Camps:** Remove 1 creep counter from the camp. The hero receives **gold and XP** but also loses **Health** (neutrals fight back).
- **If Denied:** An enemy hero may use the Deny reaction (see below). If the Deny succeeds, the farming hero receives **reduced XP and no gold**.

No die roll is required to farm — spending the AP secures the last hit unless interrupted by a Deny reaction.

### Passive Income
Every hero receives a flat gold amount at the **Round End Phase**, regardless of farming activity.

### Deny
Deny is a **Reaction** (see §3) costing **1 AP from the reacting hero's next turn**. An allied hero may react to an enemy's Farm action targeting an allied creep wave to attempt to deny the last hit, depriving the enemy of gold.

- Resolved with a **die roll challenge** between the denying hero and the farming hero.
- **Deny succeeds:** The farming hero gains **reduced XP and no gold** from that creep.
- **Deny fails:** Farm proceeds normally — the enemy receives full gold and XP.

### Gold Uses
Gold is spent to:
- Purchase **Item Cards** at the Fountain shop.
- Pay the **Buyback** fee to respawn immediately.

---

## 9. XP & Leveling

### Earning XP
Heroes gain XP from:
- Farming lane creep waves.
- Killing or assisting in the death of an enemy hero (shared among nearby allied heroes).
- Farming Neutral or Ancient Camps.

### Leveling Up
Heroes level up when their XP track is filled. Milestones:

| Level | Effect |
|---|---|
| **6** | Unlock a new Ability Card. |
| **12** | Upgrade existing Ability Cards. |
| **18** | Final Ability Card unlock or upgrade. |

All other level-ups provide stat increases as printed on the Hero Card.

---

## 10. Creeps

### Lane Creeps
Creep waves spawn at the Round End Phase from each team's base and meet at the **Creep Meeting Point** — the midpoint between the two nearest standing towers on opposite sides of a lane.

- The Meeting Point shifts **toward the enemy during Round End Phase** when a tower on that side has been destroyed. The shift takes effect when the new creep wave spawns, causing creeps to appear at the advanced position and creating immediate lane pressure.
- Lane creeps may only be Farmed at the Meeting Point.
- A creep wave persists until Farmed or replaced by the next wave.
- Each lane's meeting point hexes are pre-marked on the board with visual indicators.

### Lane Creep States
Lane creep strength scales based on how many enemy Barracks have been destroyed. When a team's Barracks falls, the **opposing team's** creeps in that lane become stronger.

| State | Trigger | AP to Farm a Wave | Health Cost to Farm | Gold Awarded |
|---|---|---|---|---|
| **Normal** | Barracks standing | Standard | None | Full |
| **Enhanced** | That lane's Barracks has been destroyed | +2 AP | None | Reduced |
| **Mega Creeps** | All 3 Barracks destroyed | +4 AP | Yes — same as Neutral Camps | Reduced further |

- Enhanced and Mega creep states apply **per lane** until all 3 Barracks fall, at which point Mega Creeps replace Enhanced everywhere.
- Reduced gold reflects the difficulty of farming tougher creeps — you spend more resources for a worse return.
- Passive Income is unaffected by creep state.
- Barracks cannot be rebuilt once destroyed.

### Neutral Camps
Located in the Jungle. Contain neutral creeps that belong to neither team.

- A hero Farms a Neutral Camp by spending 1 AP while in the camp's area.
- Farming costs the hero **Health** (the neutrals fight back).
- Neutral Camps do **not** require a lane creep wave to be exhausted first.
- Camps respawn on every **even-numbered round** if cleared.

### Ancient Camps
Stronger neutral camps found deep in the Jungle.

- Cost **more AP** to Farm and deal **more Health damage**.
- Award commensurately higher gold and XP.

---

## 11. Towers & Siege

### Tower Tier Progression
Structures must be destroyed in the following order per lane:

> **Tier 1 → Tier 2 → Tier 3 → Barracks / Tier 4 Towers → Ancient**

- A higher-tier tower cannot be attacked until all lower-tier towers in that lane are destroyed.
- Once the Tier 3 Tower in a lane falls, heroes gain access to the **base interior** for that lane. Both the **Barracks** for that lane and the **Tier 4 Towers** may then be sieged.
- The **Ancient** cannot be attacked until both Tier 4 Towers are destroyed.

### Barracks
Each team has three Barracks buildings, one per lane, located in the base interior behind the Tier 3 Tower.

- Barracks use the same **Siege Requirement** as towers: the allied creep wave in that lane must be exhausted before heroes can attack.
- Barracks have a fixed HP value and do **not** deal retaliation damage to attackers (unlike towers).
- When a Barracks is destroyed, place a **Fallen Barracks token** on that lane. The opposing team's creeps immediately become **Enhanced** in that lane (see §10).
- If all 3 Barracks fall, replace all lane tokens with a **Mega Creeps token**. All lane creeps for the opposing team immediately become **Mega Creeps** (see §10).
- Destroying a Barracks awards a **gold bonus** to all heroes on the attacking team.

### Siege Requirement
A Tower may only be attacked if the **enemy creep wave in that lane has been exhausted** for the current round. Creeps must be cleared before heroes can deal damage to a tower.

### Tower Attack Damage
When a hero attacks a tower, the tower deals a **Health penalty** back to the attacker. This penalty is **reduced** (or nullified) by the number of allied lane creeps present in the area — creep bodies absorb tower aggro.

---

## 12. Roshan

Roshan occupies **Roshan's Pit**, a fixed area on the board.

- Any hero or team may attack Roshan. He is treated as a very powerful neutral camp — he deals significant Health damage to attackers.
- Upon death, Roshan drops the **Aegis of the Immortal**.
- If heroes from **both teams** are present when Roshan dies, a **die roll** determines which team claims the Aegis.
- Roshan **respawns** after a fixed number of rounds.

### Aegis of the Immortal
- The holding hero **revives in place** upon death with full Health and Mana, consuming the Aegis.
- Aegis revival bypasses the normal respawn timer and Buyback cost.

---

## 13. Power Runes

Every **4th round**, a Power Rune spawns at one of two designated **River rune positions** — one on the Radiant side, one on the Dire side. At the **start of that round**, any player simultaneously rolls the **custom Rune Die** (determines rune type) and flips a **coin** (determines which side receives it). Both results are resolved together and immediately known to both teams. Only one rune exists on the board at a time.

| Rune | Effect |
|---|---|
| **Illusion** | Creates 3 Illusion tokens controlled by the hero. Illusions deal reduced damage and take increased damage. |
| **Haste** | Move actions move the hero 2 areas per AP spent, for the duration. |
| **Invisibility** | Grants the hero the Invisibility status (see §14). |
| **Regeneration** | Restores full Health and Mana. Can be interrupted by an enemy attack before completion, reducing the amount restored. |
| **Double Damage** | All attacks deal double the hero's Damage value, for the duration. |

- A hero claims the rune by moving into its area.
- Only one rune exists on the board at a time. An unclaimed rune remains until picked up or replaced at the next spawn.

---

## 14. Vision & Invisibility

### Default Visibility
All units are **visible** to both teams unless they have the Invisibility status.

### Gaining Invisibility
Invisibility is granted by:
- The **Invisibility Rune** (see §13).
- Certain **Ability Cards** and **Item Cards**.
- **Smoke of Deceit** — grants group invisibility that bypasses Observer Wards (see below).

### Invisibility Mechanics
When a hero becomes invisible:
1. Remove the hero token from the board.
2. Place an **Invisibility Cloud** — a multi-tile token — over the hero's area.
3. The player **secretly** places their hero token beneath one tile of the cloud.
4. The cloud moves as a single unit. The player may silently rearrange which tile the hero is under when the cloud moves.
5. The cloud **cannot** be targeted by single-target attacks or abilities.
6. **AoE abilities** may target individual cloud tiles. If the tile containing the hero is hit, the hero is **revealed**.

**Attacking from Invisibility:**
When an invisible hero attacks or uses an offensive ability, the targeted hero **cannot use reactions** — the attack resolves without the defender being able to Flee, Dodge, or use Defensive Items. The invisible hero is then revealed immediately after the attack resolves.

### Breaking Invisibility
The hero is revealed when:
- They **Attack** or use a **revealing Ability**.
- A cloud tile enters a **Sentry Ward** or **Dust of Appearance** radius.
- An AoE ability hits the correct tile.

### Sentry Wards
A purchased consumable token placed by a hero in any area.

- Any Invisibility Cloud **entering** the ward's area is immediately revealed — the owning player must disclose the hero's tile.
- Sentry Wards remain active for a set number of rounds before expiring.

### Dust of Appearance
A consumable item. When used, creates a **Reveal radius** centred on the using hero for the current round. Functions identically to Sentry Wards but moves with the hero and is single-use.

### Observer Wards
A purchased consumable token placed by a hero on any Open hex.

- Observer Wards cover a fixed radius of hexes (typically 3–4 hexes, specified on the Item Card).
- **Tactical Advantage:** When an enemy hero standing in a warded area attacks or uses an ability on an allied hero, that allied hero (and any other allied heroes targeted during that same activation) may use **two reactions** instead of the normal one. This represents superior awareness and positioning intel.
- Observer Wards remain active for a set number of rounds before expiring.
- Observer Wards do **not** grant detection — they only provide the reaction advantage. Use Sentry Wards or Dust for invisibility detection.
- Observer Wards can be destroyed by enemy heroes who locate them (costs 1 AP while adjacent to the ward token).
- **Smoke of Deceit bypasses Observer Wards** — heroes under Smoke are invisible to wards and do not trigger the tactical advantage (see below).

### Smoke of Deceit
A consumable item purchased at the Fountain. When used, Smoke grants **Invisibility** to the using hero and all allied heroes within a fixed radius (typically 2 hexes, specified on the Item Card).

**Rules:**
- All affected heroes move together as a group under a single **Smoke Cloud** token (similar to Invisibility Clouds, but covering multiple heroes).
- **Activation Restriction:** The hero who activates Smoke **cannot attack or use offensive abilities for the remainder of that turn**. This prevents immediate exploitation of the Smoke buff.
- Heroes under Smoke are **invisible to Observer Wards** — they do not trigger the tactical reaction advantage when attacking from a warded area.
- **Attacking from Smoke:** When a hero under Smoke attacks or uses an offensive ability, the targeted hero **cannot use reactions** — the attack resolves without the defender being able to Flee, Dodge, or use Defensive Items. The Smoke dispels from the attacking hero immediately after the attack resolves.

**Smoke Dispels When:**
- Any affected hero moves within **3 hexes** of an enemy hero.
- Any affected hero enters a **Tower's area of control**.
- Any affected hero attacks or uses an offensive ability.

Once Smoke dispels, all affected heroes are immediately revealed and return to normal visibility. Smoke is a single-use consumable.

---

## 15. Items & the Shop

### Purchasing Items
Heroes buy Item Cards at the **Fountain** shop. A hero must be **physically at the Fountain** to purchase directly, or use the Courier for remote delivery.

### Item Cards
Items provide:
- **Passive stat bonuses** — added directly to the hero's Damage, Defense, Health, Mana, or Move Speed.
- **Active abilities** — cost AP and/or Mana when activated.
- **Consumable effects** — single-use items (e.g. Sentry Ward, Observer Ward, Dust, Smoke of Deceit).

### The Courier
A shared team token that delivers items from the Fountain stash to heroes in the field.

- Delivery takes **1–2 rounds** depending on distance to the target hero.
- The Courier can be killed by enemy heroes; any items being carried are **lost**.
- Each team has one Courier.

### Aghanim's Scepter
A high-cost luxury item purchased at the Fountain. When a hero acquires Aghanim's Scepter, one of their abilities receives a permanent upgrade.

**Rules:**
- Each hero has **one ability** that can be upgraded by Aghanim's Scepter. This is clearly marked on the Ability Card.
- The upgrade effect is **printed directly on the Ability Card** in a dedicated "Aghanim's Upgrade" section.
- The Scepter provides the upgrade immediately upon purchase — no additional activation required.
- Scepter upgrades are permanent as long as the item is held by the player.
- **Aghanim's Shard is not included in this board game.**

---

## 16. Respawn & Buyback

### Respawn
When a hero is killed they are removed from the board and placed in a respawn queue.

- **Respawn Timer:** A dead hero respawns after a number of **turns** equal to their **current level**. For example, a Level 8 hero waits 8 turns before respawning.
- Turns are counted individually across all players, not rounds. If killed during an opponent's turn, the timer begins counting with the next player's turn.
- On their designated respawn turn, the hero returns to the **Fountain** with full Health and Mana.
- Death timers scale automatically with level progression — higher-level heroes are out of the game longer when killed, making late-game deaths more punishing.

### Buyback
A dead hero may pay a **Gold fee** at any point during their respawn wait to return to the Fountain immediately.

- **Buyback Cost:** Scales with hero level. The exact gold cost is specified on reference cards or the game board.
- A hero who uses Buyback cannot Buyback again for a set number of rounds (typically 5 rounds).
- Buyback bypasses the respawn timer entirely — the hero returns to the Fountain at the start of their next turn.

---

## 17. Ability Types & Targeting

Ability Cards use different targeting and activation methods. This section defines how each type works in the board game context. All entries are pending design discussion.

### Activation Methods

**Passive** — Always active; no mana cost or activation required. Effect is continuous as long as the hero is alive.

**Active** — Manually cast during a hero's turn. Costs Mana and AP as printed on the card.

**Toggle** — Can only be **activated** during the hero's own turn (costs Mana and AP as printed). Once active, can be **toggled off at any time** — even during another player's turn — unless the hero is Silenced. While active, may drain Mana or Health per round. Examples: Rot, Mana Shield.

**Channeled** — Can be **activated** during the hero's own turn (costs Mana and AP as printed). Once active, the hero must remain stationary and the effect persists across subsequent turns until interrupted or cancelled. **Interrupted by:** Stun, Silence, forced movement, or the target moving out of range. The casting player may **cancel the channel at any time** (like a toggle). Examples: Freezing Field, Black Hole.

### Targeting Types

**No Target (Self-Cast)** — Instant effect centered on or affecting only the caster. No targeting step required. Examples: God's Strength, Battle Hunger.

**Unit Target (Single Target)** — Targets a specific unit (ally, enemy, creep, or structure) within range and LoS. Must declare target before resolving.

**Point Target** — Player declares a specific hex within range as the target location. The effect occurs at that hex. Whether the effect is instant or has travel time is specified on the Ability Card. Examples: Light Strike Array, Ice Path.

**Direction/Vector Target** — Player declares a direction or line from the caster by specifying a target hex. How the ability resolves along that direction (instant movement, projectile, persistent zone, etc.) is specified on the Ability Card. Examples: Swashbuckle (movement + attack along direction), Macropyre (line of fire).

### Effect Shapes

**Circular AoE** — Affects all units within a fixed radius (measured in hexes) from the center point.

**Linear/Line** — Straight line from caster extending outward. Hits all units along the path.

**Cone** — Wedge-shaped area in front of the caster. Hits all units in the cone.

**Global** — Affects all enemy or allied heroes (as specified on the card) on the entire board, regardless of range or Line of Sight. No targeting step required — all valid targets are affected simultaneously. Balance is handled through the ability's damage values, mana cost, cooldown, and other printed parameters. Examples: Thundergod's Wrath, Nature's Call.

### Special Mechanics

**Skillshot** — Abilities that travel in a line from the caster to a target location and can be dodged. **Whether an ability is a skillshot must be explicitly marked on the Ability Card.** Only abilities marked as Skillshot may be dodged using the Dodge Skillshot reaction — all other abilities resolve instantly and too quickly to dodge. The caster declares a direction by specifying a target hex (using Direction/Vector targeting). The ability creates a line effect from the caster's hex toward the target hex. Any hero in the path of the skillshot (including at the end position) may use the **Dodge Skillshot** reaction (see §3) to attempt to avoid being hit. The dodge reaction costs 2 AP from the hero's next turn, requires a die roll to determine success, and forces the hero to immediately move to an adjacent hex regardless of the roll's outcome. Examples: Sacred Arrow, Meat Hook.

**Ground-Targeted AoE** — Combination of Point Target + Circular AoE. Player picks a hex; all units within the radius are affected.

**Unit-Targeted AoE** — Targets a unit; effect radiates from that unit to nearby hexes. Examples: Poison Nova, Thundergod's Wrath (per-hero basis).

**Aura** — Passive effect that continuously radiates from the hero to all allied or enemy units (as specified on the card) within a fixed range measured in hexes. The aura's radius, which units are affected (allies/enemies/both), and the specific effect are all printed on the Ability Card. Auras are always active while the hero is alive and do not require activation. Examples: Precision Aura, Vampiric Aura.

---

## ── EXCLUDED MECHANICS ──

The following were considered and deliberately excluded to avoid bloat. Candidates for expansion or variant rules.

| Mechanic | Reason for Exclusion |
|---|---|
| **Talent Tree** | Per-hero card complexity; Ability unlocks at levels 6/12/18 cover progression. |
| **Bounty Runes** | Redundant with Passive Income in the Round End Phase. |
| **Glyph of Fortification** | Risks stalling siege turns; candidate for optional rule after playtesting. |
| **Neutral Item Drops** | Requires a separate tiered item pool; excessive component overhead. |
| **Day / Night Cycle** | Touches vision, hero stats, and towers simultaneously; high complexity for limited return. |
| **Hero Roles / Position Priority** | Left to player strategy; no mechanical enforcement needed. |
| **Comeback Gold** | Bookkeeping overhead; revisit as variant rule if snowballing proves a problem in playtesting. |
| **Aghanim's Shard** | Scepter provides sufficient ability upgrade depth; Shard would require separate upgrade tier and additional card complexity. |
| **Tormentor** | Reward (Aghanim's Shard) excluded in §F; no longer needed. |
