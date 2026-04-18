# DOTA 2: THE BOARD GAME — RULEBOOK

## Objective
Destroy the enemy team's Ancient, located within their base. To reach the Ancient, heroes must gain power, accumulate gold, and destroy defensive Towers in at least one lane.

---

## Game Components
- **Hero Cards** — Statistics for Attack, Defense, Health, Mana, and Move Speed.
- **Ability Cards** — Unique skills for each hero, unlocked and upgraded as the hero levels up.
- **The Board** — A map featuring three lanes (Top, Mid, Bottom), the River, the Jungle, and two Bases.
- **Tokens** — Representations for Creeps, Towers, Gold/XP, and Invisibility markers.
- **Action Point (AP) Trackers** — Tools to manage resources available each turn.

---

## Game Loop
The game is played in Rounds. Each Round consists of 20 turns — every hero activates twice.

### Picking Phase
A coin is flipped between the two teams. The winner chooses to either pick a hero first or play first; the loser gets the other option. Heroes are picked in alternating fashion by each team.

### Game Start
All heroes start with 3× the AP at the start of the game to get out onto the map. Creeps only spawn after the first round, so the only actions available during this time are movement and level 1 fights.

### Planning Phase
Before each half-round (10 turns), all players simultaneously:
1. Select Action Cards (Move, Attack, Farm, Use Ability, etc.) for each hero they control
2. Place cards face-down in front of them (one set per hero if controlling multiple)
3. Once all players are ready, the Turn Phase begins
4. Each hero's cards remain face-down until that hero's activation, when they are revealed and executed

### Turn Phase
Heroes execute their committed actions one at a time. Each hero activates twice per round (once per half-round). Heroes alternate between teams in a pendulum pattern to ensure fairness — if a player controls multiple heroes, those heroes do not all activate in succession.

### Round End Phase
After all heroes have completed both activations (20 turns total):
- **Creep Spawning** — New waves spawn at the Creep Meeting Point in each lane.
- **Passive Income** — All heroes receive a set amount of passive gold.
- **Neutral Respawns** — Every even-numbered round, neutral creeps in jungle camps are replenished.
- **Rune Spawns** — Every 4th round, a Power Rune spawns at one of the river positions.

---

## Action Points (AP) and Actions
Each hero has their own AP per turn to spend.

| Action | Description |
|--------|-------------|
| **Move** | Move a hero to an adjacent area. |
| **Attack** | Initiate combat with a Creep, Tower, or Enemy Hero. |
| **Farm** | Spend AP to gain gold and XP from a creep wave or neutral camp. |
| **Deny** | *(Reaction)* Use AP from your next turn to interrupt an opponent's Farm action. Requires a die roll challenge. |
| **Use Item** | Activate an item card's effect. |
| **Use Ability** | Activate a hero-specific ability card (requires Mana). |

---

## Map Areas

### Fountain
Located in the base. Instantly restores all Health and Mana to heroes in this area.

### Creep Meeting Points
Locations halfway between the closest standing towers in a lane. Lane creeps can only be farmed here. (Each possible location is marked on the map.)

When a tower is destroyed, the meeting point in that lane shifts forward (toward the enemy base) during the Round End Phase when new creeps spawn. This causes the next wave to appear at the advanced position, creating immediate lane pressure.

### Neutrals and Ancients
Jungle areas that provide XP and Gold at the cost of Health. Ancient camps require extra AP and cost more health.

### Roshan's Pit
Home to Roshan. Defeating him drops the **Aegis of the Immortal**. If both teams are present at his death, a die roll determines who claims the item.

### Runes
Two rune spawn points sit on opposite sides of the river. Every 4th round, any player simultaneously rolls the **custom Rune Die** (determines rune type) and flips a **coin** (determines which side spawns it). Both results are resolved together and immediately visible to both teams. Rune types:

| Rune | Effect |
|------|--------|
| **Illusion** | Creates 3 lesser clone tokens that attack for reduced damage and take increased damage from all sources. |
| **Haste** | Doubles the effectiveness of movement actions. |
| **Invisibility** | Provides the hero with an invisibility cloud. |
| **Regeneration** | Restores all health and mana; can be interrupted by an enemy attack, reducing its effectiveness. |
| **Double Damage** | Doubles damage on attacks. |

---

## Towers and Siege

- **Progression** — Towers must be destroyed in sequence: Tier 1 → Tier 2 → Tier 3 → Tier 4 → Ancient.
- **Siege Rules** — A Tower can only be attacked if the enemy creep wave in that lane has been exhausted for the round.
- **Health Cost** — Attacking a tower incurs a Health penalty to the hero, reduced based on the number of allied creeps present.

---

## Terrain and Structures

Hexes on the board have different properties that affect movement and line of sight:

| Type | Movement | Line of Sight | Notes |
|------|----------|---------------|-------|
| **Open** | Passable | Clear | No restrictions. |
| **Tree** | Blocked | Blocked | Cannot enter; blocks LoS; can be destroyed by abilities/items. Regrows every 4th round. |
| **Impassable** | Blocked | Blocked | Permanent walls, cliffs, water. Cannot enter or see through. |
| **Building** | Blocked | **Clear** | Cannot enter; does **not** block LoS. Destroyable — becomes Open when destroyed. |
| **Obstacle** | Blocked | **Clear** | Cannot enter; does **not** block LoS. Permanent — cannot be destroyed. |

Buildings and Obstacles allow heroes to see (and target) enemies on the other side, but physically block the path — heroes must go around them.

---

## Combat and Hero Fights

- **Initiative** — When multiple heroes are in the same area, action order is determined by Move Speed.
- **Resolution** — `Damage − Defense = Health Lost`
- **Crowd Control (CC)** — Stuns remove AP from the target's next turn. Silences prevent the use of Ability Cards for one round.
- **Range** — Melee heroes must be in the same area to attack. Ranged heroes can attack from an adjacent area.

---

## Vision and Invisibility

- **Visibility** — All units are visible unless they have the Invisibility status.
- **Invisibility Mechanics** — Replace the hero with an invisibility cloud. The cloud covers multiple tiles with a compartment in each; the player decides under which tile their hero token sits. The entire cloud moves as the player wishes. Individual tiles may be targeted with AOE abilities (not single-target). If an AOE ability hits, the hero is revealed. Attacking or using an ability also reveals the hero, unless specified otherwise.
- **Sentry Wards and Dust** — Items that provide a passive Reveal radius. Any cloud token entering this radius must be replaced with the hero token in the correct position.

---

## Economy and Progression

- **The Courier** — A shared unit that delivers items from the Fountain to heroes. Delivery typically takes 1–2 rounds.
- **Leveling** — Heroes gain levels via XP. At levels 6, 12, and 18, heroes unlock or upgrade their Ability cards.
- **Buybacks** — Dead heroes can spend a significant Gold fee to respawn immediately at the Fountain.