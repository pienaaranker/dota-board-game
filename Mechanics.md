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
Teams alternate sides taking hero turns. Each side activates their heroes one at a time, spending AP until all AP is used or the player passes.

- Turn order within a round: **Dire → Radiant → Dire → Radiant …** until all heroes on both sides have acted.
- A player may pass their remaining AP at any time, ending that hero's turn early.
- AP does not carry over between rounds.

### Reactions
When an active hero targets your hero with an attack or ability, you may **React** before the effect resolves. Reactions interrupt the active hero's turn, are resolved immediately, and then the active hero continues.

**Rules:**
- A hero may only **react once** per opposing hero's turn (not once per round — once per activation).
- Reactions are **always paid from the reacting hero's next turn AP**. The cost is deducted at the start of that hero's next turn — they simply have that many fewer AP to spend.
- Only the **targeted hero** may react, not teammates.

**Reaction Types:**

| Reaction | AP Cost (from next turn) | Effect |
|---|---|---|
| **Flee** | 2 AP | Move 1 hex in any direction before the attack or ability resolves. If the attacker required adjacency or LoS, the attack misses entirely. |
| **Activate Defensive Item** | 1 AP | Immediately trigger a held defensive Item Card (e.g. BKB equivalent) before damage is applied. The item's effect takes place before resolution. |
| **Deny** | 1 AP | Contest an allied creep's last hit to deny the enemy gold and XP. See §8 for full rules. |

> **Example:** Juggernaut (4 AP) attacks Crystal Maiden. She reacts with **Flee** (costs 2 AP from her next turn), moving 1 hex away. Juggernaut is melee — he no longer has adjacency — so the attack misses. On Crystal Maiden's next turn she has 2 fewer AP to spend.

### Round End Phase
After all heroes on both sides have completed their turns, the following occur in order:

1. **Creep Spawning** — A new creep wave appears at the Creep Meeting Point in each lane (skipped during Round 1).
2. **Passive Income** — Every hero receives a fixed amount of gold regardless of activity.
3. **Power Rune Spawn** — On every 4th round, a Power Rune spawns at the River rune location (see §11).
4. **Neutral Respawns** — On every even-numbered round, all cleared jungle camps are replenished.

---

## 4. The Board

The board represents the battlefield, divided into named areas. Heroes, creeps, and tokens occupy these areas.

### Hex Grid & Terrain
The entire map is built on a **hex grid**. Every hex is one of three terrain types:

| Terrain Type | Movement | Line of Sight | Notes |
|---|---|---|---|
| **Open** | Passable | Clear | Default hex — no restrictions. |
| **Tree** | **Blocked** | **Blocked** | Impassable unless an ability says otherwise; blocks LoS; can be destroyed. |
| **Impassable** | **Blocked** | **Blocked** | Permanent walls, cliffs, and water. Cannot be entered or seen through under any circumstances. |

The key difference between **Tree** and **Impassable**: trees can be destroyed and converted to Open hexes; impassable terrain is permanent.

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

### Initiative
When combat occurs in an area with multiple heroes, action order is resolved by **Move Speed** (printed on the Hero Card). Ties are broken by the active player's choice.

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

### Death
When a hero's Health reaches 0 they are removed from the board and enter a respawn countdown (see §15).

---

## 8. Farming & Economy

### Farm Action
A hero in the same area as a creep wave or neutral camp spends 1 AP to **Farm**. Successful farming awards **gold and XP**.

### Last Hit & Gold Source 🔄 Pending Discussion
In Dota 2, only the hero landing the killing blow earns gold. How this is adjudicated in the Farm action — whether a die roll is required and how the Deny mechanic integrates — is pending discussion. See §A.

### Passive Income
Every hero receives a flat gold amount at the **Round End Phase**, regardless of farming activity.

### Deny
Deny is a **Reaction** (see §3) costing **1 AP from the reacting hero's next turn**. An opposing hero may react to a friendly Farm action to attempt to contest the last hit on an allied creep, depriving the enemy of gold and XP.

- Resolved with a **die roll challenge** between the denying hero and the farming hero.
- **Deny succeeds:** The farming hero gains no gold or XP from that unit.
- **Deny fails:** Farm proceeds normally.

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

- The Meeting Point shifts **toward the enemy** whenever a tower on that side is destroyed.
- Lane creeps may only be Farmed at the Meeting Point.
- A creep wave persists until Farmed or replaced by the next wave.

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

A Power Rune spawns at the **River rune position** every **4th round**. Runes cycle in a fixed, predictable order — both teams can anticipate the next rune.

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
- **Smoke of Deceit** (pending — see §E).

### Invisibility Mechanics
When a hero becomes invisible:
1. Remove the hero token from the board.
2. Place an **Invisibility Cloud** — a multi-tile token — over the hero's area.
3. The player **secretly** places their hero token beneath one tile of the cloud.
4. The cloud moves as a single unit. The player may silently rearrange which tile the hero is under when the cloud moves.
5. The cloud **cannot** be targeted by single-target attacks or abilities.
6. **AoE abilities** may target individual cloud tiles. If the tile containing the hero is hit, the hero is **revealed**.

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

### Observer Wards 🔄 Pending Discussion
A ward type for persistent general vision of a board area (not detection). Pending discussion. See §D.

---

## 15. Items & the Shop

### Purchasing Items
Heroes buy Item Cards at the **Fountain** shop. A hero must be **physically at the Fountain** to purchase directly, or use the Courier for remote delivery.

### Item Cards
Items provide:
- **Passive stat bonuses** — added directly to the hero's Damage, Defense, Health, Mana, or Move Speed.
- **Active abilities** — cost AP and/or Mana when activated.
- **Consumable effects** — single-use items (e.g. Sentry Ward, Dust, Smoke of Deceit).

### The Courier
A shared team token that delivers items from the Fountain stash to heroes in the field.

- Delivery takes **1–2 rounds** depending on distance to the target hero.
- The Courier can be killed by enemy heroes; any items being carried are **lost**.
- Each team has one Courier.

### Aghanim's Scepter & Aghanim's Shard 🔄 Pending Discussion
Special items that modify hero abilities in unique, hero-specific ways. Pending discussion. See §F.

---

## 16. Respawn & Buyback

### Respawn
When a hero is killed they are removed from the board and placed in a respawn queue.

- Respawn takes a number of rounds that increases as the game progresses — deaths are more punishing late game.
- The specific round-count table is **pending discussion** (see §G).
- On their designated respawn round, the hero returns to the **Fountain** with full Health and Mana.

### Buyback
A dead hero may pay a **Gold fee** at any point during their respawn wait to return to the Fountain immediately.

- Buyback cost scales upward as the game progresses.
- A hero who uses Buyback cannot Buyback again for a set number of rounds.

---

## ── PENDING DISCUSSIONS ──

The following mechanics are confirmed for inclusion but need specific rulings before the design is final. Discuss one at a time.

### §A — Last Hit & the Farm Action
The Farm action awards gold and XP, but the exact requirement — whether a die roll or challenge must be passed to "earn" the last hit, and how Deny integrates — needs a ruling.

### §B — Ban Phase in Draft ✅ Resolved
**All Pick** is the default mode and includes a ban phase: 3 bans per team, alternating, starting with the team that lost the coin flip. Two additional modes — **Single Draft** and **All Random** — are included as variants. See §2 for full rules.

### §C — High Ground Advantage ❌ Not Included
**Decision:** Excluded. A miss-chance mechanic risks making late-game defence too strong and could stall games. Not included for now; may be revisited if playtesting shows pushes are too easy.

### §D — Observer Wards
Wards providing persistent vision of a board zone — flagging enemy movement without grant of detection. Ruling needed on how "vision" is mechanically useful on the board, ward duration, placement limits, and interaction with Smoke of Deceit.

### §E — Smoke of Deceit
A consumable that covers a group of allied heroes in Invisibility for coordinated movement. Ruling needed on how many heroes can share one Smoke, what breaks the effect (entering a tower zone? enemy detection range?), and number of charges.

### §F — Aghanim's Scepter & Aghanim's Shard
Two items that upgrade hero abilities in hero-specific ways rather than giving generic stat bonuses. Ruling needed on card format (attached upgrade card vs. overlay vs. printed secondary box on Ability Card), and handling of Scepters that grant entirely new abilities.

### §G — Respawn Timer Scaling
Deaths should cost more rounds as the game progresses. Ruling needed on a specific table (e.g. Early / Mid / Late game thresholds and their corresponding round costs) and how Buyback cost scales alongside it.

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
| **Tormentor** | Reward (Aghanim's Shard) is pending §F; revisit if §F is resolved. |
