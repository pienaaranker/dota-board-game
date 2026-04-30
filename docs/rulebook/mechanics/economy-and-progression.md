# DOTA 2: THE BOARD GAME — ECONOMY AND PROGRESSION

This document collects gold, farming, leveling, items, and death-cycle rules.

---

## Creep Kills & Economy

### Attacking Creeps And Camps
A hero in the same area as a lane creep wave or neutral camp spends AP on a normal **Attack** action targeting a specific creep or camp token.

Lane creeps use the shared **Hit** system from [creeps-towers-and-objectives.md](creeps-towers-and-objectives.md), not numeric HP.

- **Normal Lane Creeps:** Each creep killed gives the killing hero **5 gold**. Each killed creep also gives exactly **2 shared XP** to allied heroes within **4 hexes** of that creep.
- **XP Split:** If 2 allied heroes are in XP range, each gains **1 XP**. If only 1 allied hero is in XP range, that hero gains the full **2 XP**. If more than 2 allied heroes are in XP range, only the **2 closest** allied heroes gain **1 XP** each.
- **XP Ties:** If multiple allied heroes are tied for the final eligible XP position, the creep-killing team chooses which tied hero receives that XP.
- **Super Creeps:** Each creep killed gives the killing hero **3 gold** and gives **1 XP** to the **closest** allied hero within **4 hexes**.
- **Mega Creeps:** Each creep killed gives the killing hero **3 gold** and gives **1 XP** to the **closest** allied hero within **4 hexes**. Whenever a hero uses a basic **Attack** action against one or more Mega Creeps, that hero takes **5 damage** in retaliation. If that basic attack hits multiple Mega Creeps at once, that retaliation still applies only **once** for that attack.
- **Neutral/Ancient Camps:** Remove 1 creep counter from the camp. The hero receives the camp's normal gold and XP but also loses **Health** (neutrals fight back).
- **If Denied:** An enemy hero may use a committed **Attack** reaction (see Deny below) only when the current **Attack** would remove the target lane creep's **last remaining Hit**. If the Deny succeeds, the attacking hero receives **no gold**, and only the **closest** eligible hero on the attacking team within **4 hexes** of the denied creep gains **1 XP**.

There is **no separate Farm action**. Heroes must target and attack creeps directly to kill them.

### Passive Income
Every hero receives a flat gold amount at the **Round End Phase**, regardless of farming activity.

### Deny
There is no dedicated Deny token. To attempt a deny, a hero commits an **Attack** token into a **reaction slot** during Planning Phase, reserving 1 AP. When an enemy declares an **Attack** that would remove an allied lane creep's last remaining Hit, that hero may trigger their Attack reaction against the same creep token — racing the enemy to land the killing blow first.

- Deny may only be attempted when the triggering **Attack** would remove the target creep's **last remaining Hit**.
- Both the attacker and the denying hero are targeting the same creep simultaneously. Resolve with a **die roll challenge** — the higher roll lands the kill.
- **Deny succeeds (denier wins roll):** The denying hero kills the creep. The attacking hero gains **no gold**. Only the **closest** eligible hero on the attacking team within **4 hexes** of the denied creep gains **1 XP**.
- **Deny fails (attacker wins roll):** The enemy's Attack resolves normally — they receive that creep's normal gold and XP reward.

### Gold Uses
Gold is spent to:
- Purchase **Item Cards** at the Fountain shop.
- Pay the **Buyback** fee to respawn immediately.

---

## XP & Leveling

### Earning XP
Heroes gain XP whenever a unit dies within **4 hexes** of them:
- **Lane creeps** — All allied heroes within 4 hexes of the killed creep gain XP (split among eligible heroes).
- **Enemy heroes** — **XP = 5 + killed hero's level**, split equally among all allied heroes within 4 hexes. The closest hero receives any remainder.
- **Neutral/Ancient creeps** — Only heroes who attacked the camp gain XP (printed on the camp).

### Leveling Up
Level is derived directly from XP: **Level = XP ÷ 10** (rounded down). Track only XP — no separate level counter is needed.

**Ability unlocking:**
- Level 1: Hero starts with one basic ability unlocked.
- Levels 2–4: Each level unlocks one additional basic ability (the player chooses which to unlock).
- Level 5: Stats only — no ability unlock.
- Level 6: The hero's ultimate unlocks. All basic abilities and the ultimate upgrade to their level 6–11 values.

**Milestone upgrades:**

| XP | Level | Effect |
|---|---|---|
| **60** | **6** | Ultimate unlocked. All abilities upgrade to the 6–11 bracket. |
| **120** | **12** | All abilities upgrade to the 12–17 bracket. |
| **180** | **18** | All abilities upgrade to their final values (18+ bracket). |

Every 10 XP earned grants the hero's per-level stat increases as printed on the Hero Card, applied immediately upon reaching that XP total. Ability values between milestones use the values of the most recently unlocked bracket.

---

## Items & the Shop

### Purchasing Items
Heroes buy Item Cards at the **Fountain** shop. A hero must be **physically at the Fountain** to purchase directly, or use the Courier for remote delivery.

### Item Cards
Items provide:
- **Passive stat bonuses** — added directly to the hero's Damage, Defense, Health, Mana, or Move Speed.
- **Active abilities** — cost AP and/or Mana when activated.
- **Consumable effects** — single-use items (e.g. Sentry Ward, Observer Ward, Dust, Smoke of Deceit).

### Inventory, Active Slots, And Backpack
- Each hero has **6 active item slots** and **3 backpack slots**.
- Only items in the **6 active item slots** may be activated, committed with numbered item-slot planning tokens, or provide passive bonuses.
- Items in the **backpack** are carried for storage only. They cannot be activated directly from the backpack and provide no passive bonuses while stored there.
- During the hero's own activation, that hero may swap items between active slots and backpack slots.
- Any item moved from the backpack into an active slot becomes usable only in the **next round**. Until then, it cannot be activated, committed with an item-slot token, or provide passive bonuses.

### The Courier
A shared team token that delivers items from the Fountain stash to heroes in the field.

- Delivery takes **1–2 rounds** depending on distance to the target hero.
- The Courier can be killed by enemy heroes; any items being carried are **lost**.
- Each team has one Courier.

### Aghanim's Scepter
A high-cost luxury item purchased at the Fountain. When a hero acquires Aghanim's Scepter, one of their abilities receives a permanent upgrade.

**Rules:**
- Each hero has **one ability** that can be upgraded by Aghanim's Scepter. This is clearly marked on the hero's Abilities Card.
- The upgrade effect is **printed directly on the Abilities Card** in a dedicated "Aghanim's Upgrade" section.
- The Scepter provides the upgrade immediately upon purchase — no additional activation required.
- Scepter upgrades are permanent as long as the item is held by the player.
- **Aghanim's Shard is not included in this board game.**

---

## Respawn & Buyback

### Respawn
When a hero is killed they are removed from the board and placed in a respawn queue.

- **Respawn Timer:** A dead hero respawns after a number of **turns** equal to their **current level**. For example, a Level 8 hero waits 8 turns before respawning.
- **Clarification:** "Turns" are counted across all players — not just the dead hero's own activations. If there are 6 players and a Level 8 hero dies, they will respawn after 8 total player turns have passed (which could be less than one complete round).
- Turns are counted individually as each hero activates during the Turn Phase. If killed during an opponent's turn, the timer begins counting with the next player's turn.
- On their designated respawn turn, the hero returns to the **Fountain** with full Health and Mana at the start of that turn (before committing planning tokens).
- Death timers scale automatically with level progression — higher-level heroes are out of the game longer when killed, making late-game deaths more punishing.

### Buyback
A dead hero may pay a **Gold fee** at any point during their respawn wait to return to the Fountain immediately.

- **Buyback Cost:** Scales with hero level. The exact gold cost is specified on reference cards or the game board.
- A hero who uses Buyback cannot Buyback again for a set number of rounds (typically 5 rounds).
- Each hero has a dedicated **Buyback token**. While Buyback is available, that token remains in the hero's ready area. When Buyback is used, place the token in the hero board's **round cooldown track** at the appropriate value and advance it toward 0 at each Round End. Buyback becomes available again when the token returns to the ready area.
- Buyback bypasses the respawn timer entirely — the hero returns to the Fountain at the start of their next scheduled activation (during the Planning Phase for that half-round).
- If a hero buybacks during the first half of a round and hasn't activated yet that half, they return immediately and can participate in Planning Phase. If they've already activated that half, they return for the second half Planning Phase.