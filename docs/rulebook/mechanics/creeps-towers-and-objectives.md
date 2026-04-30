# DOTA 2: THE BOARD GAME — CREEPS, TOWERS, AND OBJECTIVES

This document collects lane-state, siege-state, and major map-objective rules.

---

## Creeps

### Lane Creeps
Creep waves spawn at the Round End Phase from each team's base and meet at the **Creep Meeting Point** — the midpoint between the two nearest standing towers on opposite sides of a lane.

- The Meeting Point shifts **toward the enemy during Round End Phase** when a tower on that side has been destroyed. The shift takes effect when the new creep wave spawns, causing creeps to appear at the advanced position and creating immediate lane pressure.
- Each lane's meeting point has **3 creep positions per team**: **2 melee positions** in front and **1 ranged position** behind them.
- Each team's wave in a lane therefore consists of **2 melee tokens** and **1 ranged token**.
- Each **melee token** is double-sided: one side shows **2 melee creeps**, the other shows **1 melee creep**. When one melee creep from that token is killed, flip the token to its 1-creep side. When the last melee creep on that token is killed, remove the token.
- Each **ranged token** represents **1 ranged creep**. Remove it when that ranged creep is killed.
- Heroes attack lane creeps directly using normal **Attack** actions. There is **no separate Farm action**.
- A creep wave persists until all 3 tokens for that team have been removed or the next wave replaces it.
- Each lane's meeting point hexes are pre-marked on the board with visual indicators.

### Lane Creep Hits
Lane creeps do **not** track numeric HP or Defense. They use a low-bookkeeping **Hit** system instead.

- **Normal Creeps:** Each creep has **1 Hit**.
- **Super Creeps:** Each creep has **2 Hits**.
- **Mega Creeps:** Each creep has **2 Hits**.
- A successful basic **Attack** action or a damaging ability removes **1 Hit** from each lane creep it affects, unless that card explicitly says otherwise.
- AoE and cleave effects remove **1 Hit** from each affected creep separately.
- Resolve Hits within a token **one creep at a time**. Do not spread partial damage across multiple creeps in the same token before one of them dies.
- If a Super or Mega creep on a token has lost **1 Hit** but is still alive, place a **Creep Damage Marker** on that token. Remove that marker when the damaged creep dies.
- A lane creep token can have only **1 Creep Damage Marker** at a time.

### Lane Creep States
Lane creep strength scales based on how many enemy Barracks have been destroyed. When a team's Barracks falls, the **opposing team's** creeps in that lane become stronger.

| State | Trigger | Effect |
|---|---|---|
| **Normal** | Barracks standing | Base wave uses the standard 2 melee + 1 ranged token formation. |
| **Super Creeps** | That lane's Barracks has been destroyed | That lane keeps the same token formation, but its creeps use the stronger Super Creep profile. Each Super Creep kill gives **3 gold** to the killer and **1 XP** to the closest allied hero within **4 hexes**. |
| **Mega Creeps** | All 3 Barracks destroyed | All lanes keep the same token formation, but their creeps use the stronger Mega Creep profile. Each Mega Creep kill gives **3 gold** to the killer and **1 XP** to the closest allied hero within **4 hexes**. Whenever a hero uses a basic **Attack** action against one or more Mega Creeps, that hero takes **5 damage** in retaliation. If that basic attack hits multiple Mega Creeps at once, that retaliation still applies only **once** for that attack. |

- Super and Mega creep states apply **per lane** until all 3 Barracks fall, at which point Mega Creeps replace Super Creeps everywhere.
- Passive Income is unaffected by creep state.
- Barracks cannot be rebuilt once destroyed.

### Neutral Camps
Located in the Jungle. Contain neutral creeps that belong to neither team.

- A hero attacks a Neutral Camp by spending AP on normal **Attack** actions while in the camp's area.
- Attacking neutral creeps costs the hero **Health** (the neutrals fight back).
- Neutral Camps do **not** require a lane creep wave to be exhausted first.
- Camps respawn on every **even-numbered round** if cleared.

### Ancient Camps
Stronger neutral camps found deep in the Jungle.

- Require **more successful attacks** to clear and deal **more Health damage**.
- Award commensurately higher gold and XP.

---

## Towers & Siege

### Tower Tier Progression
Structures must be destroyed in the following order per lane:

> **Tier 1 → Tier 2 → Tier 3 → Barracks / Tier 4 Towers → Ancient**

- A higher-tier tower cannot be attacked until all lower-tier towers in that lane are destroyed.
- Once the Tier 3 Tower in a lane falls, heroes gain access to the **base interior** for that lane. Both the **Barracks** for that lane and the **Tier 4 Towers** may then be sieged.
- Destroying a tower awards gold to every allied hero: **Tier 1 — 30g, Tier 2 — 50g, Tier 3 — 75g, Tier 4 — 100g**.
- Towers use the **Hits** system: each successful Attack removes 1 Hit. **Tier 1 = 10 Hits, Tier 2 = 15 Hits, Tier 3 = 18 Hits, Tier 4 = 20 Hits**.
- The **Ancient** cannot be attacked until both Tier 4 Towers are destroyed. The Ancient has **30 Hits**.

### Barracks
Each team has three Barracks buildings, one per lane, located in the base interior behind the Tier 3 Tower.

- Barracks use the same **Siege Requirement** as towers: the allied creep wave in that lane must be exhausted before heroes can attack.
- Barracks have **15 Hits** and do **not** deal retaliation damage to attackers.
- Each Barracks is represented by a removable **standing Barracks token** on its hex. When a Barracks is destroyed, remove that token. The printed board art beneath shows the broken Barracks state.
- When a Barracks is destroyed, the opposing team's creeps immediately become **Super Creeps** in that lane (see Creeps).
- If all 3 Barracks fall, the lane-state tracker for that team shifts to **Mega Creeps** globally. No separate Mega Creeps token is required.
- Destroying a Barracks awards **50 gold** to all heroes on the attacking team.

### Siege Requirement
A Tower may only be attacked if the **enemy creep wave in that lane has been exhausted** for the current round. Creeps must be cleared before heroes can deal damage to a tower.

### Tower Retaliation Damage
When a hero attacks a tower, the tower deals **5 damage** to the attacker (reduced by the number of allied lane creeps present in the area — creep bodies absorb tower aggro).

---

## Roshan

Roshan occupies **Roshan's Pit**, a fixed area on the board.

- Any hero or team may attack Roshan. He is treated as a very powerful neutral camp — he deals significant Health damage to attackers.
- Upon death, Roshan drops the **Aegis of the Immortal** and awards **50 gold** and **10 XP** to every allied hero.
- If heroes from **both teams** are present when Roshan dies, a **die roll** determines which team claims the rewards.
- Roshan **respawns** after a fixed number of rounds.
- Roshan HP is tracked on the printed Roshan track, not with a separate Roshan HP token.

### Aegis of the Immortal
- The holding hero **revives in place** upon death with full Health and Mana, consuming the Aegis.
- Aegis revival bypasses the normal respawn timer and Buyback cost.