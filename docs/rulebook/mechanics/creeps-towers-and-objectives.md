# DOTA 2: THE BOARD GAME — CREEPS, TOWERS, AND OBJECTIVES

This document collects lane-state, siege-state, and major map-objective rules.

---

## Creeps

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

## Towers & Siege

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
- Each Barracks is represented by a removable **standing Barracks token** on its hex. When a Barracks is destroyed, remove that token. The printed board art beneath shows the broken Barracks state.
- When a Barracks is destroyed, the opposing team's creeps immediately become **Enhanced** in that lane (see Creeps).
- If all 3 Barracks fall, the lane-state tracker for that team shifts to **Mega Creeps** globally. No separate Mega Creeps token is required.
- Destroying a Barracks awards a **gold bonus** to all heroes on the attacking team.

### Siege Requirement
A Tower may only be attacked if the **enemy creep wave in that lane has been exhausted** for the current round. Creeps must be cleared before heroes can deal damage to a tower.

### Tower Attack Damage
When a hero attacks a tower, the tower deals a **Health penalty** back to the attacker. This penalty is **reduced** (or nullified) by the number of allied lane creeps present in the area — creep bodies absorb tower aggro.

---

## Roshan

Roshan occupies **Roshan's Pit**, a fixed area on the board.

- Any hero or team may attack Roshan. He is treated as a very powerful neutral camp — he deals significant Health damage to attackers.
- Upon death, Roshan drops the **Aegis of the Immortal**.
- If heroes from **both teams** are present when Roshan dies, a **die roll** determines which team claims the Aegis.
- Roshan **respawns** after a fixed number of rounds.
- Roshan HP is tracked on the printed Roshan track, not with a separate Roshan HP token.

### Aegis of the Immortal
- The holding hero **revives in place** upon death with full Health and Mana, consuming the Aegis.
- Aegis revival bypasses the normal respawn timer and Buyback cost.