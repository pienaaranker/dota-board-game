# DOTA 2: THE BOARD GAME — VISION, RUNES, AND INVISIBILITY

This document collects rune rules, warding rules, and the hidden-information systems around invisibility and smoke.

---

## Power Runes

Every **4th round**, a Power Rune spawns at one of two designated **River rune positions** — one on the Radiant side, one on the Dire side. At the **start of that round**, determine the rune type, then flip a **coin** to determine which side receives it. Place the matching **Power Rune token** on that river position. Only one rune exists on the board at a time.

| Rune | Effect |
|---|---|
| **Illusion** | Creates 3 Illusion tokens controlled by the hero. Illusions deal reduced damage and take increased damage. |
| **Haste** | Move actions move the hero 2 areas per AP spent, for the duration. |
| **Invisibility** | Grants the hero the Invisibility status (see below). |
| **Regeneration** | Restores full Health and Mana. Can be interrupted by an enemy attack before completion, reducing the amount restored. |
| **Double Damage** | All attacks deal double the hero's Damage value, for the duration. |

- A hero claims the rune by moving into its area.
- The specific rune is represented by its matching single-hex Power Rune token.
- Only one rune exists on the board at a time. An unclaimed rune remains until picked up or replaced at the next spawn.

---

## Vision & Invisibility

### Default Visibility
All units are **visible** to both teams unless they have the Invisibility status.

### Gaining Invisibility
Invisibility is granted by:
- The **Invisibility Rune** (see above).
- Certain hero abilities and **Item Cards**.
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
- Ward duration is tracked on the shared board's ward log using a die or generic number marker, not a dedicated ward-duration token.
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