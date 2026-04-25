# DOTA 2: THE BOARD GAME — TURN STRUCTURE

This document collects the rules for objective, setup, drafting, and the round-to-round flow of play.

---

## Objective

Destroy the enemy team's **Ancient**, located inside their base. To reach the Ancient, a team must destroy all Towers in at least one lane in sequence. The first team to destroy the enemy Ancient wins.

---

## Game Setup & Draft

### Hero Classes
Heroes are divided into three playable stat classes: **Agility**, **Strength**, and **Intelligence**. **Universal heroes are not used as a separate class in this game; Magnus is the current exception and is treated as a Strength hero.**

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
- Planning Tokens include: Move, Attack, Farm, Pass, 6 numbered item slot tokens per hero, and hero-specific ability tokens.
- Players may select up to their hero's AP worth of actions.
- Each hero also has **2 dedicated reaction token slots** for the current half-round.
- Tokens remain hidden until activation — players commit actions without knowing what enemies have planned.
- Once a hero's tokens are revealed at the start of their activation, actions are locked in and must be executed in the order committed unless prevented by crowd control, reactions, or game state changes.
- If a hero loses AP before their activation due to a stun or reaction cost, remove committed tokens from left to right until the removed tokens total at least the AP lost. Those removed actions are lost for that activation.
- Item use is committed by slot, not by a generic Use Item token. Revealing an item slot token means the hero is attempting to use the item currently in that numbered slot.
- Reactions **are** committed during Planning Phase using the hero's reaction slots.
- Any committed reaction reserves **1 AP** from that hero's normal AP budget for the current half-round.
- Reaction slots are **token slots**, not AP slots. Any action that costs exactly **1 AP** may be committed there if it is legal to use as an out-of-turn action.
- AP committed to reaction slots cannot also be committed to that hero's normal activation actions.
- If a committed reaction is never triggered during that half-round, its reserved AP is lost.

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
- If a hero loses their next turn to a stun, that activation is skipped and all committed actions for it are lost.

### Failed Actions
When a committed action cannot be executed, the following rules apply:

**Example Action Failure Causes:**
- **Invalid Target** — The target unit has moved, died, or is no longer in range/LoS.
- **Stunned Hero** — Hero has AP reduced below the cost of the action due to stun effects.
- **Silenced Hero** — Hero cannot use abilities while Silenced.
- **Insufficient Resources** — Hero lacks the Mana to cast a committed ability.
- **Invalid Item Slot** — The revealed item slot is empty, or the item expected to be there is no longer in that slot.
- **Movement Blocked** — The destination hex is occupied or impassable due to game state changes.

**Resolution:**
When a committed action is revealed during a hero's activation, the player declares the specific target or destination at that moment. If the action cannot be executed as originally intended, the player has two options:

1. **Cancel the action** — The token is returned to the hero's available token pool and can be committed again in a future activation. No AP is spent. The activation proceeds to the next committed action.
2. **Retarget the action** — If a valid alternative target or destination exists, the player may choose to execute the action on that alternative instead. The action executes normally and AP is spent as usual.

**Target Declaration Timing:**
- Specific targets (which enemy hero to attack, which hex to move to, which unit to cast an ability on) are **not** committed during Planning Phase.
- Only the **type** of action is committed (Move, Attack, Storm Hammer, Item Slot 2, etc.).
- The specific target or destination is declared when the token is revealed during execution.
- This gives players flexibility to adapt to game state changes, but commits them to the action type itself.

**When Retargeting is Not Possible:**
Some actions cannot be retargeted because no valid alternative exists:

- **Stunned Hero** — The action was already removed by the stun's token-removal rule, or the hero's entire activation was skipped. Action cannot execute at all.
- **Silenced Hero** — Hero cannot use abilities while Silenced. Ability actions cannot execute at all.
- **Insufficient Resources** — Hero lacks the Mana to cast a committed ability. Action cannot execute at all.
- **Invalid Item Slot** — The chosen slot is empty, or no usable item is currently in that slot. The item action cannot execute.
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
Reactions are pre-committed out-of-turn actions that can interrupt another hero's turn. They are committed during Planning Phase, triggered after targeting is declared, resolved immediately, and then the active hero continues.

**Rules:**
- A reaction is, in its purest form, an action taken out of turn.
- Only heroes **directly affected** by the triggering action may react. A hero is directly affected if they are targeted by the action, included in its affected area or skillshot path, or are eligible to use **Deny** against that action.
- A hero may normally use only **1 committed reaction** per half-round.
- **Exception — Observer Ward Coverage:** If the acting enemy hero is standing in an area covered by an allied **Observer Ward**, each directly affected defending hero may use up to **2 committed reactions** during that half-round instead of 1.
- A hero may split those 2 reactions across different triggers during the same half-round if later valid triggers occur.
- Reactions are triggered **after targeting is declared** and **before** the triggering action resolves.
- If multiple defending heroes react to the same action, reactions resolve in **turn-order order** among the eligible defenders.
- A committed reaction can only be used if that hero is currently able to perform that action. If the reaction becomes illegal before use, it cannot be used and the reserved AP remains lost for that half-round.
- When a committed reaction is used, its specific target or destination is declared at that moment using the normal targeting rules for that action.

**Common Reaction Uses:**

| Reaction | AP Cost | Effect |
|---|---|---|
| **Move** | 1 AP | Reposition 1 hex using the normal movement rules before the triggering action resolves. If this movement breaks the attacker's required adjacency or Line of Sight, the attack or ability misses. |
| **Activate Defensive Item** | 1 AP | Immediately trigger a committed defensive item-slot action before damage is applied. The item's effect takes place before resolution. |
| **Deny** | 1 AP | Contest an allied creep's last hit to deny the enemy gold and XP. See Economy and Progression for full rules. |

These are common reactions, not the full limit of the system. Any committed action that costs exactly **1 AP** may be used as a reaction if it is legal to perform at that timing window.

**Examples of legal 1 AP reactions:**
- **Movement reaction:** A hero commits **Move** into a reaction slot so they can reposition out of danger when directly affected.
- **Ability reaction:** Mirana commits **Leap** into a reaction slot. If she is directly affected by an enemy action later in the half-round and is still able to Leap, she may use it out of turn as her reaction.
- **Item reaction:** A hero commits an item-slot token for a 1 AP defensive item, then triggers it when directly affected before damage resolves.
- **Deny reaction:** A hero commits **Deny** into a reaction slot so they can contest an enemy **Farm** action against an allied creep wave.

**Dodging a Skillshot:**
- A hero may attempt to dodge a **Skillshot** only by using a committed **1 AP movement action or 1 AP movement ability** as their reaction.
- After the Skillshot's path is declared and before it resolves, both players roll a die: the reacting hero and the acting hero.
- If the reacting hero rolls higher, the Skillshot misses.
- If the acting hero rolls equal or higher, the Skillshot hits normally.
- The reacting hero then resolves the committed movement action or movement ability used for the dodge, following that action's normal movement rules.

> **Example:** Crystal Maiden commits **Move** into one of her reaction slots during Planning Phase, reserving 1 AP for it. Later in the half-round, Juggernaut attacks her from melee range. After Juggernaut declares Crystal Maiden as the target, she triggers that committed **Move**, chooses an adjacent hex, and moves there before the attack resolves. Because Juggernaut no longer has adjacency, the attack misses. That 1 reserved AP is already spent for the half-round and cannot be used during Crystal Maiden's own activation.

> **Example:** Mirana commits **Leap** into a reaction slot during Planning Phase, reserving 1 AP for it. Later in the half-round, an enemy declares an attack against her. After targeting is declared, Mirana may trigger **Leap** as her reaction, moving according to Leap's rules before the enemy action resolves. If no valid trigger occurs before Mirana's own activation, the reserved AP is still lost for the half-round, but she may still use Leap normally on her turn if she has the AP and a legal action slot for it.

> **Example:** Pudge throws **Meat Hook** at Mirana. Mirana has committed **Leap** in a reaction slot. After the Hook path is declared and before it resolves, both players roll a die. If Mirana rolls higher than Pudge, the Hook misses and Mirana resolves **Leap** normally. If Pudge rolls equal or higher, the Hook hits normally and Mirana does not avoid the Hook.

### Round End Phase
After all heroes on both sides have completed their turns, the following occur in order:

1. **Creep Spawning** — A new creep wave appears at the Creep Meeting Point in each lane (skipped during Round 1).
2. **Passive Income** — Every hero receives a fixed amount of gold regardless of activity.
3. **Power Rune Spawn** — On every 4th round, determine the rune type and flip a coin to determine which river position it spawns at, then place the matching Power Rune token. See Vision, Runes, and Invisibility.
4. **Neutral Respawns** — On every even-numbered round, all cleared jungle camps are replenished.