# DOTA 2: THE BOARD GAME — ITEMS

This document defines all items included in the board game. Each entry describes the item's intended board game effect, cost, and type. For purchasing rules, item slots, and delivery mechanics, see [../../rulebook/mechanics/Mechanics.md](../../rulebook/mechanics/Mechanics.md).

Items marked **🔲 TODO** are pending final design confirmation. Items marked **✅ Confirmed** are fully designed and locked in.

---

## How to Read Item Entries

Each entry includes:
- **Type** — *Consumable*, *Passive*, *Active*, *Passive / Active*, or *Aura*
- **Cost** — Gold required to purchase

Stat shorthand used throughout:
- **HP** — Health points
- **Mana** — Resource for abilities
- **Attack** — Physical damage
- **Armor** — Damage reduction against physical attacks
- **Movement** — Hexes moved per Move AP
- **Attack Speed** — Attacks available per Attack AP

---

## Consumables

Single-use items. Once activated, the item card is discarded.

#### Blood Grenade *(50 Gold)*
**Type:** Consumable | **Status:** ✅ Confirmed

Thrown at a target hex within range. Apply a **Bleed** token to all enemy heroes within a **1-hex radius** of the target hex (the target hex and all 6 adjacent hexes). Bleed deals X physical damage at the start of each of the affected hero's turns for Y turns. Bleed is dispellable. See [../../rulebook/mechanics/Mechanics.md](../../rulebook/mechanics/Mechanics.md) for DoT rules.

---

#### Bottle *(675 Gold)*
**Type:** Consumable / Active | **Status:** ✅ Confirmed

Can store one Rune token or be used if full. **Use:** Restore X HP and Y Mana over 4 turns. **Stored Rune:** Consume the stored Rune for its full effect. Refilled at the Fountain. One Bottle per hero maximum.

---

#### Clarity *(60 Gold)*
**Type:** Consumable | **Status:** ✅ Confirmed

Restore X Mana over 2 rounds. Interrupted if the user takes damage from an enemy hero before regen completes.

---

#### Dust of Appearance *(80 Gold)*
**Type:** Consumable | **Status:** ✅ Confirmed

Use during your turn (1 AP). Remove Invisible tokens from all enemy heroes within 2 hexes. Affected heroes cannot regain Invisibility for 1 round.

---

#### Enchanted Mango *(65 Gold)*
**Type:** Consumable | **Status:** ✅ Confirmed

Instantly restore X Mana. Can be used on an allied hero within 1 hex instead of self.

---

#### Healing Salve *(100 Gold)*
**Type:** Consumable | **Status:** ✅ Confirmed

Restore X HP over 2 rounds. Interrupted if the user takes damage from an enemy hero before regen completes.

---

#### Observer Ward *(50 Gold)*
**Type:** Consumable (Placeable) | **Status:** ✅ Confirmed

Place on any Open hex (1 AP). The ward token remains on the board until destroyed and covers a fixed radius of hexes as printed on the item card.

**Tactical Advantage:** While an enemy hero is standing within a warded area, any allied hero they target may use **two reactions** instead of the normal one. This represents the awareness and intel that vision provides. Heroes attacking from under **Smoke of Deceit** bypass this advantage entirely.

Observer Wards do **not** grant invisibility detection — they only provide the reaction advantage. Use Sentry Wards or Dust of Appearance for that.

**Destroying a Ward:** Observer Wards are invisible to the enemy team and cannot be targeted or destroyed unless first revealed by **true sight**. A ward is revealed if it falls within the radius of an enemy **Sentry Ward**, or within range of an enemy hero carrying a **Gem of True Sight**. Once revealed, an adjacent hero may spend 1 AP to destroy it. See [../../rulebook/mechanics/Mechanics.md](../../rulebook/mechanics/Mechanics.md) for full ward rules.

---

#### Sentry Ward *(50 Gold)*
**Type:** Consumable (Placeable) | **Status:** ✅ Confirmed

Place on any Open hex (1 AP). The ward token remains on the board until destroyed and provides **true sight** within its printed radius.

**True Sight:** All enemy units with Invisibility tokens and all enemy Observer Wards within the radius are revealed for as long as the Sentry Ward remains active. Revealed Observer Wards may be destroyed by an adjacent hero spending 1 AP.

**Invisible by default:** Like Observer Wards, Sentry Wards are invisible to the enemy team. They can only be revealed and destroyed if the enemy has a true sight source of their own covering the ward's hex.

Sentry Wards do **not** provide the tactical reaction advantage that Observer Wards do — they are purely a detection tool. See [../../rulebook/mechanics/Mechanics.md](../../rulebook/mechanics/Mechanics.md) for full ward rules.

---

#### Smoke of Deceit *(50 Gold)*
**Type:** Consumable | **Status:** ✅ Confirmed

When activated, all affected heroes (the user and all allied heroes within **2 hexes**) move together under a single **Smoke Cloud** token for group invisibility. The hero who activates Smoke **cannot attack or use offensive abilities for the remainder of that turn**. Heroes under Smoke are **invisible to Observer Wards** and do not trigger the tactical reaction advantage. When a Smoke hero attacks or uses an offensive ability, the targeted hero **cannot use reactions** — the attack resolves uncontested — and Smoke immediately dispels from the attacker.

**Smoke dispels from all affected heroes when any one of them:**
- Moves within **3 hexes** of an enemy hero.
- Enters a Tower's area of control.
- Attacks or uses an offensive ability.

See [../../rulebook/mechanics/Mechanics.md](../../rulebook/mechanics/Mechanics.md) for full Smoke rules.

---

#### Tango *(90 Gold)*
**Type:** Consumable | **Status:** ✅ Confirmed

Target an adjacent Tree hex — it is destroyed (becomes Open). Restore X HP to the using hero over 2 rounds. The destroyed Tree follows standard regrowth rules.

---

#### Town Portal Scroll *(100 Gold)*
**Type:** Consumable (Channeled) | **Status:** 🔲 TODO

Channel: spend 2 AP. At the start of your next turn, teleport to any friendly structure (Tower, Barracks, or Fountain). Cancelled only if the hero is Stunned or Rooted while channeling. Consumed on use.

---

## Miscellaneous

Standalone items that don't fit neatly into an upgrade line.

#### Blink Dagger *(2250 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Instantly teleport up to X hexes in any direction, ignoring all terrain and units. Cannot be activated if this hero took damage this round.

---

#### Boots of Speed *(500 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+1 Movement.

---

#### Gem of True Sight *(900 Gold)*
**Type:** Passive | **Status:** ✅ Confirmed

While carried, grants the hero **true sight** in a radius around them at all times: all enemy units with Invisibility tokens and all enemy Observer Wards within range are revealed.

**On death:** The Gem drops onto the hero's hex as a token. Any hero — from either team — may pick it up by moving onto that hex. The Gem is never destroyed.

---

#### Ghost Scepter *(1500 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Become Ethereal for 1 round: immune to physical attack damage, cannot attack, takes increased magic damage. Ends at start of your next turn.

---

## Accessories

#### Boots of Travel *(2500 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 2 AP. Teleport to any friendly structure (Tower, Barracks, Fountain) or allied creep wave position. Cooldown: 4 rounds.

---

#### Bracer *(505 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+HP, small +Armor and +Attack bonuses.

---

#### Falcon Blade *(1125 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack Speed. Restore X Mana at the start of each of your turns.

---

#### Hand of Midas *(2200 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Once per round, use during a Farm action on a neutral camp: gain double gold and bonus XP from that camp. Cannot be used on lane creeps.

---

#### Magic Wand *(460 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

**Passive:** Each time an enemy hero within 3 hexes uses an ability, add 1 charge to this item (max 15), tracked with a die or generic counter. **Active:** Spend all charges — restore HP and Mana equal to the number of charges spent.

---

#### Mask of Madness *(1900 Gold)*
**Type:** Active (Toggle) | **Status:** 🔲 TODO

Toggle on/off during your turn (costs 1 AP to activate). **While active:** +Attack Speed and Lifesteal (restore X HP per attack dealt). **Drawback:** While active, hero is Silenced — cannot use abilities.

---

#### Moon Shard *(4000 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

**Passive:** +Attack Speed; hero may attack twice per Attack AP spent. **Active (consume):** Permanently gain +1 Attack and discard this item card.

---

#### Null Talisman *(505 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Mana, small bonus to magic damage dealt by abilities.

---

#### Oblivion Staff *(1625 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Mana, +Attack Speed. Restore X Mana at the start of each of your turns.

---

#### Perseverance *(1400 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

Restore X HP and Y Mana at the start of each of your turns.

---

#### Phase Boots *(1500 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

**Passive:** +1 Movement. **Active:** Spend 1 AP. For this turn only, the hero may move through hexes occupied by allied or enemy heroes (but not terrain).

---

#### Power Treads *(1400 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

**Passive:** +1 Movement, +Attack Speed. **Active (free action):** Switch between Strength (+HP), Agility (+Attack), and Intelligence (+Mana) stances for different stat bonuses.

---

#### Soul Booster *(3000 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

Large +HP and +Mana.

---

#### Soul Ring *(805 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Convert X HP into Y Mana. Cannot be used if it would leave the hero at 0 HP.

---

#### Wraith Band *(505 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack, small +Movement and +HP bonuses.

---

## Support

Items focused on team utility, healing, and auras.

#### Arcane Boots *(1500 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Restore X Mana to all allied heroes within 2 hexes. Cooldown: 3 rounds.

---

#### Boots of Bearing *(4225 Gold)*
**Type:** Aura / Active | **Status:** 🔲 TODO

**Aura:** Allied heroes within 2 hexes gain +Attack Speed. **Active:** Spend 1 AP. Additionally grant all nearby allies +1 Movement for 1 round.

---

#### Drum of Endurance *(1625 Gold)*
**Type:** Active (Charges) | **Status:** 🔲 TODO

Comes with 5 charges, tracked with a die or generic counter. Spend 1 AP to consume 1 charge: grant +1 Movement and +Attack Speed to yourself and all allied heroes within 2 hexes for 1 round.

---

#### Guardian Greaves *(4450 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Heal all allied heroes within 2 hexes for X HP and remove one debuff token from each. Cooldown: 3 rounds.

---

#### Holy Locket *(2250 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+HP, +Mana. All healing effects applied to this hero are increased by 30%.

---

#### Medallion of Courage *(975 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Target an enemy hero or structure within range: reduce their Armor by X for 1 round. Alternatively, target an allied hero: grant them +Armor for 1 round.

---

#### Mekansm *(1775 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Restore X HP to all allied heroes within 3 hexes. Cooldown: 3 rounds.

---

#### Pavise *(1350 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Apply a Shield token to yourself or target allied hero within 2 hexes. The shield absorbs the next X incoming damage (physical or magic). Token lasts until consumed or end of round.

---

#### Pipe of Insight *(3725 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Grant a Magic Barrier token to all allied heroes within 2 hexes. Each token absorbs the next instance of magic damage that hero receives. Cooldown: 3 rounds.

---

#### Solar Crest *(2575 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Target an allied hero within range: grant +Armor and Evasion chance (roll 5+ to dodge next attack) for 1 round. Or target an enemy hero: reduce their Armor and remove their Evasion for 1 round.

---

#### Spirit Vessel *(2725 Gold)*
**Type:** Active (Charges) | **Status:** 🔲 TODO

Gain 2 charges each time a nearby enemy hero dies, tracked with a die or generic counter. Spend 1 AP to use 2 charges: target enemy hero — deal X damage per round for 2 rounds and suppress their HP regen; or target allied hero — restore X HP per round for 2 rounds.

---

#### Tranquil Boots *(900 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+1 Movement. Restore X HP at the start of each of your turns, unless you took damage during the previous round.

---

#### Urn of Shadows *(825 Gold)*
**Type:** Active (Charges) | **Status:** 🔲 TODO

Gain 2 charges each time a nearby enemy hero dies, tracked with a die or generic counter. Spend 1 AP to use 2 charges: heal target allied hero for X HP, or deal X damage per round for 2 rounds to target enemy hero within range.

---

#### Vladmir's Offering *(2200 Gold)*
**Type:** Aura | **Status:** 🔲 TODO

Allied heroes within 2 hexes gain Lifesteal (restore X HP each time they deal attack damage) and +Armor.

---

## Magical

Items focused on ability enhancement, crowd control, and magical effects.

#### Aghanim's Scepter *(4200 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

Upgrades this hero's ultimate ability as printed on the hero's Abilities Card (Aghanim's Scepter upgrade section).

---

#### Bloodstone *(4700 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

Large +Mana and +Mana Regen. On death: deal X magic damage to all enemy heroes within 3 hexes.

---

#### Dagon *(3050 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Deal X magic damage to a single enemy hero within range. Can be upgraded (Level 1–5) at the Fountain, each level increasing damage at additional gold cost.

---

#### Ethereal Blade *(5200 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Target enemy hero becomes Ethereal for 1 round (cannot attack, takes increased magic damage, immune to physical attacks) and immediately takes X magic damage.

---

#### Eul's Scepter of Divinity *(2600 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Target any unit within range: that unit is lifted (Cyclone — untargetable and invulnerable) for 1 round and all debuffs are removed. Unit lands on the same hex at the start of their next turn.

---

#### Force Staff *(2200 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Push target unit (ally, enemy, or self) 4 hexes in a chosen direction. The unit stops at the last valid Open hex in that direction.

---

#### Gleipnir *(4650 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Root target enemy hero and up to 2 additional enemy heroes within 2 hexes of the target. All Rooted heroes take X magic damage and cannot move for 1 round.

---

#### Glimmer Cape *(2150 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Become Invisible and gain +Magic Resistance for 1 round. Invisibility ends if you attack or use a damaging ability.

---

#### Meteor Hammer *(2850 Gold)*
**Type:** Active (Channeled) | **Status:** 🔲 TODO

Spend 1 AP to begin channeling. Target a hex within range. After a 1-round delay, deal X magic damage and Stun all units on the target hex and adjacent hexes for 1 round. Channel interrupted if hero moves or takes damage.

---

#### Octarine Core *(4900 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+HP, +Mana. Restore X HP each time you deal magic damage with an ability (Spell Lifesteal). All ability cooldowns reduced by 1 round (minimum 1).

---

#### Orchid Malevolence *(3275 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Silence target enemy hero for 2 rounds — they cannot use abilities. When the Silence ends, deal bonus magic damage equal to 20% of all ability damage that hero dealt while Silenced (track with a counter token).

---

#### Refresher Orb *(5000 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 2 AP. Reset all ability and item cooldowns for this hero to 0. Can only be used once per game.

---

#### Rod of Atos *(2250 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Root target enemy hero within range — they cannot move for 2 rounds but may still attack and use abilities.

---

#### Scythe of Vyse *(5200 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Hex (polymorph) target enemy hero for 2 rounds: they cannot attack, use abilities, or use items. All buff tokens on that hero are removed while Hexed.

---

#### Wind Waker *(6800 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Lift yourself or target allied hero into the wind (Cyclone — untargetable, invulnerable) for up to 2 rounds. The lifted hero's player chooses when to land (on their turn). On landing, place the hero on any hex within 5 hexes of the takeoff point.

---

## Armor

Items focused on defense, damage mitigation, and survivability.

#### Aeon Disk *(3000 Gold)*
**Type:** Passive (Trigger) | **Status:** 🔲 TODO

When this hero's HP drops to 20% or below, automatically gain an Aeon Shield token: immune to all damage and most debuffs for 1 round. Triggers once per game.

---

#### Assault Cuirass *(5125 Gold)*
**Type:** Aura | **Status:** 🔲 TODO

+Armor, +Attack Speed. **Aura:** Allied heroes within 2 hexes gain +Armor; enemy heroes within 2 hexes suffer –Armor.

---

#### Black King Bar *(4050 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Become Magic Immune for 1 round: immune to all magic damage and ability effects, except abilities explicitly marked "pierces BKB" on the hero's Abilities Card. Cooldown decreases with each use (first use: 3 rounds; subsequent uses: 2 rounds, minimum 1).

---

#### Blade Mail *(2400 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. For 1 round, any attack damage dealt to this hero is also applied to the attacker. +Armor.

---

#### Crimson Guard *(3725 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Apply a Physical Block token to yourself and all allied heroes within 2 hexes. Each token negates the first physical damage instance that hero receives. Cooldown: 3 rounds.

---

#### Eye of Skadi *(5900 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

Large +HP, +Mana, +Attack. Attacks from this hero apply an Arctic Slow token to the target: –1 Movement and reduced Attack Speed for 1 round.

---

#### Heart of Tarrasque *(5100 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

Large +HP. If this hero did not take damage during the previous round, restore X HP at the start of your turn.

---

#### Linken's Sphere *(4800 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

Once every 2 rounds, automatically block the next single-target ability cast at this hero. The blocked ability is completely negated. Cooldown resets after triggering.

---

#### Lotus Orb *(3850 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Apply a Lotus Echo token to yourself or target allied hero within range. The next single-target ability cast at that hero is reflected back at the caster and negated on the original target. Echo lasts until triggered or end of round.

---

#### Shiva's Guard *(4500 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

**Passive:** +Armor. **Active:** Spend 1 AP. Emit a Frost Wave — all enemy heroes within 3 hexes take X magic damage and receive –1 Movement for 1 round. Cooldown: 2 rounds.

---

#### Vanguard *(1700 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+HP. Each time this hero takes attack damage, roll a die. On 4+, reduce incoming damage by X (damage block).

---

#### Veil of Discord *(1700 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Apply a Veil token to all enemy heroes within 2 hexes: they take +25% magic damage for 2 rounds.

---

## Weapons

Items focused on attack damage, on-hit effects, and offensive power.

#### Abyssal Blade *(6250 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

**Passive:** +Attack. Attacks have a 25% chance to Bash (roll 5+): deal bonus damage and Stun the target for 1 round. **Active:** Spend 1 AP. Guarantee a Bash on target enemy hero — bypasses Linken's Sphere.

---

#### Battle Fury *(3900 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack, +HP Regen, +Mana Regen. **Cleave:** When this hero deals attack damage, 35% of that damage is also applied to all enemy units within 1 hex of the target.

---

#### Bloodthorn *(6400 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Silence target enemy hero for 2 rounds. While Silenced by Bloodthorn, all attacks against that hero from any source are treated as Critical Hits.

---

#### Butterfly *(5450 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack, +Attack Speed. **Evasion:** When this hero is attacked, roll a die. On 5+, dodge the attack entirely.

---

#### Crystalys *(2000 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack. Attacks have a chance to be a Critical Hit (roll 5+): deal 150% damage.

---

#### Daedalus *(5100 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack. Attacks have a high chance to be a Critical Hit (roll 4+): deal 225% damage.

---

#### Desolator *(3500 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack. Attacks apply Corruption: reduce the target's Armor by 1 (stackable up to 3). Stacks reset when combat with that unit ends.

---

#### Diffusal Blade *(2500 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

**Passive:** +Attack. Attacks burn X Mana from the target. If the target has no Mana, deal bonus damage instead. **Active:** Spend 1 AP. Apply a Slow token (–1 Movement for 1 round) to target enemy hero.

---

#### Disperser *(6100 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

Upgraded Diffusal Blade. **Passive:** Increased Mana burn on attacks. **Active:** Spend 1 AP. Purge target enemy hero — remove all positive buff tokens and apply a Slow token.

---

#### Divine Rapier *(5600 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

Massive +Attack. **On death:** This item drops to the hero's hex as a token. Any hero who moves onto that hex immediately picks it up, regardless of team.

---

#### Mage Slayer *(3100 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack, +Magic Resistance. Attacks apply Mage Slayer Debuff: target hero deals –25% magic damage for 1 round.

---

#### Monkey King Bar *(5000 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack. Attacks bypass all Evasion effects — cannot be dodged. Small chance to Mini-Bash (roll 6): deal bonus magic damage and briefly stun the target.

---

#### Nullifier *(4350 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Target enemy hero within range: remove all positive buff tokens and apply Nullify — they cannot use items for 2 rounds.

---

#### Parasma *(5975 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack, +Mana. Attacks deal bonus magic damage. **On kill:** Place one Illusion token of the killed hero under this hero's control for 1 round (acts on owner's turn at reduced stats).

---

#### Radiance *(4700 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack. **Burn Aura:** At the start of each round, all enemy heroes within 2 hexes take X magic damage. Enemy heroes within 1 hex also suffer Miss Chance: roll 3 or lower on an attack die to miss.

---

#### Revenant's Brooch *(3300 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. For 1 round, this hero's attacks become magic damage, gain +1 Attack Range, and bypass Magic Immunity (BKB).

---

#### Shadow Blade *(3250 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Become Invisible. The next attack made from Invisible state deals bonus damage and ends Invisibility. Moving does not break Invisibility; attacking or using abilities does.

---

#### Silver Edge *(5700 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Upgraded Shadow Blade. Spend 1 AP. Become Invisible. The next attack from Invisible state deals bonus damage, ends Invisibility, and applies Break to the target for 2 rounds — disabling all of that hero's passive abilities.

---

#### Skull Basher *(2875 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack, +HP. Attacks have a 25% chance to Bash (roll 5+): deal bonus damage and Stun the target for 1 round.

---

#### Witch Blade *(2775 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack Speed, +Armor. Attacks deal bonus magic damage and apply a Slow token (–1 Movement for 1 round).

---

## Armaments

Hybrid items combining offensive power with utility effects.

#### Dragon Lance *(1900 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+HP, +Attack Range (+1 hex reach on attacks).

---

#### Echo Sabre *(2700 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack, +Mana Regen. The first attack each turn triggers an Echo Attack: a second immediate attack at 50% damage.

---

#### Harpoon *(4700 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Pull target enemy hero within range to the hex adjacent to this hero. Can interrupt channeled abilities.

---

#### Heaven's Halberd *(3400 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

+HP. **Active:** Spend 1 AP. Disarm target enemy hero for 2 rounds — they cannot make attack actions.

---

#### Hurricane Pike *(4450 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

+Attack Range. **Active:** Spend 1 AP. Push target enemy hero 3 hexes directly away from this hero. Can alternatively be used on self to push away from an adjacent enemy.

---

#### Hydra's Breath *(5900 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack. Attacks deal full damage to the primary target and 50% damage to all other enemy heroes within 1 hex of the target.

---

#### Kaya *(2100 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Mana. Abilities deal +12% bonus magic damage.

---

#### Kaya and Sange *(4200 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+HP, +Mana. Abilities deal bonus magic damage. Debuff durations applied to this hero are reduced.

---

#### Khanda *(5600 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+HP, +Attack. When you cast a damaging ability, it has a 25% chance to be a Critical Ability Hit (roll 5+): deal 150% of the ability's normal damage.

---

#### Maelstrom *(2950 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack. Attacks have a 20% chance to trigger Chain Lightning (roll 5+): deal X magic damage to the target and bounce to up to 2 additional nearby enemy heroes.

---

#### Manta Style *(4650 Gold)*
**Type:** Active | **Status:** 🔲 TODO

Spend 1 AP. Place 2 Illusion tokens of this hero on adjacent hexes. Illusions last 2 rounds, have 33% of this hero's stats, deal 35% damage, and take 350% damage. Illusions are controlled by the same player and act on this hero's turn.

---

#### Mjollnir *(5500 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

Upgraded Maelstrom. **Passive:** Chain Lightning triggers more frequently (roll 4+). **Active:** Spend 1 AP. Apply a Static Shield token to yourself or target allied hero — the next hero to attack them takes X magic damage.

---

#### Phylactery *(2600 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Mana, +HP. After this hero casts any ability, their next attack within 1 round applies a Slow token and deals bonus magic damage.

---

#### Sange *(2100 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+HP. Debuff durations applied to this hero are reduced.

---

#### Sange and Yasha *(4200 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+HP, +Attack Speed, +1 Movement. Debuff durations applied to this hero are reduced.

---

#### Satanic *(5050 Gold)*
**Type:** Passive / Active | **Status:** 🔲 TODO

+Attack, +HP. **Passive:** Attacks restore X% of damage dealt as HP (Lifesteal). **Active:** Spend 1 AP. For 1 round, Lifesteal is massively amplified.

---

#### Specialist's Array *(2550 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack. Attacks hit the primary target for full damage and up to 2 additional enemy heroes within range for 30% damage (Split Shot).

---

#### Yasha *(2100 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack Speed, +1 Movement.

---

#### Yasha and Kaya *(4200 Gold)*
**Type:** Passive | **Status:** 🔲 TODO

+Attack Speed, +1 Movement, +Mana. Abilities deal bonus magic damage.

---

## Secret Shop

The Secret Shop on the board stocks a limited item pool separate from the Fountain. The specific items available at the Secret Shop are **🔲 TODO** — to be chosen from the items in this document once individual item designs are confirmed.

**Design notes:**
- Prefer high-cost items that are worth the risk of entering enemy jungle
- Items with strong global or area effects are good candidates
- Aim for a pool of around 8–12 items per shop

---

## Excluded Items

| Item | Original Category |
|------|------------------|
| Aghanim's Shard | Consumables |
| Faerie Fire | Consumables |
| Band of Elvenskin | Attributes |
| Belt of Strength | Attributes |
| Blade of Alacrity | Attributes |
| Circlet | Attributes |
| Crown | Attributes |
| Diadem | Attributes |
| Gauntlets of Strength | Attributes |
| Iron Branch | Attributes |
| Mantle of Intelligence | Attributes |
| Ogre Axe | Attributes |
| Robe of the Magi | Attributes |
| Slippers of Agility | Attributes |
| Staff of Wizardry | Attributes |
| Blades of Attack | Equipment |
| Blitz Knuckles | Equipment |
| Broadsword | Equipment |
| Chainmail | Equipment |
| Claymore | Equipment |
| Gloves of Haste | Equipment |
| Helm of Iron Will | Equipment |
| Infused Raindrops | Equipment |
| Javelin | Equipment |
| Mithril Hammer | Equipment |
| Orb of Blight | Equipment |
| Orb of Frost | Equipment |
| Orb of Venom | Equipment |
| Quelling Blade | Equipment |
| Ring of Protection | Equipment |
| Splintmail | Equipment |
| Chasm Stone | Miscellaneous |
| Cloak | Miscellaneous |
| Fluffy Hat | Miscellaneous |
| Magic Stick | Miscellaneous |
| Morbid Mask | Miscellaneous |
| Ring of Health | Miscellaneous |
| Ring of Regen | Miscellaneous |
| Sage's Mask | Miscellaneous |
| Shadow Amulet | Miscellaneous |
| Shawl | Miscellaneous |
| Void Stone | Miscellaneous |
| Voodoo Mask | Miscellaneous |
| Wind Lace | Miscellaneous |
| Wizard Hat | Miscellaneous |
| Demon Edge | Secret Shop |
| Eaglesong | Secret Shop |
| Energy Booster | Secret Shop |
| Hyperstone | Secret Shop |
| Mystic Staff | Secret Shop |
| Platemail | Secret Shop |
| Point Booster | Secret Shop |
| Reaver | Secret Shop |
| Ring of Tarrasque | Secret Shop |
| Sacred Relic | Secret Shop |
| Talisman of Evasion | Secret Shop |
| Tiara of Selemene | Secret Shop |
| Ultimate Orb | Secret Shop |
| Vitality Booster | Secret Shop |
| Orb of Corrosion | Accessories |
| Essence Distiller | Support |
| Headdress | Support |
| Ring of Basilius | Support |
| Aether Lens | Magical |
| Crella's Crozier | Magical |
| Armlet of Mordiggian | Armor |
| Buckler | Armor |
| Consecrated Wraps | Armor |
| Helm of the Dominator | Armor |
| Helm of the Overlord | Armor |
| Arcane Blink | Armaments |
| Overwhelming Blink | Armaments |
| Swift Blink | Armaments |
