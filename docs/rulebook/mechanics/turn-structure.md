# DOTA 2: THE BOARD GAME — TURN STRUCTURE

This document collects the rules for objective, setup, drafting, and the round-to-round flow of play.

---

## Objective

Destroy the enemy team's **Ancient**, located inside their base. To reach the Ancient, a team must destroy all Towers in at least one lane in sequence. The first team to destroy the enemy Ancient wins.

---

## Game Setup & Draft

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

## Game Loop

The game is played in **Rounds**. Each Round consists of **20 turns** — all heroes activate twice using pendulum rotation. Each Round has three phases: Planning, Turn Phase, and Round End Phase.

**Terminology:**
- **Turn** — One hero's activation, during which they execute their committed actions.
- **Round** — 20 turns total. Each hero activates twice (once in each half-round of 10 turns).
- **Activation** — When a specific hero executes their committed planning tokens during their turn.
- **Duration:** When an ability or buff specifies a duration, it can be measured in:
  - **Rounds** — Lasts until the end of X complete rounds (all 20 turns).
  - **Turns** — Lasts for X total player turns (counted across all players).
  - The hero's Abilities Card or the relevant item entry will specify which measurement is used.

### Planning Phase
Before the Turn Phase begins, all players simultaneously select their actions for the upcoming half-round (10 turns):

1. Each player selects **Planning Tokens** for each hero they control, representing the actions that hero will take during their next activation.
2. Players place these tokens **face-down** in front of them (one set per hero if controlling multiple heroes).
3. Once all players have committed their planning tokens and are ready, the Turn Phase begins.
4. Planning tokens remain **face-down** until that specific hero's activation, at which point the player reveals their committed actions.
5. After the first 10 turns complete, players repeat the Planning Phase for the second half of the round.

**Planning Rules:**
- Planning Tokens include: Move, Attack, Farm, Use Item, Pass, and hero-specific ability tokens.
- Players may select up to their hero's AP worth of actions.
- Tokens remain hidden until activation — players commit actions without knowing what enemies have planned.
- Once a hero's tokens are revealed at the start of their activation, actions are locked in and must be executed in the order committed unless prevented by crowd control, reactions, or game state changes.
- Reactions are **not** included in Planning Phase — reactions are declared in real-time during the Turn Phase when triggered.

**Strategic Implications:**
- Players must predict enemy positions and actions when committing their tokens.
- Targeted actions (Attack specific hero, single-target abilities) carry risk if targets move or die before your activation.
- Revealing your actions only when you activate prevents enemies from adjusting their later-activating heroes' targets based on your plans.
- Earlier heroes in turn order have more uncertainty but also more flexibility in responding to the actual game state.

### Turn Phase
Heroes activate one at a time within a round, executing their committed actions. Each hero spends all their AP before the next hero activates.

**Turn Order — Pendulum Rotation:**
The **Round Start Token** determines which hero goes first each round. The token follows a **circular rotation** — it moves to the next hero in the alternating sequence at the start of each new round, wrapping around after the last hero.

Once the starting hero is determined, heroes activate in **alternating team order** (one Radiant hero, then one Dire hero, then one Radiant hero, etc.). The direction (forward or backward through the hero sequence) alternates every 10 turns, creating a "pendulum" pattern within the round.

**Important:** Turn order alternates by **hero**, not by player. If a player controls multiple heroes, those heroes are interspersed with enemy heroes in the rotation — a player does not activate all their heroes in succession.

**Example with 10 heroes (5v5):**
- Team Radiant: Hero A, Hero B, Hero C, Hero D, Hero E
- Team Dire: Hero V, Hero W, Hero X, Hero Y, Hero Z
- Rotation sequence: A → V → B → W → C → X → D → Y → E → Z (alternating teams)

**Round 1 (20 turns total):**
- Round Start Token is on Hero A.
- **Turns 1-10 (First Half):** Play proceeds forward (e.g., Hero A → Hero V → Hero B → Hero W → Hero C → Hero X → Hero D → Hero Y → Hero E → Hero Z).
- **Turns 11-20 (Second Half):** Play proceeds backward (e.g., Hero Z → Hero E → Hero Y → Hero D → Hero X → Hero C → Hero W → Hero B → Hero V → Hero A).

**Round 2 (20 turns total):**
- Round Start Token moves to next hero in circular sequence (Hero V).
- **Turns 1-10 (First Half):** Play proceeds forward (e.g., Hero V → Hero B → Hero W → Hero C → Hero X → Hero D → Hero Y → Hero E → Hero Z → Hero A, wrapping around).
- **Turns 11-20 (Second Half):** Play proceeds backward (e.g., Hero A → Hero Z → Hero E → Hero Y → Hero D → Hero X → Hero C → Hero W → Hero B → Hero V).

**Round 3 (20 turns total):**
- Round Start Token moves to next hero in circular sequence (Hero B).
- **Turns 1-10 (First Half):** Play proceeds forward from Hero B.
- **Turns 11-20 (Second Half):** Play proceeds backward.

**Round 4 (20 turns total):**
- Round Start Token moves to next hero in circular sequence (Hero W).
- Pattern continues with the token cycling through: A → V → B → W → C → X → D → Y → E → Z → A (circular).

This ensures positional fairness over time — no hero is always first or always last.

**General Rules:**
- Each hero activates twice per round (once in each half).
- A player may commit fewer actions than their total AP allows, effectively passing early.
- AP does not carry over between activations or rounds.
- Committed actions must be attempted in order, but may fail or be prevented by game state (e.g., target no longer valid, hero stunned).

### Failed Actions
When a committed action cannot be executed, the following rules apply:

**Example Action Failure Causes:**
- **Invalid Target** — The target unit has moved, died, or is no longer in range/LoS.
- **Stunned Hero** — Hero has AP reduced below the cost of the action due to stun effects.
- **Silenced Hero** — Hero cannot use abilities while Silenced.
- **Insufficient Resources** — Hero lacks the Mana to cast a committed ability.
- **Movement Blocked** — The destination hex is occupied or impassable due to game state changes.

**Resolution:**
When a committed action is revealed during a hero's activation, the player declares the specific target or destination at that moment. If the action cannot be executed as originally intended, the player has two options:

1. **Cancel the action** — The token is returned to the hero's available token pool and can be committed again in a future activation. No AP is spent. The activation proceeds to the next committed action.
2. **Retarget the action** — If a valid alternative target or destination exists, the player may choose to execute the action on that alternative instead. The action executes normally and AP is spent as usual.

**Target Declaration Timing:**
- Specific targets (which enemy hero to attack, which hex to move to, which unit to cast an ability on) are **not** committed during Planning Phase.
- Only the **type** of action is committed (Move, Attack, Storm Hammer, etc.).
- The specific target or destination is declared when the token is revealed during execution.
- This gives players flexibility to adapt to game state changes, but commits them to the action type itself.

**When Retargeting is Not Possible:**
Some actions cannot be retargeted because no valid alternative exists:

- **Stunned Hero** — Hero has AP reduced below the cost of the action due to stun effects. Action cannot execute at all.
- **Silenced Hero** — Hero cannot use abilities while Silenced. Ability actions cannot execute at all.
- **Insufficient Resources** — Hero lacks the Mana to cast a committed ability. Action cannot execute at all.
- **No Valid Targets** — All potential targets are out of range, dead, or otherwise invalid. Action cannot execute.

In these cases, the action is automatically cancelled (returned to the hero's available token pool, no AP spent).

**Example:** Sven commits 10 AP worth of actions: Move (1 AP) → Attack (1 AP) → Move (1 AP) → Farm (1 AP) → Move (1 AP). He intended to attack Hero X, but Hero X dies during another hero's activation before Sven's turn.
- First Move executes: 1 AP spent (9 AP remaining).
**Example:** Sven commits 10 AP worth of actions: Move (1 AP) → Attack (1 AP) → Move (1 AP) → Farm (1 AP) → Move (1 AP). He intended to attack Hero X, but Hero X dies during another hero's activation before Sven's turn.
- First Move executes: 1 AP spent (9 AP remaining).
- Attack action revealed: Hero X is dead. Sven may either (a) cancel the Attack (returned to deck, 0 AP spent) or (b) attack a different valid target in range (Hero Y). He chooses to attack Hero Y: 1 AP spent (8 AP remaining).
- Second Move executes: 1 AP spent (7 AP remaining).
- Farm executes: 1 AP spent (6 AP remaining).
- Third Move executes: 1 AP spent (5 AP remaining).
- Sven's turn ends with 5 unused AP (which is lost).

**Example:** Crystal Maiden commits: Move (1 AP) → Crystal Nova (1 AP, 15 Mana) → Move (1 AP). She currently has 10 Mana.
- First Move executes normally: 1 AP spent.
- Crystal Nova token revealed: insufficient Mana (needs 15, has 10). No valid alternative exists — she cannot retarget this to make it work. Action automatically cancelled and returned to her available token pool, 0 AP spent.
- Second Move executes normally: 1 AP spent.
- The Crystal Nova token can be committed again in her next activation if she has enough Mana.

**Strategic Considerations:**
- Committing action types gives you strategic flexibility at execution time — you can adapt targets based on the actual game state when your turn arrives.
- Actions that require specific resources (Mana, AP, non-Silenced status) carry risk — if you don't meet the requirements, the action fails entirely regardless of what targets are available.
- Earlier heroes in turn order have more uncertainty about what the board state will be, but also more actual flexibility when their turn arrives since fewer actions have resolved.
- Later heroes can commit actions more confidently knowing more of the game state, but have less ability to adapt since more enemy actions have already resolved.

### Reactions
When an active hero targets your hero with an attack or ability, you may **React** before the effect resolves. Reactions interrupt the active hero's turn, are resolved immediately, and then the active hero continues.

**Rules:**
- A hero may only **react once** per opposing hero's activation (not once per round — once per turn when that specific enemy hero is acting).
- **Exception — Observer Ward Coverage:** If the attacking hero is standing in an area covered by an enemy **Observer Ward**, the defending team's heroes may react **twice** during that hero's activation instead of once. This represents the tactical advantage of having vision and awareness of enemy positioning.
- Reactions are **always paid from the reacting hero's next activation AP**. The cost is deducted at the start of that hero's next turn during Planning Phase — they simply have that many fewer AP to commit to actions.
- Only the **targeted hero** may react, not teammates.

**Reaction Types:**

| Reaction | AP Cost (from next turn) | Effect |
|---|---|---|
| **Flee** | 2 AP | Move 1 hex in any direction before the attack or ability resolves. If the attacker required adjacency or LoS, the attack misses entirely. |
| **Activate Defensive Item** | 1 AP | Immediately trigger a held defensive Item Card (e.g. BKB equivalent) before damage is applied. The item's effect takes place before resolution. |
| **Deny** | 1 AP | Contest an allied creep's last hit to deny the enemy gold and XP. See Economy and Progression for full rules. |
| **Dodge Skillshot** | 2 AP | Roll a die to attempt to dodge an incoming Skillshot ability. On success, the ability misses. On failure, the ability hits normally. Regardless of outcome, the hero must immediately move to an adjacent hex. Only usable against abilities marked as Skillshot. |

> **Example:** Juggernaut (4 AP) attacks Crystal Maiden. She reacts with **Flee** (costs 2 AP from her next turn), moving 1 hex away. Juggernaut is melee — he no longer has adjacency — so the attack misses. On Crystal Maiden's next turn she has 2 fewer AP to spend.

### Round End Phase
After all heroes on both sides have completed their turns, the following occur in order:

1. **Creep Spawning** — A new creep wave appears at the Creep Meeting Point in each lane (skipped during Round 1).
2. **Passive Income** — Every hero receives a fixed amount of gold regardless of activity.
3. **Power Rune Spawn** — On every 4th round, any player rolls the custom Rune Die and flips a coin simultaneously to determine the rune type and which river position it spawns at. See Vision, Runes, and Invisibility.
4. **Neutral Respawns** — On every even-numbered round, all cleared jungle camps are replenished.