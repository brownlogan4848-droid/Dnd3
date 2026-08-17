# NARUTO COMPENDIUM — BOOK IV: THE GAME

*The complete Shinobi Chronicles system, combat, jutsu progression, and everything behind the screen.*

**Companion to:** the Jutsu Compendium (7 rank files) and the other three Books.


**Contents**

- **§1** — The Shinobi Chronicles System
- **§2** — Advanced Combat & Combo Mastery
- **§3** — Jutsu Mastery & Creation
- **§4** — Npc & Threat Design
- **§5** — Gm Toolkit

---
---

# §1 — THE SHINOBI CHRONICLES SYSTEM

**This file replaces the earlier generic D&D 5e conversion.** It documents the actual *Naruto D&D: Shinobi Chronicles* system as defined by the character sheet, Body Origin sheet, Clan Bloodline Reference, Genin Ability sheet, Combo System sheet, and NPC guidance sheet.

**Sourcing convention for this file:**

| Tag | Meaning |
|---|---|
| **[SHEET]** | Printed directly on one of the official sheets. Authoritative. |
| **[INF]** | Extrapolated from the sheets to fill an obvious gap. |
| **[GM]** | Table addition — not on any sheet. Optional. |
| **[CONFLICT]** | The sheets and the Jutsu Compendium disagree. Flagged, not resolved. |

---
---

### PART ONE — CORE ARCHITECTURE **[SHEET]**

#### The Three Resources

This is the system's defining feature and its biggest departure from standard 5e. **There are no spell slots.** There are three bars.

| Resource | Starting value | Spent on |
|---|---|---|
| **Chakra** | 100 / 100 | Ninjutsu, Genjutsu, activating abilities |
| **Stamina** | 100 / 100 | Movement, Taijutsu, dodging, blocking, physical effort |
| **Special** | 0 / 100 | Powerful techniques, clan awakenings, unique events |

**Chakra and Stamina start full and deplete. Special starts empty and fills.** That inversion is the whole rhythm of a fight: you begin strong and get tired, but you also begin ordinary and become dangerous.

#### The Special Bar **[SHEET]**

**Gain Special by:** landing attacks, taking damage, completing objectives, roleplay, and critical moments.
**Spend Special to:** unleash stronger techniques, awaken clan abilities, or trigger powerful effects.

##### Suggested gain values **[GM — the sheets name the triggers but not the numbers]**

| Trigger | Special gained |
|---|---|
| Start of each combat round | +5 |
| Land a hit | +5 |
| Land a critical hit | +10 |
| Take a hit dealing 25%+ of your max HP | +15 |
| Reduce an enemy to 0 HP | +15 |
| Complete a mission objective | +20 |
| A genuine character moment (DM's call) | +10 |

##### THE SPEND MENU **[GM]** — *the single authoritative list*

> **This table is the only Special spend menu in the system.** Book IV §2 Part Four repeats the *combat finisher* rows for convenience during a fight; Book 0 repeats a subset for lookup. Neither adds costs, and neither overrides this table. If a number disagrees anywhere, this one is correct.

| Effect | Special | Where it's used |
|---|---:|---|
| **Heavy Strike** — the action deals **+2 damage dice** | **20** | Combo finisher — §2 Part Four |
| **Unavoidable** — the action cannot be dodged, blocked, or substituted | **30** | Combo finisher — §2 Part Four |
| **Push through an interruption** — continue your own broken combo; next action takes an additional **−2** | **30** | §2 Part Five. **The only way without a feature. There is no free save.** |
| **Ignore the Chakra *or* Stamina cost** of one technique | **30** | Any time |
| **Extension** — add one action beyond your combo limit, ignoring slot cost | **40** | Combo finisher — §2 Part Four |
| **Auto-succeed** on one saving throw or check | **40** | Any time |
| **Activate a clan bloodline ability** | **40–60** | Per the clan entry, Part Four |
| **Perfect Strike** — the action is an automatic critical hit | **60** | Combo finisher — §2 Part Four |
| **Bloodline awakening** (story moment) | **100** (full bar) | Once, narratively |
| **SIGNATURE TECHNIQUE** — auto-hit, auto-crit, maximum damage, described your way | **100** (full bar) | Combo finisher — §2 Part Four |

**[RESOLVED — was a live contradiction.]** Two overlapping menus previously existed: this section listed *"add +1 damage die = 20"* while §2 Part Four listed *"Heavy Strike, +2 damage dice = 20"* — same price, different product. **§2's version wins** (it is the combat-authoritative section, and Book 0 already propagated it), and the two menus are merged above. The §1-only entries — ignore a cost, auto-succeed a save — are preserved and priced against their neighbours.

##### ⚠ SPEND LIMITS **[GM — REPAIRED. The menu had no limits of any kind.]**

> **The exploit:** nothing said how *often* any row could be bought. A five-action combo generated **+30 Special a round** (+5 round start, +5 per hit) — more with crits, more again for taking a heavy hit or dropping an enemy. **Extension costs 40 and adds an action, and that action generates another +5.** The loop paid for itself, and *"Heavy Strike"* could in principle be purchased once per action.

| Limit | Rule |
|---|---|
| **Special gain per round** | **Capped at +40.** Beyond that the bar does not fill, however good the round was |
| **Finishers** | **One per combo.** *Heavy Strike · Unavoidable · Extension · Perfect Strike · Signature Technique* are marked *"Combo finisher"* and only one may be bought in a single combo |
| **Extension** | **Once per combat**, not once per combo. It exists for the moment a fight turns, not as a per-round tax |
| **Ignore a cost · Auto-succeed a save · Push through an interruption** | **Once per round each.** These are not finishers and may be used mid-combo |
| **Bloodline awakening · Signature Technique (100)** | Full bar. **Unchanged** — spending everything you have should stay spectacular |

**Design note:** the Special bar is where the genre lives. Naruto fights turn on someone finding a second wind at the worst possible moment. **Be generous with gains during dramatic beats and let players cash out spectacularly** — the limits above exist to stop the bar becoming an engine, not to stop it becoming a moment.

---

#### Attributes **[SHEET]**

Six attributes, base 10, modifier +0 at start.

| Attribute | Governs |
|---|---|
| **Strength** | Taijutsu power, physical force |
| **Dexterity** | Agility, reflexes, hand seals, stealth |
| **Constitution** | Health, endurance, chakra reserves |
| **Intelligence** | Ninjutsu knowledge, analysis, strategy |
| **Wisdom** | Perception, insight, sensory ability |
| **Charisma** | Leadership, willpower, genjutsu resistance |

Note **Dexterity governs hand seals** — a bound or injured shinobi is in real trouble. And **Charisma is genjutsu resistance**, not just social ability, which makes it far more load-bearing than in standard 5e.

#### Skills **[SHEET]**

Twelve skills, each with a proficiency toggle and a modifier.

| Skill | Governing attribute **[INF]** |
|---|---|
| **Taijutsu** | STR or DEX (player's choice, locked at creation) |
| **Ninjutsu** | INT |
| **Genjutsu** | CHA |
| **Kenjutsu** | DEX |
| **Shurikenjutsu** | DEX |
| **Sensor Skills** | WIS |
| **Stealth** | DEX |
| **Medical Ninjutsu** | WIS |
| **Summoning** | CHA |
| **Intimidation** | CHA |
| **Persuasion** | CHA |
| **Strategy** | INT |

**Skill modifier = governing attribute modifier + proficiency bonus (if proficient).**

#### Vitals **[SHEET]**

| Stat | Starting value |
|---|---|
| **Health** | 30 / 30 |
| **Defense (AC)** | 10 + DEX modifier |
| **Initiative** | +0 (DEX modifier) |
| **Movement** | 30 ft |

#### Proficiency Bonus **[GM — REPAIRED. This was referenced three times and never defined.]**

> **⚠ Every save DC and every skill check in this system depends on this number, and no table for it existed.** The value below is the one the campaign has been using in practice (Ardo, Suzume and Souji all sit at **+5** at Level 13) — it is now written down.

| Level | Rank band | Proficiency |
|---|---|---:|
| **1–4** | Genin | **+2** |
| **5–8** | Chūnin | **+3** |
| **9–12** | Jōnin | **+4** |
| **13–16** | Jōnin (13) → S-Rank | **+5** |
| **17–20** | S-Rank (17) → Kage | **+6** |

#### Technique DCs

**DC = 8 + proficiency bonus + governing attribute modifier**

| Discipline | Governing attribute |
|---|---|
| Ninjutsu DC | INT |
| Genjutsu DC | CHA |
| Taijutsu DC | STR or DEX |
| Medical DC | WIS |

#### Rank Progression **[SHEET]**

**Genin → Chūnin → Jōnin → S-Rank → Kage**
*"Complete missions, gain experience, and prove yourself. Your path is in your hands."*

#### Experience **[SHEET]**

The XP track runs **0 → 25 → 50 → 75 → 100 → Next Level**. One hundred points per level, marked in quarters.

##### Suggested XP awards **[GM]**

| Event | XP |
|---|---|
| Completing a D-rank mission | 15–25 |
| Completing a C-rank mission | 30–40 |
| Completing a B-rank mission | 50–60 |
| Completing an A-rank mission | 75–90 |
| Completing an S-rank mission | 100 |
| Defeating a notable enemy | 10–25 |
| A major story beat or personal breakthrough | 25 |
| Excellent roleplay or a clever solution | 5–15 |

At these rates a squad levels roughly every two to four sessions, which suits the genre's fast early growth.

---
---

### PART TWO — CHARACTER CREATION

The Body Origin sheet is labeled **"Step 2 of 6."** The full sequence, reconstructed: **[INF except where noted]**

##### Step 1 — Attributes
Assign your six attribute scores. Track **Attribute Points Remaining** on the sheet. **[SHEET]**

##### Step 2 — Body Origin **[SHEET]**
See Part Three.

##### Step 3 — Clan / Bloodline **[SHEET]**
See Part Four. Record **Clan, Clan Rarity, and Clan Ability** on the sheet.

##### Step 4 — Nature Affinity **[SHEET]**
Choose from **Wind (風), Fire (火), Water (水), Lightning (雷), Earth (土)**. Genin begin with one. Affinity gates access to elemental jutsu — the Genin Ability sheet lists *"Lightning Release Affinity"* and *"Fire Release Affinity"* as hard requirements.

##### Step 5 — Specialty & Skills **[SHEET]**
Record your **Specialty** and allocate **Skill Points**.

##### Step 6 — Jutsu, Equipment & Backstory **[SHEET]**
Fill in **Known Jutsu** (Rank / Type / Cost), **Clan Bloodline Ability** (Cost), **Passive Abilities**, **Equipment**, **Weapons** (Damage / Type), and **Notes & Backstory**.

---
---

### PART THREE — BODY ORIGIN **[SHEET]**

*"Choose the lineage that flows through your body. This choice shapes your natural reserves and path as a shinobi."*

Every character descends from one of the Sage of Six Paths' two sons. This is the system's first real fork.

#### Body of Indra
*The path of genius, talent, and overwhelming chakra.*

| | |
|---|---|
| **Bonuses** | +30 Chakra · −15 Stamina · +1 Intelligence · +1 Ninjutsu Skill |
| **Starting resources** | Chakra **130** · Stamina **85** · Special 0 |
| **Passive — Natural Chakra Control** | The first Ninjutsu you use each combat costs **2 less Chakra** (minimum cost 1) |
| **Playstyle** | Excels at elemental ninjutsu, genjutsu, and high-chakra techniques. Casts more jutsu early but tires quickly in prolonged physical fights. |

#### Body of Ashura
*The path of endurance, resilience, and overwhelming life force.*

| | |
|---|---|
| **Bonuses** | +30 Stamina · −15 Chakra · +1 Constitution · +1 Taijutsu Skill |
| **Starting resources** | Chakra **85** · Stamina **130** · Special 0 |
| **Passive — Powerful Life Force** | Recover **5 Stamina at the start of each combat round** |
| **Playstyle** | Excels at taijutsu, weapon combat, long battles, and taking punishment. Fights far longer but has fewer reserves for powerful jutsu. |

> *"Indra sought power through the eyes. Ashura sought strength through the body."*

**Reading the bars [INF]:** the sheets display both resources on a shared 0–130 scale. The practical reading is that base is **100/100**, the +30 raises that resource's maximum to 130, and the −15 lowers the other to 85. Indra's stamina caps at 85; Ashura's chakra caps at 85.

**Narrative weight:** this choice is also the Indra/Asura reincarnation cycle from **Book I §1**. A player who picks Body of Indra has, at minimum, thematic company with the Uchiha line. Whether that's literal in your campaign is a fine thing to leave ambiguous for twenty sessions.

---
---

### PART FOUR — CLANS & BLOODLINES **[SHEET]**

Three rarity tiers. **Rarity is difficulty, not power ceiling.**

| Rarity | Difficulty | Meaning |
|---|---|---|
| **Common** | ★☆☆☆☆ | Easier training, techniques unlock early |
| **Rare** | ★★★☆☆ | Requires additional training and dedication |
| **Legendary** | ★★★★☆ | Locked behind major story arcs and life-changing events |

#### Common Clans

| Clan | Stat Bonuses | Passive Ability |
|---|---|---|
| **Nara** | +2 INT, +1 WIS | Advantage on tactical planning and investigation checks |
| **Akimichi** | +2 STR, +1 CON | Carry twice normal weight; resist forced movement |
| **Yamanaka** | +2 WIS, +1 CHA | Advantage on Insight and mental resistance checks |
| **Aburame** | +2 WIS, +1 CON | Insects provide tremor sense within 15 ft; resist poison |
| **Inuzuka** | +2 DEX, +1 CON | Heightened smell grants advantage on tracking |
| **Sarutobi** | +1 STR, +1 INT, +1 WIS | Learn elemental ninjutsu 25% faster than others |
| **Hatake** | +2 DEX, +1 INT | +10 ft movement while wearing light armor |
| **Shimura** | +2 INT, +1 CON | Advantage on Stealth while hidden; resistance to fear |
| **Puppet Master** | +2 INT, +1 DEX | Begin play with a basic combat puppet |
| **Kamizuru** | +2 WIS, +1 DEX | Bee summons grant advantage on Survival and tracking |
| **Fūma** | +2 DEX, +1 STR | Proficiency with all thrown weapons and ninja tools |

#### Rare Clans

| Clan | Stat Bonuses | Passive Ability |
|---|---|---|
| **Uchiha** | +2 INT, +1 DEX | Advantage on sight-based Perception. **Unlocks Sharingan progression.** |
| **Hyūga** | +2 WIS, +1 DEX | Byakugan grants enhanced vision and **+2 Initiative** |
| **Hōzuki** | +2 DEX, +1 CON | Partial liquefaction reduces non-elemental weapon damage |
| **Kaguya** | +2 STR, +1 CON | Natural Bone Armor increases **AC by +1** |
| **Yuki** | +2 INT, +1 WIS | Ice Release techniques cost **1 less Chakra** |
| **Hoshigaki** | +2 STR, +1 CON | Breathe underwater; swim at full movement |
| **Karatachi** | +2 CON, +1 WIS | Strong Water affinity grants resistance to water techniques |
| **Yōtsuki** | +2 STR, +1 DEX | +10 ft movement; resistance to lightning damage |
| **Magnet Release** | +2 INT, +1 WIS | Resistance to metal weapons; **unlocks Magnet Release** |
| **Storm Release** | +2 INT, +1 WIS | Storm Release techniques ignore half cover |
| **Explosion Release** | +2 STR, +1 INT | Explosive techniques ignore resistance to fire damage |
| **Kurama** | +2 CHA, +1 INT | **Genjutsu save DC increases by +2** |
| **Iburi** | +2 DEX, +1 CON | Smoke Form usable once per short rest |

#### Legendary Clans

| Clan | Stat Bonuses | Passive Ability |
|---|---|---|
| **Senju** | +2 CON, +1 STR | **Mastery of the Earth** — regain an additional **25% of maximum Health** on a long rest; and **once per long rest**, a full round of genuine stillness (no other action) restores **20 Stamina / 10 Chakra** outside normal rest **[GM — restated; see note below]** |
| **Uzumaki** | +2 CON, +1 CHA | **+25% Chakra Pool**; advantage against sealing effects |
| **Hagoromo** | +2 STR, +1 WIS | Once per long rest, reduce incoming damage by half |
| **Chinoike** | +2 WIS, +1 INT | Unlocks **Ketsuryūgan** progression |
| **Jūgo** | +2 STR, +1 CON | Passively regenerate a small amount of HP each combat |
| **Dust Release Bloodline** | +2 INT, +1 WIS | Dust Release deals bonus damage to constructs and barriers |
| **Kazekage Bloodline** | +2 WIS, +1 CON | Natural Sand Shield grants **+1 AC while conscious** |

> **[RESOLVED — dangling 5e artifact.]** The Senju row previously read *"Recover extra HP whenever spending Hit Dice during a rest."* **This system has no Hit Dice** — it runs Chakra / Stamina / Health with percentage recovery per rest (Part Six). The trait is restated above in this system's own terms, and folded together with **Mastery of the Earth**, the version already established in play on `characters/souji.md`. Souji's sheet is no longer an override; it now matches the printed clan trait.

#### Clanless Shinobi **[SHEET]**

| | |
|---|---|
| **Bonus** | +1 to any ability score of your choice |
| **Extra** | One additional starting **feat** and one additional starting **jutsu** |
| **Limit** | Cannot naturally learn Kekkei Genkai or clan-exclusive jutsu |
| **Strength** | Excel at general shinobi training; grow quickly through determination |

**This is a genuinely competitive option, not a consolation prize.** An extra feat and extra jutsu at level 1 is a real head start, and it maps directly onto the setting's central argument — Naruto, Rock Lee, and Might Gai are all clanless.

#### Bloodline Awakening & Progression **[SHEET]**

> *"A powerful bloodline is not a reward for choosing a clan — it is a reward for surviving the journey."*

Choosing a Rare or Legendary clan does **not** grant immediate access to its strongest abilities. To awaken advanced bloodline powers a character must:

1. **Reach the required level**
2. **Complete specialized training**
3. **Fulfill story requirements**
4. **Receive DM approval for major awakenings**

##### Progression chains **[SHEET]**

| Base | → | Advanced | → | Peak |
|---|---|---|---|---|
| Sharingan | → | Mangekyō Sharingan | → | Eternal Mangekyō |
| Byakugan | → | Advanced Byakugan Techniques | | |
| Wood Release | → | True Wood Release | | |
| Chakra Chains | → | Adamantine Sealing Chains | | |
| Dust Release | → | Complete Particle Style | | |
| Sage Transformation | → | Perfect Sage Mode | | |
| Eight Trigrams | → | Eight Trigrams Secret Techniques | | |

##### The cost of Legendary bloodlines **[SHEET]**

Legendary bloodlines are nearly extinct for a reason. Unlocking true potential often requires:
- **Life-threatening experiences**
- **Ancient relics or forbidden scrolls**
- **Legendary mentors**
- **Sacrifices and consequences**

**GM note:** every item on that list is an adventure. Treat a player's awakening requirement as a mission hook, not a checkbox — see **Book IV §5**.

---
---

### PART FIVE — ABILITY FORMAT **[SHEET]**

Every technique is written with five fields:

| Field | Meaning |
|---|---|
| **Chakra Cost** | Chakra required to perform the ability |
| **Stamina Cost** | Physical exertion required |
| **Action Cost** | Action, Bonus Action, or Reaction |
| **Requirements** | Rank, stats, clan, affinity, or situational conditions |
| **Effect** | What it does, plus bullets for limitations and riders |

#### The Genin Ability Set **[SHEET]**

##### Academy Jutsu — E Rank

| Technique | Chakra | Stamina | Action | Requirements |
|---|---|---|---|---|
| **Clone Technique** (Bunshin no Jutsu) | 5 | 0 | 1 Action | Academy Graduate |
| **Transformation Technique** (Henge no Jutsu) | 4 | 0 | Bonus Action | Academy Graduate |
| **Substitution Technique** (Kawarimi no Jutsu) | 8 | 5 | **Reaction** | Nearby object (log, rock, barrel) |
| **Rope Escape Technique** (Nawa Nobori no Jutsu) | 3 | 2 | Bonus Action | Rope bindings or restraints |

**Clone Technique.** Creates up to 3 illusionary copies. Clones cannot attack, cannot take damage, and vanish on contact. Grants advantage on one Deception or Performance check involving visual trickery.

**Transformation Technique.** Transform into another person or object of similar size. **Maintain: 1 Chakra each round.** Ends if you attack, take damage, or someone succeeds on an Investigation check against your Ninjutsu DC.

**Substitution Technique.** When targeted by an attack, teleport to an unoccupied space within 15 ft and replace yourself with a nearby object. **Cannot be used against area attacks. Usable once per round.**

**Rope Escape Technique.** Attempt to escape ropes or basic restraints, rolling with advantage against non-chakra restraints. **Does not work on chakra-based seals or advanced bindings.**

##### D Rank

| Technique | Chakra | Stamina | Action | Requirements |
|---|---|---|---|---|
| **Body Flicker (Basic)** (Shunshin no Jutsu) | 8 | 6 | Bonus Action | Academy Graduate |
| **Flash Step** (Hikari no Jutsu) | 10 | 5 | Bonus Action | Academy Graduate |
| **Water Walking Technique** (Mizu Watari no Jutsu) | 10 | 5 | Action | Water surface nearby |
| **Leaf Whirlwind** (Konoha Senpuu) | 12 | 5 | Action | Academy Graduate |
| **Lightning Blade** (Raikiri no Jutsu) | 12 | 5 | Action | **Lightning Release Affinity** |
| **Fire Release: Fireball** (Housenka no Jutsu) | 12 | 5 | Action | **Fire Release Affinity** |

**Body Flicker (Basic).** Move up to your movement speed without provoking opportunity attacks. **Cannot attack the same turn** unless a feature allows it.

**Flash Step.** Move up to 30 ft in a straight line. Does not provoke opportunity attacks. Cannot end movement in an occupied space.

**Water Walking Technique.** Walk on water surfaces for up to 1 minute. Ends if you take damage. Heavy armor or over-encumbrance prevents use.

**Leaf Whirlwind.** A swirl of wind and leaves in a **15 ft radius**. Creatures in the area must succeed a DEX save or take damage and be pushed back 10 ft.

**Lightning Blade.** Shape a current of lightning in your hand or weapon. Your next weapon attack this turn gains extra Lightning damage.

**Fire Release: Fireball.** Ranged attack up to **60 ft**. On hit: Fire damage, and the target may be ignited.

#### General Notes **[SHEET]**

- **Genin Level.** These abilities represent what a shinobi can learn right after graduating the Academy.
- **Costs.** Chakra and Stamina costs **may increase if techniques are overused or performed in extreme conditions.**
- **Actions.** Action economy is vital. Use Bonus Actions and Reactions wisely.
- **Upgrades.** As rank and experience grow, these jutsu can be improved or evolved into more powerful versions. → **Fully expanded in Book IV §3: Jutsu Mastery & Creation.**
- **Rule of Balance.** *A true shinobi knows that intelligence, timing, and teamwork are just as important as power.*

> *"Talent may open the door, but dedication and discipline are what make a true shinobi."*

---

#### [CONFLICT] — Genin sheet vs. Jutsu Compendium

Three techniques on the Genin sheet carry names or ranks that disagree with the Jutsu Compendium. **Flagged, not resolved.**

| Genin sheet | Jutsu Compendium | Nature of the conflict |
|---|---|---|
| **Lightning Blade** (Raikiri no Jutsu) — **D rank** | **Lightning Cutter** (Raikiri, 雷切) — **S rank** | Same Japanese name, six rank steps apart. Kakashi's signature technique is S-rank in the compendium and an Academy-adjacent D-rank here. |
| **Fire Release: Fireball** (Housenka no Jutsu) — **D rank** | **Fire Release: Phoenix Sage Fire Technique** (Hōsenka, 鳳仙火) — **C rank** | Same technique name, different English gloss, one rank step apart. |
| **Flash Step** (Hikari no Jutsu), **Water Walking Technique** (Mizu Watari no Jutsu) | *Not present* | System-original techniques with no compendium entry. |

**Suggested resolutions — pick one at session zero:**
- **A. Sheet wins.** These are the *beginner* forms; the compendium entries are the mature versions, unlocked through the Upgrades rule. Rename the D-rank version (e.g. "Lightning Current") to keep both.
- **B. Compendium wins.** Rerank the sheet entries and swap in genuine D-rank alternatives from the D-Rank file (Decapitating Airwaves, Leaf Gale, Dynamic Entry).
- **C. Split the difference.** Keep the sheet costs, adopt the compendium names, and treat rank as a *narrative* label rather than a power tier.

Option A best fits the sheet's own **"Upgrades"** note and is the recommended default.

---
---

### PART SIX — COMBAT

#### The Combo System **[SHEET]**

> *A combo is a sequence of up to 3 actions (attacks or jutsu) performed during your Action. You may mix any eligible abilities as long as you have the required Chakra and/or Stamina. After your combo, you still have your Bonus Action and Reaction.*

##### Combo I — Single Strike
Make 1 attack or use 1 jutsu. Counts as your Action.
*Examples: Punch, Kick, Throw Kunai, Fireball Jutsu, Body Flicker.*

##### Combo II — Three-Strike Combo
Make up to 3 actions in sequence. Counts as your Action. Mix any eligible abilities. Pay the Chakra and/or Stamina cost for **each** ability.
*Example: Punch → Kick → Throw Kunai.*

##### The Five Combo Rules **[SHEET]**

1. **Up to 3 Actions.** Your combo can include up to 3 actions of your choice.
2. **Mix Freely.** Mix any attacks and jutsu as long as each counts as 1 Action.
3. **Pay Costs.** Pay the full Chakra and/or Stamina cost for each ability used.
4. **Within Limits.** You cannot exceed 3 actions. After the combo ends, your Action is used.
5. **Counters & Interruption.** If the combo is interrupted — stunned, knocked down, silenced — **remaining actions are lost.**

##### Reference **[SHEET]**

| | |
|---|---|
| Max actions in combo | **3** |
| Uses your Action | Yes |
| Bonus Action after | **Yes** |
| Reaction after | **Yes** |
| Includes Jutsu | Yes |
| Must pay costs | Yes |

##### Sample combos **[SHEET]**

| Type | Sequence |
|---|---|
| **Taijutsu** | Punch → Kick → Elbow |
| **Ninjutsu** | Fireball Jutsu → Shadow Clone Jutsu → Chidori |
| **Mixed** | Throw Kunai → Body Flicker → Water Dragon Jutsu |

> *"Strength isn't just power... it's how you combine it."*

##### Why Rule 5 is the balancing mechanism
The combo system is enormously generous — three full actions plus a bonus action plus a reaction, every turn. **The governor is Rule 5.** Any control effect that lands mid-combo deletes the rest of it. This means:

- **Stun, prone, and silence effects are worth far more than their damage suggests.** Prioritize them.
- **Going second in initiative is dangerous** in a way it isn't in standard 5e.
- **Resource drain is the real limiter.** A full three-jutsu combo at D-rank costs ~32 Chakra and ~16 Stamina. A genin can do that three times before they're empty.

##### Combo scaling by rank — see Book IV §2

The printed 3-action cap is the **Genin** limit. It grows by one action per rank:

| Rank | Combo Limit |
|---|---|
| Academy | 1 |
| **Genin** | **3** **[SHEET]** |
| Chūnin | 4 |
| Jōnin | 5 |
| S-Rank | 6 |
| Kage | 7 |

**Book IV §2 — Advanced Combat & Combo Mastery** carries the full expansion: Action Weight (higher-rank techniques consume multiple combo slots), Chain Momentum, Openings, Combo Finishers, **the Counter Window and Clash system**, escape assets, team combos, and elemental chaining.

**Two rules from Book IV §2 you should adopt immediately, at any rank:**
- **Reactions are usable at any moment**, including mid-combo against any single action — that is what Substitution is for **[SHEET]**. But it's **one per round**, and escaping requires a jutsu, clan ability, ninja tool, or feature. With an empty kit, the only option is Brace.
- **When the first action of a combo misses, the defender may spend their Reaction to cast a jutsu.** If it meets the attacker's next action, they **clash**.

---

#### Resource Depletion **[INF — the sheets track the bars but don't define empty]**

| Condition | Effect |
|---|---|
| **Chakra at 25% or less** | Disadvantage on Ninjutsu and Genjutsu attack rolls |
| **Chakra at 0** | Cannot use Chakra abilities. You may spend **2 Health per 1 Chakra** — this is how shinobi die. |
| **Stamina at 25% or less** | Movement reduced by 10 ft; disadvantage on DEX saves |
| **Stamina at 0** | Cannot use Taijutsu, dodge, or block. Movement halved. |
| **Both at 0** | Unconscious at the end of your next turn unless you receive aid |

#### Recovery **[INF]**

| Rest | Recovery |
|---|---|
| **Short rest (1 hour)** | Regain 25% of max Chakra and Stamina |
| **Long rest (8 hours)** | Full Chakra and Stamina |
| **Soldier pill** | +40 Chakra immediately; **−20 max Chakra until a long rest** |
| **Ashura passive** | +5 Stamina at the start of each combat round **[SHEET]** |

#### Overuse and Extreme Conditions **[SHEET, expanded [GM]]**

The sheet states costs *"may increase if techniques are overused or performed in extreme conditions."* Suggested implementation:

| Situation | Cost adjustment |
|---|---|
| Third+ use of the **same** jutsu in one combat | +50% Chakra |
| Casting in hostile terrain (Water jutsu in desert, Fire in heavy rain) | +50% Chakra |
| Casting while below 25% in either resource | +25% both |
| Casting in favorable terrain (Water beside a lake, Fire in dry forest) | **−25% Chakra** |

This one rule does more to make terrain matter than any amount of description. See **Book I §2** for terrain profiles.

---
---

### PART SEVEN — SCALING BEYOND GENIN **[INF / GM]**

The sheets define Genin precisely and stop. Everything in this part is extrapolation built to remain consistent with the printed numbers.

#### Resource Growth

**Chakra Max = 100 + (20 × [Level − 1]) + (10 × CON modifier)**
**Stamina Max = 100 + (20 × [Level − 1]) + (10 × CON modifier)**
**Health = 30 + (10 × [Level − 1]) + (2 × CON modifier × Level)**

*At Level 1 with CON +0 this produces exactly 100 / 100 / 30 — matching the sheet.*
Apply Body Origin (+30 / −15) and Uzumaki (+25% Chakra) on top.

| Level | Rank | Chakra & Stamina (CON +0) | Health |
|---|---|---|---|
| 1 | Genin | 100 | 30 |
| 4 | Genin | 160 | 60 |
| 5 | Chūnin | 180 | 70 |
| 8 | Chūnin | 240 | 100 |
| 9 | Jōnin | 260 | 110 |
| 13 | Jōnin | 340 | 150 |
| 14 | S-Rank | 360 | 160 |
| 17 | S-Rank | 420 | 190 |
| 18 | Kage | 440 | 200 |
| 20 | Kage | 480 | 220 |

#### Rank by Level

| Rank | Levels | Max jutsu rank |
|---|---|---|
| **Genin** | 1–4 | D |
| **Chūnin** | 5–8 | C |
| **Jōnin** | 9–13 | B, and one A-rank signature |
| **S-Rank** | 14–17 | A, and one S-rank signature |
| **Kage** | 18–20 | S |

#### ADVANCEMENT BY LEVEL **[GM — REPAIRED. Fixes fifteen dead levels.]**

> **⚠ The problem this fixes.** Progression was **rank-band only**. A character levelling from 2 to 3, or 10 to 11, gained **+20 Chakra, +20 Stamina, +10 Health and nothing else** — no feature, no decision, no reason to look forward to it. **Eleven of twenty levels handed the player a number and nothing to do with it.**
>
> Every level below now gives something. **Nothing here raises raw output** beyond what the resource formulas already grant; the additions are *choices, slots and permissions.*

| Lvl | Rank | What you gain |
|---:|---|---|
| **1** | Genin | Body Origin · Clan or **Clanless** (extra feat + extra jutsu) · Nature Affinity · **3 combo slots** · the Genin ability set |
| **2** | Genin | **+1 technique** (E or D) · Mastery XP begins tracking (Book IV §3) |
| **3** | Genin | **Feat, or +2 to one attribute / +1 to two** |
| **4** | Genin | **+1 technique** · begin training a second nature affinity *(not yet usable)* |
| **5** | **CHŪNIN** | **4th combo slot** · **C-rank unlocked** · proficiency **+3** |
| **6** | Chūnin | **+1 technique** (up to C) · **first Acceleration** becomes purchasable with Mastery |
| **7** | Chūnin | **Feat or attribute increase** |
| **8** | Chūnin | **Declare a Signature Technique** — one technique you own permanently gains **+1 to its attack roll and its save DC** |
| **9** | **JŌNIN** | **5th combo slot** · **B-rank unlocked, plus one A-rank signature** · proficiency **+4** |
| **10** | Jōnin | **+1 technique** · **second nature affinity unlocked** and usable |
| **11** | Jōnin | **Feat or attribute increase** |
| **12** | Jōnin | **Second Wind** — once per combat, regain your Reaction after spending it |
| **13** | Jōnin | Proficiency **+5** · **second Acceleration** becomes purchasable |
| **14** | **S-RANK** | **6th combo slot** · **A-rank unlocked, plus one S-rank signature** |
| **15** | S-Rank | **Feat or attribute increase** |
| **16** | S-Rank | **Kinjutsu access** — you may learn forbidden techniques, and you pay their permanent costs |
| **17** | S-Rank | Proficiency **+6** · **Signature Technique II** — your signature's bonus rises to **+2** |
| **18** | **KAGE** | **7th combo slot** · **S-rank unrestricted** |
| **19** | Kage | **Feat or attribute increase** |
| **20** | Kage | **CAPSTONE — choose one:** a permanent **second Reaction each round** · one owned technique becomes **Perfected** at no XP cost · or an **8th combo slot** |

> **Attribute increases follow the standard rule:** +2 to one attribute or +1 to two, maximum 20 in any attribute. A character may always take a feat instead.
>
> **[SHEET] fidelity:** Levels 1–4 remain exactly the printed Genin experience. Everything from 5 up is **[GM]** extrapolation built to stay inside the printed bands.

#### Cost by Jutsu Rank

Extrapolated from the printed E and D values (E: 3–8 Chakra / 0–5 Stamina; D: 8–12 Chakra / 5–8 Stamina). *(The D Stamina band reads 5–8 here and in every table below; an earlier draft of this line said 5–6, which no printed technique actually respects — Body Flicker is 8/6 and Gale Fist is 10/6.)*

| Rank | Chakra | Stamina | Notes |
|---|---|---|---|
| **E** | 3–8 | 0–5 | **[SHEET]** |
| **D** | 8–12 | 5–8 | **[SHEET]** |
| **C** | 15–25 | 8–14 | |
| **B** | 30–45 | 15–22 | |
| **A** | 50–70 | 25–35 | |
| **S** | 80–110 | 40–55 | Usually one per fight |
| **Kinjutsu** | 80+ | 40+ | **Plus a permanent cost** — see below |

**Sanity check:** a Level 20 Kage with 480 Chakra can throw four to six S-rank techniques in a battle. That's right for the genre.

#### Kinjutsu **[GM]**

Forbidden techniques cost Chakra, Stamina, **and something you don't get back.**

| Kinjutsu | Additional cost |
|---|---|
| **Multiple Shadow Clone** | Chakra is **divided** among clones; drop to 0 and you fall unconscious 1d4 hours |
| **Eight Gates (per gate)** | See below |
| **Impure World Reincarnation** | A living sacrifice per reanimation |
| **Dead Demon Consuming Seal** | **The user dies.** Always. |
| **One's Own Life Reincarnation** | The user's life for the target's |
| **Cursed Seal application** | Target rolls a CON save; on failure, **they die** |

#### The Eight Gates **[GM]**

Opening a gate is a **Bonus Action**. Gates stay open until combat ends or you drop.

| Gate | Level | Benefit | Cost when combat ends |
|---|---|---|---|
| 1 — Opening | 5 | +2 STR/DEX; +10 ft movement | 25% max Stamina |
| 2 — Healing | 7 | Regain 25% Health on opening | 50% max Stamina |
| 3 — Life | 9 | +1 action to your combo limit (4 total) | Stamina to 0 |
| 4 — Pain | 11 | Advantage on all attacks | Stamina to 0; lose 25% max Health |
| 5 — Limit | 13 | Double all Taijutsu damage dice | Unconscious 1d4 hours |
| 6 — View | 15 | Attacks bypass resistance and immunity | Unconscious 1d4 days |
| 7 — Wonder | 17 | +4 AC; +1 more combo action (5 total) | Unconscious 1 week; **permanent −2 CON** |
| 8 — Death | 19 | All attacks automatically hit and crit | **You die when combat ends. No save.** |

**Gates 3 and 7 interacting with the combo system is the point.** A Gate-7 taijutsu specialist making five actions per turn is the most terrifying thing in the game, and they get one fight to be it.

#### Dōjutsu **[GM, following the sheet's progression chain]**

**Sharingan** (Uchiha, Rare — the sheet grants *"Sharingan progression"* at creation):

| Stage | Unlock | Effect | Upkeep |
|---|---|---|---|
| **1 tomoe** | Level 3 + trauma trigger | Advantage vs. Genjutsu; read hand seals | 2 Chakra/round |
| **2 tomoe** | Level 6 or second trigger | Reaction: impose disadvantage on one attack | 3 Chakra/round |
| **3 tomoe** | Level 9 | **Copy a witnessed jutsu** (Ninjutsu check, DC 10 + 2 per rank step). Cannot copy Kekkei Genkai or hiden. | 4 Chakra/round |
| **Mangekyō** | Level 14 + **the death of someone loved**, played out in-fiction | One unique technique, DM-designed. Costs **Special**, not Chakra. | 8 Chakra/round |
| **Eternal Mangekyō** | Level 18 + transplant from a relative | Removes the Vision cost entirely | 8 Chakra/round |

**Vision track:** a Mangekyō user starts at **10 Vision**. Each Mangekyō technique use costs 1. At 5, disadvantage on ranged attacks and sight-based Perception. **At 0, permanently blind.** Track it on the sheet under Passive Abilities where the player can see it.

**Byakugan** (Hyūga, Rare) — active from creation per the sheet: enhanced vision and **+2 Initiative**. Advanced Byakugan Techniques unlock through the sheet's progression requirements.

#### Jinchūriki **[GM]** — *delegated in full to Book II §3 Part Five*

Not on any sheet. **Book IV does not define jinchūriki mechanics; Book II §3 Part Five does, and it is authoritative for all of them** — the baseline package, the cloak table, the tail thresholds, and the partnership arc.

Headlines only, so you know what you are agreeing to before you allow one:

- **Chakra pool doubled**, on top of everything else.
- **Regenerate 5 Health at the start of each combat round.**
- The tailed beast is an **NPC the player negotiates with**, not a resource.
- **Tailed Beast Cloak costs Special, not Chakra.** A player may voluntarily reach **two tails**. Past that is not a choice — it is a failed save.

> **[RESOLVED — was a live contradiction.]** This section previously read *"three or more tails… the DM takes the character,"* while Book II §3 Part Five puts three tails still in the player's hands (damage, and the save DC rising to 17) and hands control to the DM only at **four**. **Book II wins** — it is the specific, complete treatment, and the three-tail stage exists precisely so a player feels the slide before losing the wheel. Book IV no longer states thresholds of its own.

See **Book II §3** for the full table and the partnership arc.

---
---

### PART EIGHT — NPCS DO NOT FOLLOW THESE RULES **[SHEET]**

This is printed guidance and it is the most important rule in the system.

> *The shinobi world is unpredictable. Not every NPC or enemy you face will follow the same rules as player characters. Their actions, abilities, and resources may reflect their situation, rank, experience, or importance to the story.*

> **DO NOT GET DISCOURAGED** if you can't keep up with higher-ranked enemies or NPCs. **They are not bound by the same limits you are.**

##### What this means **[SHEET]**

| Principle | Meaning |
|---|---|
| **Higher Rank = Greater Threats** | Jōnin, ANBU, Kage, and legendary shinobi may have stronger jutsu, better gear, and unique advantages |
| **Situation Matters** | Reinforcements, terrain, intel, clan advantages, and objectives can all shift the balance |
| **Story Comes First** | Some enemies are designed to challenge, delay, test, or teach — **not always to be defeated** |
| **Know When to Fight... and When to Live** | **Retreat is not failure. Survival is a victory of its own.** |

> *"The ninja world doesn't play fair. Adapt. Survive. Write your legend."*

**This rule resolves the setting's biggest design problem.** Minato, Itachi, Hanzō, and Madara do not need balanced stat blocks — they need to be *correct*, and the players need to know in advance that beating them isn't the assignment. **Book IV §4** is built entirely on this principle.

**Tell your players this at session zero.** The printed warning exists because a party that doesn't know the rules are asymmetric will read a losing fight as a DM being unfair, rather than as the genre working exactly as intended.


---
---

# §2 — ADVANCED COMBAT & COMBO MASTERY

An expansion of the Combo System. The base rules are on the Combo System sheet and in **Book IV §1, Part Six**; this file scales them across the full rank ladder and adds the depth that makes high-rank combat feel different from low-rank combat rather than just bigger.

**Sourcing:** **[SHEET]** = printed on the Combo System sheet. Everything else is **[GM]** — built to extend the printed rules without contradicting them.

---
---

### PART ONE — COMBO PROGRESSION BY RANK

#### The Core Rule

> **Every rank you gain adds one action to your combo limit.**

The Combo System sheet caps a Genin at **3 actions**. That cap was never meant to hold for a Kage — the sheet's own **Upgrades** note says techniques "can be improved or evolved into more powerful versions" as rank grows. This is that, applied to action economy.

| Rank | Levels | Combo Limit | Combo Tier |
|---|---|---|---|
| **Academy Student** | 0 | **1 action** | — |
| **Genin** | 1–4 | **3 actions** **[SHEET]** | Combo I–II |
| **Chūnin** | 5–8 | **4 actions** | Combo III |
| **Jōnin** | 9–13 | **5 actions** | Combo IV |
| **S-Rank** | 14–17 | **6 actions** | Combo V |
| **Kage** | 18–20 | **7 actions** | Combo VI — *Flow State* |

**You still get your Bonus Action and Reaction after the combo, at every rank.** **[SHEET]**

#### Named Combo Tiers

| Tier | Actions | Unlocked at | Name |
|---|---|---|---|
| **Combo I** | 1 | Academy | **Single Strike** **[SHEET]** |
| **Combo II** | 3 | Genin | **Three-Strike Combo** **[SHEET]** |
| **Combo III** | 4 | Chūnin | **Broken Rhythm** |
| **Combo IV** | 5 | Jōnin | **Cascade** |
| **Combo V** | 6 | S-Rank | **Storm Chain** |
| **Combo VI** | 7 | Kage | **Flow State** |

Announcing the tier at the table is worth doing. A player hitting Jōnin and saying *"Cascade"* for the first time should feel like something.

#### Why this doesn't break the game

Three things self-limit a seven-action combo, and all three are already in your rules:

1. **Resources.** Seven A-rank techniques costs 350–490 Chakra. A Level 20 Kage has ~480 total. You get **one** of those per fight, and then you're empty.
2. **Rule 5 — Interruption.** **[SHEET]** A seven-action combo that gets stunned on action two loses five actions. The higher your ceiling, the more catastrophic a break becomes. High-rank combat is *more* fragile, not less.
3. **Action Weight.** See Part Two. Your best techniques eat multiple slots.

---
---

### PART TWO — ACTION WEIGHT

Without this, a Kage throws seven S-rank techniques. With it, they weave.

> **Your combo limit is a pool of slots, not a count of actions.** Each action spends slots based on its rank.

| Action | Slot Cost |
|---|---|
| Basic attack (unarmed, weapon, thrown) | **1** |
| **E-rank** technique | **1** |
| **D-rank** technique | **1** |
| **C-rank** technique | **2** |
| **B-rank** technique | **2** |
| **A-rank** technique | **3** |
| **S-rank** technique | **4** |
| **Kinjutsu** | **4+** (DM's call) |

#### What each rank can actually build

| Rank | Slots | Sample combos |
|---|---|---|
| **Genin** | 3 | Punch → Kick → Kunai · D-rank → D-rank → Punch · C-rank (2) → Punch |
| **Chūnin** | 4 | C-rank → C-rank · C-rank → Punch → Kick · B-rank (2) → D-rank → Punch |
| **Jōnin** | 5 | **A-rank (3) → Punch → Kick** · B-rank → B-rank → D-rank · B-rank → C-rank → Punch |
| **S-Rank** | 6 | **S-rank (4) → Punch → Kick** · A-rank → A-rank · A-rank → B-rank → D-rank |
| **Kage** | 7 | **S-rank (4) → A-rank (3)** · S-rank → B-rank → Punch · A-rank → A-rank → Punch |

That "**S-rank → A-rank**" line is the whole design goal. A Kage's turn should look like a Kage's turn.

#### Mastery reduces slot cost

The **Acceleration** upgrade in **Book IV §3** lowers a jutsu's slot cost by 1 per point, to a minimum of 1. This is the single most valuable thing mastery buys.

| Technique | Base slots | With 1 Acceleration | With 2 |
|---|---|---|---|
| C / B-rank | 2 | 1 | 1 |
| A-rank | 3 | 2 | 1 |
| S-rank | 4 | 3 | **2** |

A Kage with a Perfected, doubly-Accelerated S-rank technique can use it **twice in one combo**. That should take a campaign to earn — and it should feel like it when it lands.

> ## ⚠ THE APEX RULE **[GM — REPAIRED. Closes a real loophole.]**
>
> **The exploit:** a Kage has **7 slots.** A doubly-Accelerated S-rank costs **2.** That permits **three S-rank techniques plus a basic strike in a single combo** — 330 Chakra against a 480+ pool, with **no Repetition penalty at all** if they are three *different* S-ranks. The stated design goal one paragraph above is *"S-rank → A-rank."* The maths permitted triple.
>
> ### The rule
>
> **In one combo you may use at most TWO techniques of your rank band's maximum rank, and Acceleration never reduces this limit.**
>
> | Your rank | Maximum rank | Most you may fire in one combo |
> |---|---|---:|
> | Genin | D | **2** |
> | Chūnin | C | **2** |
> | Jōnin | B *(or your one A-signature)* | **2** |
> | S-Rank | A *(or your one S-signature)* | **2** |
> | Kage | S | **2** |
>
> **Acceleration still does exactly what it always did** — it frees slots for *everything else* in the combo. A Kage running S(2) → S(2) now spends four slots and has **three left for A-rank, B-rank and basics**, which is a genuinely better turn than the old triple-S and looks far more like the genre.
>
> **Why a cap rather than a cost:** raising the price would have been absorbed instantly by the Special menu's *"ignore the Chakra or Stamina cost"* row. **A slot cap cannot be bought off.**

#### The Repetition Rule

Using the **same technique twice in one combo** costs **+50% Chakra** on the repeat, and **+50% again** on a third use. This applies the sheet's printed **"costs may increase if techniques are overused"** rule directly to combos.

It doesn't forbid a double Rasengan. It just makes you pay for it.

---
---

### PART THREE — CHAIN MOMENTUM

The tension that makes a long combo a *decision* rather than a default.

#### Escalating Difficulty

| Action in sequence | Attack roll / Save DC modifier |
|---|---|
| 1st, 2nd, 3rd | **No penalty** |
| 4th | **−1** |
| 5th | **−2** |
| 6th | **−3** |
| 7th | **−4** |
| **8th and beyond** | **−5, and −1 more for every action after that** **[GM — REPAIRED]** |

The first three actions are always clean — a Genin's combo never suffers. The actions rank *grants* you are the ones that get shaky.

> **⚠ Why the 8th row exists.** The table stopped at 7 because 7 was a Kage's slot maximum — but **Extension** (Special menu, 40) adds an action *beyond* the combo limit and ignores slot cost, so 8, 9 and 10-action combos were reachable and **undefined**. They are defined now, and the penalty keeps growing, which is the point.

#### Building Momentum

**Each action in the combo that hits grants +2 damage to every subsequent action in that same combo, cumulatively.**

| Actions landed so far | Bonus damage on the next action |
|---|---|
| 1 | +2 |
| 2 | +4 |
| 3 | +6 |
| 4 | +8 |
| 5 | +10 |
| 6 | +12 |

**The result:** a long combo is harder to land but devastating if you're connecting. Missing early kills the payoff. This is why a Jōnin opens with a basic attack instead of leading with their strongest technique — you want the momentum built before the expensive action lands.

#### Openings

> **When a target fails a saving throw against one of your combo actions, they are Open until your combo ends.** Every remaining action in that combo has **advantage** against them.

This is the reward for sequencing. Lead with a control technique to force the save, then cash in. It's also why a Leaf Whirlwind (DEX save) makes such a good combo opener at low rank.

---
---

### PART FOUR — COMBO FINISHERS

Spend **Special** to end a combo with something the enemy can't answer. Declared before the final action resolves.

> **These are the combat rows of the master spend menu in §1 Part One.** That table is authoritative and also lists the non-finisher spends (pushing through an interruption, ignoring a cost, auto-succeeding a save). Nothing here adds a cost the master menu doesn't carry.

| Finisher | Special Cost | Effect |
|---|---|---|
| **Heavy Strike** | 20 | The final action deals **+2 damage dice** |
| **Unavoidable** | 30 | The final action **cannot be dodged, blocked, or substituted** |
| **Extension** | 40 | Add **one action beyond your combo limit** (ignores slot cost) |
| **Perfect Strike** | 60 | The final action is an **automatic critical hit** |
| **Signature Technique** | 100 (full bar) | Your named move. Auto-hit, auto-crit, maximum damage, and **it happens the way you describe it.** |

**Signature Technique is the point of the Special bar.** Every player should name theirs at character creation and spend the campaign earning the right to use it. It should get a full description, uninterrupted, at the table.

---
---

### PART FIVE — INTERRUPTION & ESCAPE

> **Rule 5 [SHEET]:** *If the combo is interrupted (stunned, knocked down, silenced, etc.), remaining actions are lost.*

The most important rule in the system. Here's what triggers it and how to fight it.

#### What Breaks a Combo

| Condition | Source |
|---|---|
| **Stunned** | Lightning techniques, concussive impacts, sound jutsu |
| **Knocked prone** | Leaf Whirlwind, sweeps, Earth techniques |
| **Silenced / seals blocked** | Grapples, restraints, chakra suppression |
| **Grappled or bound** | Wire, chains, Shadow Imitation, Water Prison |
| **Blinded** | Flash bombs, Blinding Technique, Hidden Mist |
| **Chakra or Stamina hits 0 mid-combo** | Your own overreach |
| **Genjutsu takes hold** | Failed CHA save |
| **Losing a Clash outright** | See Part Six |

#### Pushing Through **[GM]**

When an effect would interrupt **your own** combo, you may continue **only if you have the means**:

| Means | Effect |
|---|---|
| **Spend 30 Special** | Push through one interruption. The next action takes an additional **−2**. |
| **A clan, class, or mastery feature that grants it** | As written by that feature |

**There is no free save.** If you have neither, Rule 5 applies and the remaining actions are lost. Overreaching on a long combo is supposed to be a gamble.

---

#### THE TIMING IS FREE — THE MEANS ARE GATED

> **You may always react.** Your Reaction is available at any moment, including while a combo is landing on you (**Part Six**).
> **But escaping requires a jutsu, a clan ability, a ninja tool, or a feature that explicitly says so.** There is no generic "break the combo" option.

A character caught in a Jōnin's five-action **Cascade** is never *forbidden* from answering it — they Substitute out on action two if they have the Chakra, or throw down a flash bomb, or trigger a bloodline. What they cannot do is escape with an empty kit. **With nothing, they Brace and take all five actions.** That is correct, and it is why shinobi carry tools.

**Why it works this way:**

- **Substitution already exists.** It's on every character sheet from the Academy onward, it's a native Reaction **[SHEET]**, and it is *canonically* the answer to being caught out. It should be usable exactly when the fiction says it is — at the instant of impact, against any strike in a sequence. A generic escape button would make it redundant.
- **Combos need to be frightening.** One Reaction per round means answering action two leaves actions three through five unopposed.
- **It makes preparation matter.** Smoke bombs, flash bombs, and a spare tagged kunai stop being flavor and start being survival.

**What you can always do:** react, and Brace. See Part Seven.
**What you cannot do without an asset:** evade an action, displace out of reach, or end the combo.

---

#### The Three Escape Effects

Every escape asset produces exactly one of these. The wording on the asset tells you which.

| Effect | What it does | Typical source |
|---|---|---|
| **EVADE** | Negate **one action** of the combo. **The combo continues** with its remaining actions. | Defensive jutsu, clan passives, armor techniques |
| **DISPLACE** | You **move**. The attacker must still have the reach or range to continue; if not, the combo ends. | Substitution, Body Flicker, space–time techniques |
| **BREAK** | The combo **ends outright.** Remaining actions are lost. | Rare. Blinding the attacker, area denial, top-tier defenses |

**Evade is common, Displace is the workhorse, Break is precious.** Do not hand out Break casually.

---
---

### PART SIX — REACTIONS, THE COUNTER WINDOW & CLASHES

---

#### REACTION TIMING — you may act at any moment

> **Your Reaction is available at all times, including in the middle of someone else's combo.**

You do not wait for a missed opener, for the combo to end, or for your own turn. If an attacker is on action 3 of a five-action **Cascade** and you still have your Reaction, you spend it **right there**, against that action, before it resolves.

**This is what Substitution is for.** It is a native Reaction jutsu learned at the Academy **[SHEET]** precisely so a shinobi is never helpless mid-exchange.

##### What you may do at any point, against any single action

| Option | Requirement |
|---|---|
| **Substitution (Kawarimi)** | Know the jutsu — 8 Chakra / 5 Stamina, native Reaction **[SHEET]** |
| **Any other native-Reaction jutsu** | Know it |
| **Any jutsu with the Reactive mastery upgrade** | Book IV §3, Tier 3+, once per combat |
| **Any Escape Kit tool** | Carry it — flash bomb, smoke bomb, escape tag, tagged kunai |
| **A clan or bloodline ability that grants it** | Have the bloodline |
| **Brace** | None — universal, 8 Stamina |

##### What has not changed

**The timing is free. The means are not.** You still cannot invent an escape out of nothing — see Part Five. A character with no jutsu, no tool, and no feature can only **Brace**, and Brace does not stop the combo.

##### The real limit is one Reaction per round

Substituting out of action 2 of a five-action combo means **actions 3, 4, and 5 land unopposed.** You get one answer per round and you choose when to spend it — early and safe, or late and desperate.

##### After a mid-combo Displace

You've moved. The attacker must still have the **reach or range** to reach your new position:
- **They do** → the combo continues against you where you now stand.
- **They don't** → **[GM — house rule, superseding the original text below]** the attacker gets **one reroll** to close back in and continue, rather than the combo automatically ending. The Reaction that caused this is still spent for the round — there's no second Substitution waiting to answer the reroll — so whatever that second roll produces stands as the real outcome. This applies to DISPLACE specifically (Substitution and its kin); it does not change EVADE (already just negates the one action and moves on) or BREAK (still meant to be rare and genuinely combo-ending — blinding, hard area denial, top-tier defenses).

*Original ruling, superseded above: the combo simply ended on lost reach (Rule 5, no valid target). Kept here for reference — this is why Substitution against a melee combatant used to be so dominant, and it's exactly the edge case the house rule exists to soften.*

That's still why closing techniques like Flash Step matter to the attacker — a reroll only helps if there's a real way to use it.

---
---

#### THE COUNTER WINDOW

The one situation where you can cast a jutsu that **isn't** normally a Reaction.

Everything above is available to you at any time. The Counter Window adds one thing on top of it — and it's the thing that produces clashes.

##### The Trigger

> **When the FIRST action of a combo misses, the defender gains a Counter Window.**

"Misses" means the attack roll failed to beat AC, **or** the target succeeded on the saving throw.

**Only the first action.** A whiff on action three doesn't open anything — by then the attacker has committed and the defender is on the back foot.

#### What the Window Adds

> **Cast any jutsu you know as a Reaction**, even one that is normally an Action. Pay normal Chakra + **150% Stamina** — you're moving off-rhythm.

That's the whole of it. Everything else you could already do at any moment.

| | Any time, mid-combo | Counter Window only |
|---|---|---|
| Substitution and other native-Reaction jutsu | ✓ | ✓ |
| Reactive-upgraded jutsu (Book IV §3) | ✓ | ✓ |
| Escape Kit tools, clan abilities | ✓ | ✓ |
| Brace | ✓ | ✓ |
| Basic attack at −2 | ✓ | ✓ |
| **Any jutsu in your arsenal, cast reactively** | ✗ | **✓** |

**Restrictions:**
- Costs your **Reaction**. Already spent it? No window.
- **Once per combo**, regardless of how many actions miss.
- Jutsu cast here **cannot be S-rank** unless you have a feature that says otherwise.

> **This does not make Book IV §3's Reactive upgrade redundant.** The Counter Window is *conditional* — it only exists when an opponent's opener misses, and only fires once per combo. Reactive is *unconditional*, on your terms, and works on the technique of your choosing.

#### Why This Changes How You Open a Combo

**Book IV §2, Part Three** already told you to open with a jab to build Chain Momentum. Now there's a second, sharper reason: **a missed opener hands your opponent a free jutsu.**

| Opening choice | Risk |
|---|---|
| Basic attack | High hit chance. Low chance of granting a window. Wastes a slot. |
| D-rank technique | Balanced. |
| **Leading with your A-rank** | Maximum damage — and if it misses, your opponent gets to answer with anything they have. |

Leading with your strongest move is now a genuine gamble, which is exactly right.

---
---

#### THE CLASH

When a defender's technique and an attacker's action would meet — same space, same line, opposed forces — they **clash**.

**A clash can happen any time a defender puts a technique in the way**, not only in the Counter Window. A Reactive-upgraded jutsu, a native-Reaction technique, or a bloodline barrier used mid-combo all clash the same way. The Counter Window is simply the most common route to one, because it's the only route that doesn't require a feature.

##### When a clash happens

| Situation | Clash? |
|---|---|
| Two offensive techniques meeting in the same space or along the same line | **Yes** |
| Two melee or taijutsu techniques colliding | **Yes** |
| A barrier or defensive technique intercepting an offensive one | **Yes** |
| Defender uses **Substitution** | **No** — they DISPLACE. Combo ends only if reach is lost. |
| Defender casts a buff, a heal, or something that doesn't intersect | **No** — both resolve independently |
| **Rank gap of 3+ steps** | **No clash.** The higher-ranked technique simply consumes the lower. A D-rank Fireball does not contest an S-rank. |

That last row matters. A genin cannot stalemate a Kage by throwing something at them.

---

##### Clash Resolution — Two Stages

**Stage 1 — THE LOCK**
Both combatants roll **d20 + their jutsu modifier + clash modifiers.**
Higher total **wins the Lock** — their technique has the upper hand in the collision.

**Stage 2 — THE BREAK**
Both roll again. **The Lock winner adds +5.**
Whoever wins Stage 2 pushes their technique through.

| Outcome | Result |
|---|---|
| **One combatant wins BOTH stages** | **TOTAL OVERPOWER** |
| **Different winners in each stage** | **MUTUAL DETONATION** |

**Ties in either stage go to the higher-ranked technique.** Still tied? Re-roll that stage.

---

##### Outcomes

**TOTAL OVERPOWER — attacker wins both**
Their technique blows straight through. **Full damage +50%.** The defender's jutsu is destroyed and its cost is spent for nothing. **The combo continues** with its remaining slots.

**TOTAL OVERPOWER — defender wins both**
The defender's technique blows through. Full damage to the attacker. **The attacker's combo ENDS immediately** — this is a Rule 5 interruption. Every remaining action is lost.

**MUTUAL DETONATION**
Both techniques annihilate each other in the space between. Both combatants take **half damage from the opposing technique**, both are pushed back **15 ft**, and the attacker's **combo continues at −2** on all remaining actions while they recover their footing.

---

##### Clash Modifiers

| Modifier | Bonus |
|---|---|
| Your technique is **higher rank** | **+2 per rank step** |
| **Nature advantage** (Book II §1 cycle) | **+3** |
| **Nature disadvantage** | **−3** |
| **Mastery tier** (Book IV §3) | **+1 per tier** |
| Higher ground or favorable terrain | **+2** |
| You did not move this turn (stable stance) | **+1** |
| **Off-balance** — you're the one in the Counter Window | **−1** |
| Chain Momentum already built this combo | **+1 per prior action landed** |

---

##### OVERCHARGE — pouring it on

> **Between Stage 1 and Stage 2, either combatant may Overcharge:** spend additional Chakra equal to the technique's base cost to add **+4** to their Stage 2 roll.

**Maximum two Overcharges per combatant per clash** (+8 total, at double the technique's base cost).

**Both sides declare Overcharge simultaneously, then reveal.** Nobody knows whether the other is committing until the chakra is already spent. This is the single best table moment the system produces — make people declare out loud, at the same time.

**If you Overcharge and still lose the Break,** the Chakra is gone and you take **1 level of exhaustion** from the strain.

---

##### Special Clash Types

**Mirror Clash** — the same technique against itself (Fireball vs. Fireball). No nature modifier applies. On **Mutual Detonation**, the blast is unstable: every creature within 15 ft of the collision point takes **half damage** from the explosion, not just the two combatants.

**Barrier Clash** — a defensive technique intercepting an offensive one. If the barrier wins the Lock, it holds regardless of Stage 2 — it just takes damage. If it loses the Lock, Stage 2 determines whether it **shatters** (attacker wins) or **cracks** (mutual: barrier survives at half effect for the rest of the combat).

**Force Clash** — two taijutsu or shape-manipulation techniques. Use **Taijutsu skill + STR modifier** instead of the jutsu modifier. Everything else is identical.

**Elemental Clash** — the standard case. The nature cycle applies at **+3 / −3**, which is often decisive.

---
---

#### WORKED EXAMPLE — Sasuke vs. Naruto

*Both Chūnin. Sasuke has a 4-slot combo.*

**Sasuke's turn.** He uses his **Bonus Action** for **Flash Step**, closing 30 ft in a straight line. **[SHEET]**

**Combo action 1 — Leaf Whirlwind** (D-rank, 1 slot, 12 Chakra / 5 Stamina). 15-ft radius, DEX save.
**Naruto rolls his DEX save — and succeeds.**

> **MISS. The Counter Window opens.**

**Naruto spends his Reaction.** He has three options he can actually use: Substitution (8 Ch / 5 St), Brace, or a jutsu. He picks the jutsu.

**Naruto casts Fire Release: Fireball** — 12 Chakra, and 8 Stamina instead of 5 (150% for reacting off-rhythm).

**Sasuke declares combo action 2 — Fire Release: Fireball.** Both fireballs are launched along the same line.

> **MIRROR CLASH.**

**STAGE 1 — THE LOCK**

| | Roll | Modifiers | Total |
|---|---|---|---|
| **Sasuke** | 14 | +5 Ninjutsu, +2 Mastery (Proficient) | **21** |
| **Naruto** | 17 | +3 Ninjutsu, +1 Mastery (Practiced), **−1 off-balance** | **20** |

**Sasuke wins the Lock by one.** His fireball is driving forward. Naruto's is buckling.

**OVERCHARGE — both declare simultaneously.**
Sasuke, confident, declines. **Naruto Overcharges** — another 12 Chakra for **+4**.

**STAGE 2 — THE BREAK**

| | Roll | Modifiers | Total |
|---|---|---|---|
| **Sasuke** | 8 | +7, **+5 Lock winner** | **20** |
| **Naruto** | 15 | +2, **+4 Overcharge** | **21** |

**Naruto wins the Break by one.**

> **Split result — MUTUAL DETONATION.**

The two fireballs meet mid-air and blow apart. Both take half damage from the other's technique. Both are thrown back 15 ft. Because it's a **Mirror Clash**, everyone within 15 ft of the collision eats half damage too.

**Sasuke's combo continues** — 2 slots remaining, at **−2** — and he is now 15 ft further away than he was, having spent his Flash Step to close that distance in the first place.

*Naruto spent 24 Chakra and a Reaction to turn a losing exchange into a stalemate and reset the distance. That's a win.*

---
---

### PART SEVEN — DEFENSIVE ACTIONS & ESCAPE ASSETS

You get **one Reaction per round**, spendable **at any moment** — including between actions of an enemy combo (**Part Six**). What you can do with it depends entirely on what you're carrying.

#### The only universal option: BRACE

| Action | Cost | Effect |
|---|---|---|
| **Brace** | 8 Stamina | Reduce the damage of **one action** by **1d6 + CON modifier**. |

That's it. Brace does not evade, does not displace, does not break the combo, and does not stop the actions that follow. It is what you do when you have nothing — you cover up and take it.

**If a player has no escape asset and gets caught, this is their turn.** Let it sting. It's the reason they'll buy a flash bomb before the next mission.

---

#### Escape Assets — Jutsu

Anything a character actually knows, from the Jutsu Compendium. **Cost is the jutsu's normal cost.**

| Jutsu | Rank | Cost | Effect | Notes |
|---|---|---|---|---|
| **Substitution (Kawarimi)** | E | 8 Ch / 5 St **[SHEET]** | **DISPLACE** — 15 ft | **The default answer.** Not usable vs. area attacks. Once per round. **[SHEET]** |
| **Rope Escape** | E | 3 Ch / 2 St **[SHEET]** | Ends **Bound** only | Not a combo escape; frees you for next turn |
| **Hiding in Mist** | D | Per compendium | **BREAK** if the attacker loses sight | Requires a water source |
| **Hydrification** (Hōzuki) | D | Per compendium | **EVADE** vs. non-elemental physical | Lightning bypasses it entirely |
| **Water / Earth / Ink Clone** | C | Per compendium | **DISPLACE** — the clone takes the action | Clone is destroyed |
| **Earth Release: Hiding Like a Mole** | C | Per compendium | **DISPLACE** — underground | Sensors still find you |
| **Transparent Escape Technique** | C | Per compendium | **BREAK** if the attacker can't track you | Fails vs. dōjutsu and sensors |
| **Hiding with Camouflage** | A | Per compendium | **BREAK** | Only dōjutsu can follow you |
| **Flying Thunder God** | S | Per compendium | **BREAK** | Requires a pre-placed marker |
| **Kamui** | Unranked | Per compendium | **EVADE** — intangibility | Obito / Kakashi only |
| **Eight Trigrams Palms Revolving Heaven** | Unranked | Per compendium | **BREAK** — 360° repulsion | Hyūga only |
| **Susanoo** | Unranked | Per compendium | **EVADE**, repeatedly | Mangekyō only |

**Reaction timing:** most of these are normally an **Action**. To use one as a Reaction you need either the **Reactive** mastery upgrade (**Book IV §3**) or a feature that grants it. **Substitution is a Reaction natively** **[SHEET]** — which is exactly why it's the one everyone learns first.

---

#### Escape Assets — Clan & Bloodline

Drawn from the Clan Bloodline Reference (**Book IV §1, Part Four**).

| Clan | Effect | Cost |
|---|---|---|
| **Hōzuki** | **EVADE** vs. non-elemental weapon damage | Free — it's the clan passive |
| **Iburi** | **BREAK** — Smoke Form | Once per short rest **[SHEET]** |
| **Hagoromo** | **Brace upgrade** — halve all incoming damage from the whole combo | Once per long rest **[SHEET]** |
| **Kazekage Bloodline** | **EVADE** — Sand Shield negates the first action against you each round | Free while conscious |
| **Kaguya** | Bone Armor: +1 AC (passive, not an escape) | Free |
| **Yōtsuki** | **EVADE** vs. lightning specifically | Free |
| **Akimichi** | **DISPLACE** — Human Bullet Tank rolls you clear | Technique cost |
| **Nara** | **BREAK** — Shadow Imitation on the attacker mid-combo | Technique cost; needs line of shadow |

---

#### Escape Assets — Ninja Tools

**This is why tools exist.** A squad without an escape kit is a squad that dies in someone's Cascade.

| Tool | Cost (ryō) | Effect | Uses |
|---|---|---|---|
| **Smoke bomb** | 300 | **BREAK** if the attacker relies on sight (DC 13 Perception to continue) | 1 |
| **Flash bomb** | 400 | **BREAK** — attacker makes a CON save DC 13 or is **blinded**, ending the combo | 1 |
| **Makibishi (caltrops)** | 200 | **EVADE** — attacker must stop or take 1d6 and lose their next action | 1 |
| **Tagged kunai** | 600 | **EVADE** — thrown as a Reaction; attacker must break off or eat 3d6 | 1 |
| **Tripwire (pre-set)** | 200 | **BREAK** — only in prepared terrain, set before combat | 1 |
| **Escape tag** | 1,500 | **DISPLACE** — 30 ft, no line of sight needed. A manufactured Kawarimi. | 1 |
| **Blinding powder** | 250 | **EVADE** — attacker takes −4 on their next action | 1 |
| **Chakra-shroud cloak** | 8,000 | **EVADE** — negate one action per combat | Rechargeable |

**Deliberately consumable.** An escape kit is something you spend and have to re-buy, which makes downtime shopping a real decision and gives D-rank mission pay a purpose.

---

#### Escape Assets — Skills & Features

| Source | Effect |
|---|---|
| **Kenjutsu proficiency — Parry** | **EVADE** one melee action, then a free basic attack at −4. Costs 12 Stamina. |
| **Taijutsu proficiency — Read the Rhythm** | Once per combat, **EVADE** one action if you beat the attacker's roll with a Taijutsu check |
| **Sensor Skills proficiency** | You are never **surprised**, so you always have your Reaction available |
| **Reactive mastery upgrade** (Book IV §3) | Convert one known jutsu to Reaction casting, once per combat |

---

#### Design note — Stamina and Body of Ashura

Brace and Parry both run on Stamina, which is what makes **Body of Ashura** viable defensively. *Powerful Life Force* (+5 Stamina at the start of each round) **[SHEET]** roughly pays for a Brace every other round. An Ashura taijutsu specialist doesn't escape combos — they absorb them and keep walking forward. That's the correct feel.

---
---

### PART EIGHT — TEAM COMBOS

The most Naruto thing in the system. Ino-Shika-Chō, Naruto and Sasuke, the Kakashi–Gai formations.

#### Declaring a Team Combo

Two or more characters may link their combos if:
1. They act on **consecutive initiative counts** (or one **readies** an action to link), and
2. They **declare the link** before the first character acts.

#### Benefits

| Benefit | Effect |
|---|---|
| **Shared Momentum** | Chain Momentum carries across all participants. A four-person team chain builds terrifying damage. |
| **Shared Openings** | If any participant forces a failed save, the target is **Open to everyone** in the chain. |
| **No Escalating Penalty** | Each participant's actions count separately for the −1/−2/−3 penalty. Everyone starts clean. |
| **Team Special** | If the full chain resolves without interruption, **every participant gains +15 Special.** |

#### The Risk

**If any participant's segment is interrupted, the entire chain ends.** Everyone downstream loses their actions. Team combos are high reward and genuinely fragile — which is why squads drill them.

#### Collaboration Jutsu

Two participants may spend their actions to produce a **single combined technique** one rank higher than either could cast alone. Both pay full cost. Common pairings:

| Combination | Result |
|---|---|
| **Fire + Wind** | Massively amplified flame. +3 damage dice, doubled area. |
| **Water + Lightning** | Conducting field. All targets in the water: CON save or **stunned**. |
| **Earth + Lightning** | Charged terrain. Ignores cover; difficult terrain persists. |
| **Wind + Lightning** | Extended arc. Triple range, ignores half cover. |
| **Water + Earth** | Mud field. Area becomes difficult terrain; targets have speed halved. |
| **Fire + Earth** | Molten barrier. Creates cover that deals 2d6 fire to anyone crossing. |

**This is also the mechanical argument for teamwork** that the sheet's Rule of Balance points at: *"intelligence, timing, and teamwork are just as important as power."*

---
---

### PART NINE — ELEMENTAL CHAINING

Within a **single** character's combo, consecutive actions using complementary natures gain a bonus. Same pairings as Collaboration Jutsu, at reduced effect.

| Sequence | Bonus on the second action |
|---|---|
| **Fire → Wind** or **Wind → Fire** | +2 damage dice |
| **Water → Lightning** | Target: CON save or stunned (breaks *their* next combo) |
| **Earth → Lightning** | Ignores cover |
| **Wind → Lightning** | Double range |
| **Water → Earth** | Creates difficult terrain in the area |

**Requires two nature affinities**, so this is a Jōnin-and-above reward — which is correct. Learning a second nature (**Book IV §1**) suddenly has a concrete combat payoff beyond "more options."

#### The Nature Cycle in Combat

**Fire > Wind > Lightning > Earth > Water > Fire** — see **Book II §1**.

| Relationship | Effect |
|---|---|
| **Strong against** | +1 damage die; target has **disadvantage** on the save |
| **Neutral** | No change |
| **Weak against** | **Half damage**; target has **advantage** on the save |

**Override:** if the attacker's technique is **two or more ranks higher**, ignore the cycle. Volume beats matchup.

---
---

### PART TEN — STATUS CONDITIONS

Shinobi-specific conditions. All of these interact with the combo system, which is what makes them worth applying.

| Condition | Effect | Ends when |
|---|---|---|
| **Chakra Sealed** | Cannot spend Chakra. Taijutsu only. | Seal removed, or 1 hour |
| **Stunned** | **Breaks combos.** No actions. | End of next turn, or CON save |
| **Open** | Attacks against you have advantage | Attacker's combo ends |
| **Ignited** | 1d6 fire at the start of each turn | Action to extinguish, or immersion |
| **Poisoned** | Disadvantage on attacks; escalating damage | Antidote, or the poison's duration |
| **Genjutsu'd** | The DM controls your actions | CHA save, or an ally disrupts you |
| **Marked** | Can be located and targeted at range regardless of concealment | Mark removed |
| **Bound** | Cannot move; **combos limited to 1 action** | Escape check, or Rope Escape |
| **Exhausted** | Stamina at 0 — no Taijutsu, no defensive reactions, movement halved | Rest or Stamina recovery |
| **Chakra Drained** | Chakra at 0 — no jutsu; may spend **2 Health per 1 Chakra** | Rest or Chakra recovery |

**Chakra Sealed is the Hyūga win condition.** Gentle Fist doesn't out-damage anyone — it turns a ninjutsu specialist into a civilian. Play it that way.

---
---

### PART ELEVEN — INITIATIVE, SURPRISE & THE ROUND

#### Initiative
**Initiative = DEX modifier.** Hyūga add **+2** (Byakugan) **[SHEET]**.

#### Why Going First Matters More Here
Because of Rule 5. Whoever acts first can potentially **break the other's combo before it starts.** In a game where a Kage can chain seven actions, initiative is the single most valuable die roll of the fight.

#### Surprise & Ambush

| Situation | Effect |
|---|---|
| **Target unaware** | Attacker has advantage; **the target cannot Substitute** |
| **Silent Killing** (obscured + unaware) | **Automatic critical hit** |
| **Ambush by a full squad** | Ambushers act before initiative is rolled |

#### The Round, in order

1. **Start of round** — Ashura recovers 5 Stamina; ongoing conditions tick; **+5 Special** to everyone
2. **Movement** — free, up to your speed
3. **Action** — your combo (1 to 7 slots by rank)
4. **Bonus Action** — one, after the combo **[SHEET]**
5. **Reaction** — one, available until your next turn **[SHEET]**
6. **End of turn** — check resource thresholds

---
---

### PART TWELVE — QUICK REFERENCE CARD

**Print this side of the screen.**

```
╔═══════════════════════════════════════════════════════╗
║  COMBO LIMIT BY RANK                                  ║
║  Academy 1 │ Genin 3 │ Chūnin 4 │ Jōnin 5             ║
║  S-Rank 6 │ Kage 7                                    ║
╠═══════════════════════════════════════════════════════╣
║  SLOT COST                                            ║
║  Basic / E / D .... 1    C / B .... 2                 ║
║  A .... 3                S .... 4                     ║
╠═══════════════════════════════════════════════════════╣
║  ESCALATION      4th −1 │ 5th −2 │ 6th −3 │ 7th −4    ║
║  MOMENTUM        +2 damage per prior action that HIT  ║
║  OPENING         Failed save = advantage, rest of combo║
╠═══════════════════════════════════════════════════════╣
║  AFTER THE COMBO   1 Bonus Action  +  1 Reaction      ║
╠═══════════════════════════════════════════════════════╣
║  BREAKS A COMBO                                       ║
║  Stunned · Prone · Silenced · Grappled · Blinded      ║
║  Resource at 0 · Genjutsu · Losing a Clash            ║
║  Push through: 30 SPECIAL, or a feature. No free save.║
║             next action takes an additional −2        ║
╠═══════════════════════════════════════════════════════╣
║  ESCAPING A COMBO — REQUIRES AN ASSET                 ║
║  Timing is free; the MEANS are gated.                 ║
║  No asset = Brace and eat it.                         ║
║                                                       ║
║  EVADE    negate 1 action, combo continues            ║
║  DISPLACE you move; combo ends if reach is lost       ║
║  BREAK    combo ends outright  (rare)                 ║
║                                                       ║
║  Sources: jutsu · clan ability · ninja tool · feature ║
║  Default: SUBSTITUTION  8 Ch / 5 St  (Reaction)       ║
╠═══════════════════════════════════════════════════════╣
║  REACTIONS — USABLE AT ANY MOMENT                     ║
║  Spend your Reaction ANY time, incl. mid-combo, vs    ║
║  any single action. Timing is free; the MEANS are not.║
║   Substitution 8 Ch/5 St · native-Reaction jutsu      ║
║   Reactive-upgraded jutsu · Escape Kit tools          ║
║   clan abilities · Brace (universal)                  ║
║  ONE per round — the rest of the combo still lands.   ║
║  Displaced? Combo continues if they can still reach.  ║
╠═══════════════════════════════════════════════════════╣
║  COUNTER WINDOW — adds ONE thing                      ║
║  FIRST action of a combo MISSES → you may cast ANY    ║
║  jutsu you know as a Reaction (+150% Stamina).        ║
║  Once per combo. No S-rank.                           ║
║                                                       ║
║  CLASH — when two techniques meet                     ║
║   STAGE 1 THE LOCK   d20 + jutsu mod + modifiers      ║
║   STAGE 2 THE BREAK  d20, Lock winner +5              ║
║   Win both  → TOTAL OVERPOWER (+50% dmg)              ║
║             attacker wins: combo continues            ║
║             defender wins: COMBO ENDS                 ║
║   Split     → MUTUAL DETONATION                       ║
║             both take half, both pushed 15 ft,        ║
║             combo continues at −2                     ║
║   OVERCHARGE  +4 for base cost again, max ×2          ║
║               declare SIMULTANEOUSLY, then reveal     ║
║   Rank gap 3+ steps = NO CLASH, higher just wins      ║
╠═══════════════════════════════════════════════════════╣
║  UNIVERSAL REACTION (the only one)                    ║
║  BRACE  8 St — reduce ONE action by 1d6+CON           ║
║         does not evade, displace, or break            ║
╠═══════════════════════════════════════════════════════╣
║  PUSH THROUGH your own interrupted combo:             ║
║  30 Special, or a feature. There is no free save.     ║
╠═══════════════════════════════════════════════════════╣
║  FINISHERS (Special)                                  ║
║  Heavy Strike 20 │ Unavoidable 30 │ Extension 40      ║
║  Perfect Strike 60 │ SIGNATURE 100                    ║
╚═══════════════════════════════════════════════════════╝
```

---
---

### PART THIRTEEN — NPCS AND COMBOS

Per the printed rule, **NPCs are not bound by any of this** (**Book IV §1, Part Eight**; **Book IV §4**).

Suggested NPC combo limits, for consistency rather than obligation:

| Threat Profile | Combo Limit | Notes |
|---|---|---|
| Fodder | 1 | No combos at all |
| Genin | 2 | Slightly under a PC of the same rank |
| Chūnin | 3 | |
| Jōnin | 4, **plus one free Bonus Action technique** | |
| ANBU | 4, **opens with an ambush** | |
| S-Rank | 5, **plus a rule-breaking gimmick** | |
| Kage | 6, **plus 2 free actions on others' turns** | |
| **Legendary** | **Whatever the scene requires.** | Don't count. Track rounds remaining instead. |

**Deliberately, most NPC profiles sit one below the equivalent PC rank.** The players' combo ceiling is their advantage — the NPCs' advantage is everything else on their sheet. That asymmetry is the point.


---
---

# §3 — JUTSU MASTERY & CREATION

Two connected systems: how a technique you already know gets **better**, and how you invent one that doesn't exist yet.

This is the expansion of the printed **Upgrades** note on the Genin Ability sheet — *"As you grow in rank and experience, these jutsu can be improved or evolved into more powerful versions."* **[SHEET]**

Everything else here is **[GM]**.

---
---

### PART ONE — THE MASTERY LADDER

Every jutsu on your sheet has its own mastery tier, tracked separately. Two shinobi who both "know" the Great Fireball are not equally good at it.

| Tier | Name | Mastery XP | Grants |
|---|---|---|---|
| **0** | **Learned** | 0 | You can perform it |
| **1** | **Practiced** | 10 | 1 Mastery Point |
| **2** | **Proficient** | 25 | 1 Mastery Point |
| **3** | **Mastered** | 50 | 1 Mastery Point + unlocks restricted upgrades |
| **4** | **Perfected** | 100 | 1 Mastery Point + **Signature Variant** |

**Four Mastery Points total per jutsu.** You will never perfect everything — that's the constraint that makes the choice matter.

#### What each tier feels like

- **Learned.** You can do it. Under pressure it comes out sloppy.
- **Practiced.** Reliable. You don't think about the seals anymore.
- **Proficient.** It's *yours*. You use it without deciding to.
- **Mastered.** Better than the version you were taught.
- **Perfected.** Nobody else's looks like this. You've earned the right to rename it.

#### Tracking

Add a **Mastery** column beside each entry under **Known Jutsu** on the character sheet:

```
KNOWN JUTSU              RANK  TYPE      COST      MASTERY
Fire Release: Fireball    D    Ninjutsu  12/5      ●●●○○  (Proficient, 31 XP)
Body Flicker              D    Ninjutsu   8/6      ●●○○○  (Practiced, 14 XP)
Substitution              E    Ninjutsu   8/5      ●●●●● (PERFECTED — "Empty Log")
```

---
---

### PART TWO — GAINING MASTERY XP

#### In the field

| Event | Mastery XP |
|---|---|
| Use the jutsu successfully in combat (hits, or forces a failed save) | **+1** |
| Use it successfully against a higher-ranked opponent | **+2** |
| Use it to solve a problem it wasn't designed for | **+3** |
| Land the finishing blow of a serious fight with it | **+3** |
| Use it under genuine duress — dying, blinded, out of chakra | **+2** |

**Cap: 5 Mastery XP per jutsu per combat.** Spamming one technique down a corridor doesn't teach you anything.

#### DOWNTIME ACTIVITIES **[GM — ADDED. Training was the only downtime activity in the system.]**

**A week of downtime buys each character one Major activity and any number of Minor ones.**

| Major activity | What it does |
|---|---|
| **Dedicated training** | Mastery XP per the table below. **Capped at 25 XP per technique per week** |
| **Learn a new technique** | Requires a teacher, a scroll, or firsthand observation. **One week for D-rank, two for C, four for B, a season for A, longer for S** |
| **Nature affinity work** | Progress on a second nature. **Slow by design** — Book II §2 |
| **Build something** | A seal, a tool, a poison, a modification. **GM prices it in weeks** |
| **Work a contact** | Turn an acquaintance into an asset, or an asset into a friend. **One NPC relationship advances a stage** |
| **Recover properly** | Clears one lingering injury or condition that rest alone will not touch |
| **Chase a thread** | Pursue one entry from `campaign/story-beats.md`. **This is how ARMED beats become READY** |

| Minor activity | What it does |
|---|---|
| **Shop and restock** | Escape kit, consumables, replacements. Book II §4 |
| **Requisition** | Village gear above standard issue. **Needs approval, and approval is a scene** |
| **Report and be debriefed** | Information flows both ways. **The village learns what you did** |
| **Spar** | +3 Mastery XP per day on one technique, and somebody else finds out what you can do |
| **Rest** | Nothing happens. **Let it be an option** |

> **⚠ Downtime is where the village notices you.** Every Major activity above is visible to somebody. A character who trains alone for a season is *also* a character nobody has seen for a season.

#### In downtime

| Training | Mastery XP per day |
|---|---|
| Solo practice | **+2** |
| With a teacher who has it at higher mastery | **+4** |
| With the jutsu's **creator** | **+6** |
| Against a live sparring partner | **+3** |

#### Shadow Clone Training

The single most important downtime rule in the setting, and it should be mechanically real.

> **Each Shadow Clone dedicated to training a jutsu generates Mastery XP in parallel.** When the clone dispels, its experience returns to you.

| Clones training | Effective XP multiplier **[GM — REPAIRED, was linear]** |
|---|---|
| 1 (just you) | **×1** |
| 2–4 | **×2** |
| 5–9 | **×3** |
| 10–19 | **×4** |
| 20+ | **×5** |

**The cost:** each clone drains Chakra for the duration, and dispelling them inflicts the mental strain of days of memory arriving at once.

| Clones trained that day | Chakra per training day | Strain **[GM — REPAIRED]** |
|---|---|---|
| 2–4 | 30 each | None |
| 5–9 | 30 each | CON save DC 13 or lose the next day to a migraine |
| 10–19 | 30 each | CON save DC 16 or **1 day unconscious** |
| 20+ | 30 each | CON save DC 20 or **1d4 days unconscious**, and roll on the Backfire table |

> ## ⚠ THE TWO REPAIRS, AND WHY
>
> **1 — The multiplier was linear and it broke the mastery ladder.** Ten clones at **×10** on solo practice is **+20 XP a day. Perfected costs 100.** That is **five days to take any technique to Tier 4 including its Signature Variant**, and twenty clones did it in two and a half. A month of downtime perfected an entire kit. **Diminishing returns above.** Clones are still the best training method in the setting by a wide margin — they are no longer a cheat code.
>
> **2 — The strain keyed off the *dispel*, not the training.** A shinobi with twenty clones simply dispelled them **four at a time** and paid nothing at all, because *"2–4: none."* The table now keys off **how many were trained that day**, which is what the strain is actually made of. **You cannot batch your way out of a week of memories.**
>
> **3 — Hard ceiling: a single technique may gain at most 25 Mastery XP per week of downtime**, by any method or combination of methods. **Perfected therefore takes a month of dedicated work at minimum**, which is what *"over a single downtime arc"* was always meant to mean.

**This is how a character goes from adequate to terrifying over a single downtime arc** — and it costs them something real. It's also gated behind an A-rank kinjutsu, so nobody's doing it at Genin.

---
---

### PART THREE — MASTERY UPGRADE PATHS

Spend Mastery Points from the menu below. **Max 4 points in any single jutsu.**

| Upgrade | Effect per point | Max points | Restriction |
|---|---|---|---|
| **Efficiency** | **−15% Chakra cost** | 3 | — |
| **Conditioning** | **−15% Stamina cost** | 3 | — |
| **Power** | **+1 damage die** | 2 | — |
| **Precision** | **+1 to hit and +1 to save DC** | 2 | — |
| **Acceleration** | **−1 combo slot** (minimum 1) | 2 | Tier 3+ |
| **Extension** | **+50% range or area** | 2 | — |
| **Control** | **+1 target**, or **+1 round duration** | 2 | — |
| **Seal-less** | **Remove the hand seal requirement** entirely | 1 | Tier 3+ |
| **Adaptation** | The jutsu works in one terrain that normally forbids it | 1 | — |
| **Reactive** | Cast the jutsu as a **Reaction**, once per combat | 1 | Tier 3+ |

#### Why Acceleration is the big one

**−1 combo slot** interacts directly with **Book IV §2's Action Weight.** A Mastered A-rank technique that costs **2 slots instead of 3** means a Jōnin can chain **A-rank → C-rank** in one turn instead of **A-rank → punch → punch**.

Two points of Acceleration on an S-rank drops it from 4 slots to 2. A Kage with a Perfected S-rank can throw it **twice** in one combo — which is precisely the kind of thing that should take a whole campaign to earn.

#### Why Reactive matters

Per **Book IV §2**, there is **no universal way to escape a combo** — you need a jutsu, clan ability, tool, or feature. But most defensive jutsu are cast as an **Action**, which is useless when someone else's combo is landing on you.

**Reactive is how a technique becomes an escape asset.** A Mastered Hiding in Mist that can be triggered as a Reaction turns a utility jutsu into a combo-breaker. This is one of the strongest reasons to take a defensive technique to Tier 3 instead of spreading mastery across your offense.

**Substitution is already a Reaction natively** **[SHEET]** — which is exactly why every shinobi learns it, and why it's still worth Perfecting.

#### Seal-less casting

Removing hand seals is worth more than its slot cost suggests:

- Cannot be identified by an opponent reading your seals
- Works while **grappled, bound, or one-armed**
- Immune to counter-seal interruption

The Rasengan requires no hand seals in canon. This is that, as an earned upgrade.

---
---

### PART FOUR — PERFECTED: SIGNATURE VARIANTS

At **Tier 4**, a jutsu stops being a technique you learned and becomes a technique that is *yours*.

#### You get three things:

**1. Rename it.** *Chidori* was Kakashi's Lightning Cutter before Kakashi's version got its own name. Write the new name on your sheet.

**2. A Signature Rider.** Pick one, or design one with your DM:

| Rider | Effect |
|---|---|
| **Relentless** | On a miss, deal half damage anyway |
| **Overwhelming** | Targets have disadvantage on the save |
| **Lingering** | Effect persists one additional round with no upkeep |
| **Piercing** | Ignores resistance and half cover |
| **Chained** | On a kill or a critical, you may immediately use it again free (once per combat) |
| **Momentum** | Counts as **two** actions for Book IV §2's Chain Momentum |
| **Anchor** | Cannot be interrupted by Rule 5 once begun |

**3. Signature Technique eligibility.** A Perfected jutsu can be spent as your **100-Special Finisher** (Book IV §2, Part Four) — auto-hit, auto-crit, maximum damage, described the way you want it described.

#### Evolution

A Perfected jutsu can also be **evolved** into a higher-rank technique — which is exactly how the Jutsu Compendium's real chains work:

| Base | → | Evolution | → | Peak |
|---|---|---|---|---|
| Rasengan (A) | → | Big Ball Rasengan (A) | → | Wind Release: Rasenshuriken (S) |
| Chidori (A) | → | Chidori Sharp Spear (A) | → | Lightning Cutter (S) |
| Shadow Imitation (C) | → | Shadow Clutch (A) | → | Shadow Sewing |
| Clone (E) | → | Shadow Clone (A) | → | Multiple Shadow Clone (A, kinjutsu) |
| Great Fireball (C) | → | Dragon Fire (C) | → | Fire Dragon Bullet (C) |

**Evolution requirements:**
- The base jutsu at **Perfected**
- Your rank meets the evolution's rank minimum
- The development process from Part Eight (at half time and cost — you're not starting from nothing)

**The evolved jutsu starts at Tier 0.** You perfected the parent, not the child. This is why Naruto spends years on the Rasengan and still can't throw a Rasenshuriken without wrecking his arm.

---
---

### PART FIVE — CREATING NEW JUTSU: REQUIREMENTS

You don't get to invent an S-rank technique at Genin. Gates first.

| Target rank | Minimum shinobi rank | Prerequisites |
|---|---|---|
| **E** | Genin | None |
| **D** | Genin | One E-rank at **Practiced** |
| **C** | Chūnin | Two D-rank at **Proficient** in the same category |
| **B** | Chūnin | One C-rank at **Mastered** + proficiency in the relevant skill |
| **A** | Jōnin | Two B-rank at **Mastered**, one of them **Perfected** |
| **S** | S-Rank | One A-rank at **Perfected** |
| **Kinjutsu** | Jōnin+ | DM approval, and a reason worth what it costs |

**Category** means Ninjutsu, Genjutsu, Taijutsu, Fūinjutsu, Medical, Kenjutsu, Shurikenjutsu, or Puppetry. You build on what you already do.

**Nature restrictions apply.** You cannot create a Fire Release technique without the Fire affinity. You cannot create a kekkei genkai technique without the bloodline — see **Book IV §1, Part Four**.

**Rank-ceiling overrides (Other Power System abilities) [GM — standing rule].** The "minimum shinobi rank" column above gates what rank of jutsu a character can *know and cast* under normal progression, not just what they can invent. Some Other Power System grants (Book III/character-sheet-specific, entity-granted or otherwise) lift that ceiling for their duration rather than raising the character's actual shinobi rank — the character still needs to actually *know* the technique (through the normal channels: training, story, teaching) for the override to matter; it removes the rank gate in advance, it doesn't hand out new jutsu. **First instance:** Ardo's 紅風 Kōfū — while active, he may cast up to S-rank jutsu regardless of his baseline Chūnin ceiling. See `characters/ardo.md` for the full writeup.

---
---

### PART SIX — THE DESIGN BUDGET

Each new jutsu gets a pool of **Jutsu Points (JP)** based on its target rank. Spend them on effects.

| Rank | JP Budget | Chakra cost | Stamina cost | Combo slots |
|---|---|---|---|---|
| **E** | 2 | 3–8 | 0–5 | 1 |
| **D** | 4 | 8–12 | 5–8 | 1 |
| **C** | 7 | 15–25 | 8–14 | 2 |
| **B** | 11 | 30–45 | 15–22 | 2 |
| **A** | 16 | 50–70 | 25–35 | 3 |
| **S** | 22 | 80–110 | 40–55 | 4 |

#### Effect Menu

| Effect | JP Cost |
|---|---|
| **Damage** — 1 die (d6 for most, d8 for elemental, d10 for piercing) | **1 per die** |
| **Range** — melee → 30 ft → 60 ft → 120 ft → 300 ft | **1 per step** |
| **Area** — single target → 10 ft → 15 ft → 30 ft → 60 ft | **1 per step** |
| **Line or cone** instead of radius | **1** |
| **Condition rider** (prone, stunned, blinded, restrained, ignited) | **2** |
| **Movement effect** (push, pull, or self-movement up to 30 ft) | **1** |
| **Duration** — 1 round → 1 minute → 10 minutes | **1 per step** |
| **No hand seals** | **3** |
| **Concealment or invisibility** | **2** |
| **Healing** — 1 die | **2 per die** |
| **Additional target** | **1 each** |
| **Ignores cover** | **1** |
| **Ignores resistance** | **2** |
| **Sustained** (upkeep cost per round, effect persists) | **2** |
| **Sensory effect** (detect, track, mark) | **2** |
| **Summon or construct** (a puppet, clone, or creature that acts) | **3** |
| **Barrier or defense** (grants AC or damage reduction) | **2** |
| **Bonus Action** cast instead of Action | **3** |
| **Reaction** cast instead of Action | **4** |

---
---

### PART SEVEN — DRAWBACKS

**Drawbacks give JP back.** This is the most important part of the system, because every great technique in the setting has one. The Rasenshuriken shreds the user's arm. The Chidori commits you to a straight line you can't see out of. The Eight Gates kill you.

**A jutsu with no drawback is a boring jutsu.** Encourage them.

| Drawback | JP Returned |
|---|---|
| **Self-damage** — take a fixed portion of the damage dealt | **+2** |
| **Recoil** — 1 level of exhaustion, or lose 25% remaining Stamina | **+2** |
| **Long cast** — takes your entire Action and cannot be part of a combo | **+2** |
| **Two-round cast** — interruptible; costs your Action for two rounds | **+3** |
| **Telegraphed** — straight-line only, or the target gets advantage to dodge | **+1** |
| **Situational** — requires water, darkness, open sky, a corpse, a nearby ally | **+1** |
| **Limited** — once per combat | **+2** |
| **Limited** — once per long rest | **+3** |
| **Tunnel vision** — you're blinded to everything but the target until your next turn | **+2** |
| **Fragile** — any damage taken during the cast cancels it, costs paid | **+2** |
| **Backlash** — on a natural 1, roll on the Backfire table | **+1** |
| **Escalating cost** — cost doubles each use in the same combat | **+2** |
| **Bloodprice** — costs Health instead of some Chakra | **+3** |

**Cap: a jutsu may take drawbacks worth no more than its base JP budget.** You can double your budget, not triple it.

---
---

### PART EIGHT — THE DEVELOPMENT PROCESS

#### Five Steps

##### 1. Concept
Declare it to your DM. Name it, describe what you're trying to do, and say **why your character wants it** — the answer to that question is usually where the drawback comes from.

##### 2. Research
Downtime study. Requires access to a library, a scroll collection, a teacher, or firsthand observation of something similar.

##### 3. Prototyping
Where it goes wrong. See the time and cost table below, and the **Backfire** table.

##### 4. Field Testing
The jutsu must be used successfully **three times in real combat** before it leaves prototype status. Prototypes carry an extra drawback of the DM's choosing until then.

##### 5. Naming
It's not finished until it has a name. Record it on your sheet at **Tier 0 — Learned**.

#### Time & Cost

| Rank | Development time | Ryō cost (materials, scrolls, training grounds) | Development check DC |
|---|---|---|---|
| **E** | 3 days | 500 | 10 |
| **D** | 1 week | 2,000 | 12 |
| **C** | 3 weeks | 8,000 | 14 |
| **B** | 6 weeks | 25,000 | 16 |
| **A** | 3 months | 80,000 | 18 |
| **S** | 6 months | 250,000 | 20 |

**Development check:** at the end of the development period, roll **Ninjutsu / Genjutsu / Taijutsu** (whichever matches the category) against the DC.

| Result | Outcome |
|---|---|
| **Success by 10+** | Works, and you may **immediately spend 1 Mastery Point** on it |
| **Success** | Works as designed |
| **Fail by 1–4** | Works, but with one additional DM-chosen drawback until you spend another development period |
| **Fail by 5–9** | Doesn't work. Half the time and cost is retained toward a retry. |
| **Fail by 10+** | Doesn't work, **and roll on the Backfire table** |

**Shadow clones reduce development time** by the same multiplier as training (Part Two), with the same strain.

#### Backfire Table (d10)

| d10 | Result |
|---|---|
| 1 | **Chakra rupture.** Lose 25% of your maximum Chakra until a long rest. |
| 2 | **Physical damage.** Take damage equal to the jutsu's Chakra cost. |
| 3 | **Pathway strain.** Disadvantage on all jutsu rolls for 1d4 days. |
| 4 | **Wrong nature.** The technique works, but as a different element. Keep it, or scrap it. |
| 5 | **Uncontrolled.** It works, but you cannot choose the target. |
| 6 | **Collateral.** It works, spectacularly, and destroys something you needed. |
| 7 | **Witnessed.** It works, and someone who shouldn't have seen it did. |
| 8 | **Instability.** It works, but on a natural 1–3 it targets you instead. |
| 9 | **Chakra scar.** Permanent −5 maximum Chakra. Cool scar. |
| 10 | **It works perfectly.** And you have no idea why, which means you can't teach it and can't evolve it. |

**Result 10 is the best entry on this table.** A technique the character genuinely does not understand is a campaign arc.

---
---

### PART NINE — WORKED EXAMPLES

#### Example 1: A D-rank creation

**"Ember Snare"** — a Genin with Fire affinity wants a technique that pins a target in place with a ring of flame.

**Budget:** D-rank = **4 JP**

| Spend | JP |
|---|---|
| Damage — 2 dice (d8 elemental) | 2 |
| Range — 30 ft | 1 |
| Condition rider — restrained | 2 |
| **Subtotal** | **5** |

Over budget by 1. Add a drawback:

| Drawback | JP back |
|---|---|
| Situational — requires flammable ground or debris | +1 |
| **Total** | **4 / 4** ✓ |

**Final:** Ember Snare (D) · 11 Chakra / 6 Stamina · 1 slot · 30 ft · 2d8 fire, CON save or restrained · *requires flammable ground.*

---

#### Example 2: Rebuilding the Rasengan

**Budget:** A-rank = **16 JP**

| Spend | JP |
|---|---|
| Damage — 8 dice | 8 |
| No hand seals | 3 |
| Movement effect — push 20 ft | 1 |
| Ignores cover (you're touching them) | 1 |
| Ignores resistance | 2 |
| Precision — no save, it just hits on a melee attack | 2 |
| **Total** | **17** |

One over. Take a drawback:

| Drawback | JP back |
|---|---|
| Telegraphed — melee range only, you must close the distance | +1 |
| **Total** | **16 / 16** ✓ ... *with 1 spare* |

**This is why the Rasengan is a good technique and a fair one:** enormous damage, no seals, no save — paid for by having to physically reach someone.

---

#### Example 3: Rebuilding the Chidori

**Budget:** A-rank = **16 JP** + drawbacks

| Drawback | JP back |
|---|---|
| Tunnel vision — blinded to all but the target until your next turn | +2 |
| Limited — twice per combat | +2 |
| Telegraphed — straight-line charge | +1 |
| **Budget becomes** | **21 JP** |

| Spend | JP |
|---|---|
| Damage — 10 dice (d10 piercing) | 10 |
| Ignores resistance | 2 |
| Ignores cover | 1 |
| Self-movement — dash up to 30 ft as part of the technique | 1 |
| Precision — melee attack, no save | 2 |
| Condition rider — stunned on a critical | 2 |
| Range step — 30 ft lunge | 1 |
| Lightning nature rider | 1 |
| **Total** | **20 / 21** ✓ |

**The drawbacks are the character.** Kakashi's tunnel vision is literally why he needed the Sharingan to use it safely — and that's a mechanical fact here, not just flavor.

---
---

### PART TEN — HOW JUTSU SPREAD

Creation isn't the only way to get a technique. These all matter for campaign play.

| Method | Requirement | Result |
|---|---|---|
| **Taught by a teacher** | The teacher has it at Proficient+ | Learn at Tier 0. Time per **Book IV §1**. |
| **From a scroll** | Literacy in the notation; a development check at the jutsu's DC | Learn at Tier 0. Failure wastes the scroll's first use. |
| **Sharingan copy** | 3-tomoe Sharingan; witness it used | Ninjutsu check DC 10 + 2 per rank step. **Cannot copy kekkei genkai or hiden.** Starts at Tier 0. |
| **Reverse-engineering** | Survive it three times; a development check at +2 DC | Half the normal development time |
| **Inheritance** | A clan technique, taught at the clan's discretion | Clan obligations apply — **Book II §2** |
| **Theft** | Steal the scroll. The Scroll of Seals is a capital offense. | Everything above, plus consequences |

#### Teaching your own creation

You may teach a jutsu you have at **Proficient or better**. Doing so:
- Takes the normal learning time for the student
- Grants **you** +5 Mastery XP in that jutsu (teaching sharpens it)
- Means it is now **out of your hands**

**That last line is a story.** Every technique in the setting that spread beyond its creator caused a problem — the Flying Thunder God, Edo Tensei, the Rasengan. Ask a player what they'd do if their signature move showed up in an enemy's hands.

---
---

### PART ELEVEN — QUICK REFERENCE

```
╔═══════════════════════════════════════════════════════╗
║  MASTERY TIERS                                        ║
║  0 Learned  │ 1 Practiced 10xp │ 2 Proficient 25xp    ║
║  3 Mastered 50xp │ 4 PERFECTED 100xp                  ║
║  → 1 Mastery Point per tier. Max 4 per jutsu.         ║
╠═══════════════════════════════════════════════════════╣
║  MASTERY XP                                           ║
║  Successful use +1 │ vs higher rank +2                ║
║  Creative use +3 │ Finishing blow +3 │ Under duress +2║
║  Cap 5 per jutsu per combat                           ║
║  Downtime: solo +2/day · teacher +4 · creator +6      ║
║  SHADOW CLONES MULTIPLY (×clones, with strain)        ║
╠═══════════════════════════════════════════════════════╣
║  UPGRADES (max 4 pts/jutsu)                           ║
║  Efficiency −15% Ch (×3) │ Conditioning −15% St (×3)  ║
║  Power +1 die (×2)  │ Precision +1 hit/DC (×2)        ║
║  Acceleration −1 slot (×2, T3+) │ Extension +50% (×2) ║
║  Control +1 target/round (×2) │ Seal-less (T3+)       ║
║  REACTIVE — cast as a Reaction 1/combat (T3+)         ║
╠═══════════════════════════════════════════════════════╣
║  CREATION BUDGET (Jutsu Points)                       ║
║  E 2 │ D 4 │ C 7 │ B 11 │ A 16 │ S 22                 ║
║  Drawbacks give JP back — max +100% of budget         ║
╠═══════════════════════════════════════════════════════╣
║  DEVELOPMENT                                          ║
║  E 3d/500 │ D 1w/2k │ C 3w/8k │ B 6w/25k              ║
║  A 3mo/80k │ S 6mo/250k                               ║
║  DC 10/12/14/16/18/20 · then 3 successful field uses  ║
╚═══════════════════════════════════════════════════════╝
```

---

#### DM Guidance

**Say yes to concepts, negotiate the numbers.** A player who wants to invent a technique is a player who's engaged with your setting. The budget exists so you can say "yes, and here's what it costs" instead of "no."

**Make them name it out loud.** Every jutsu in this world has a name people shout. If the player won't say it at the table, it isn't finished.

**Drawbacks are where character lives.** When a player picks *Bloodprice* or *Tunnel Vision*, ask why their character was willing to accept that. The answer is usually the best thing about the technique.

**Let mastery be visible.** When a Perfected jutsu comes out, describe it differently than you did fifty sessions ago. The player earned that.


---
---

# §4 — NPC & THREAT DESIGN

**This file replaces the earlier CR-based stat block file.** It is built on the printed rule that **NPCs do not follow player rules** (see Book IV §1, Part Eight).

> *"Their actions, abilities, and resources may reflect their situation, rank, experience, or importance to the story."*

So this file does not give you balanced encounters. It gives you **threat profiles** — what an enemy can do, how long they last, and what the party is actually supposed to achieve against them.

**[GM] applies to everything here** except quoted sheet text.

---
---

### PART ONE — THE FOUR ENEMY ROLES

Before statting anything, decide which of these an enemy is. This determines everything else.

| Role | Purpose | Can the party win? | Design priority |
|---|---|---|---|
| **Fodder** | Make the party feel strong; drain resources | Yes, easily | Numbers, not depth |
| **Rival** | A fair, winnable fight | Yes, with cost | Balance and counterplay |
| **Wall** | Teach the party they aren't ready | **No** — survival is the win | Overwhelming presence, an exit |
| **Story** | Challenge, delay, test, or teach | **Not the point** | Objective, not HP |

**Wall and Story enemies are the ones the printed guidance exists to protect.** Signal them clearly in the fiction — a flee-on-sight reputation, a Bingo Book entry marked *do not engage*, an NPC saying *"run."* Then let the players make an informed choice.

---
---

### PART TWO — THREAT PROFILES BY RANK

Use these as templates. **Adjust freely** — that's the point of the asymmetry rule.

#### Academy Student / Civilian Militia — *Fodder*
| | |
|---|---|
| **Health** | 10 |
| **AC** | 11 |
| **Movement** | 30 ft |
| **Resources** | Doesn't track. Assume 3 techniques total, then done. |
| **Actions** | 1 per turn (no combo) |
| **Damage** | 1d4+1 per hit |
| **Techniques** | E-rank only |

**Use:** crowds, hostages who fight back, a village's last line. Never as a real threat.

---

#### Genin — *Fodder to Rival*
| | |
|---|---|
| **Health** | 30 |
| **AC** | 13 |
| **Movement** | 30 ft |
| **Resources** | 100 Chakra / 100 Stamina, or just track "runs out after ~6 techniques" |
| **Actions** | Combo of 2 |
| **Damage** | 1d6+2 per hit |
| **Techniques** | E and D rank |
| **Save DC** | 12 |

**Use:** enemy squads of three. A rival genin cell is the best recurring antagonist in an Era A campaign.

---

#### Chūnin — *Rival*
| | |
|---|---|
| **Health** | 70 |
| **AC** | 15 |
| **Movement** | 35 ft |
| **Resources** | 180 / 180, or "~8 techniques" |
| **Actions** | Combo of 3 |
| **Damage** | 1d8+3 per hit |
| **Techniques** | Up to C rank |
| **Save DC** | 14 |
| **Special** | Substitution as a Reaction, twice per fight |

**Use:** squad leaders, checkpoint commanders, the Chūnin Exams tournament bracket.

---

#### Tokubetsu Jōnin — *Rival*
| | |
|---|---|
| **Health** | 100 |
| **AC** | 16 |
| **Movement** | 35 ft |
| **Actions** | Combo of 3 |
| **Damage** | 1d8+4 |
| **Techniques** | Up to B rank **within one specialty only** |
| **Save DC** | 15 |

**Design rule:** give them **one** thing they do better than the party's best, and make them mediocre at everything else. That contrast *is* the character.

---

#### Jōnin — *Rival to Wall*
| | |
|---|---|
| **Health** | 150 |
| **AC** | 17 |
| **Movement** | 40 ft |
| **Actions** | Combo of **4**, **plus one free Bonus Action technique per round** |
| **Damage** | 2d8+5 |
| **Techniques** | Up to B rank freely; **one A-rank signature per fight** |
| **Save DC** | 16 |
| **Special** | Substitution 3/fight; ignores resource costs on the first technique each round |

**Against a genin party this is a Wall.** Against a jōnin-rank party it's a Rival. Same block, different role — decided by the table, not the numbers.

---

#### ANBU — *Wall*
| | |
|---|---|
| **Health** | 170 |
| **AC** | 18 |
| **Movement** | 45 ft |
| **Actions** | Combo of **4** |
| **Damage** | 2d8+6, **plus 2d6 on a target that hasn't acted yet** |
| **Techniques** | Up to A rank |
| **Save DC** | 17 |
| **Special** | **Silent Killing** — in obscured conditions, an attack against an unaware target is an automatic critical. **Never fights alone.** |

**ANBU should feel like being hunted, not like a duel.** Open with an ambush the party can't win, then let them escape.

---

#### S-Rank / Akatsuki — *Wall*
| | |
|---|---|
| **Health** | 250 |
| **AC** | 19 |
| **Movement** | 45 ft |
| **Actions** | Combo of **5** |
| **Damage** | 3d8+7 |
| **Techniques** | A rank freely; **one S-rank per fight** |
| **Save DC** | 19 |
| **Special** | 3 "Resistances" per fight — auto-succeed on any save. **One signature gimmick that breaks a rule** (immortality, sand shield, Kamui intangibility, absolute defense). |

**The gimmick matters more than the numbers.** A party fights an Akatsuki member by figuring out the trick, not by out-damaging them. Give them the trick, let them work it out, and make the working-out the encounter.

---

#### Kage — *Wall to Story*
| | |
|---|---|
| **Health** | 400 |
| **AC** | 20 |
| **Movement** | 50 ft |
| **Actions** | Combo of **6**, plus **2 free actions at the end of other creatures' turns** |
| **Damage** | 4d8+8 |
| **Techniques** | S rank at will |
| **Save DC** | 21 |
| **Special** | 5 Resistances. **Reshapes the battlefield** — terrain changes at the start of each of their turns. |

**A Kage does not lose a straight fight to a player party.** If the party must beat one, it happens because of an objective, a sacrifice, an ally, or a trick — never because they dealt enough damage.

---

#### Legendary — *Story only*
Minato, Hanzō, Madara, a tailed beast, the Ten-Tails.

**Do not stat these.** Define instead:
1. **What they do each round** — one devastating thing, described, that the party responds to.
2. **What the party's actual objective is** — survive 5 rounds, reach the door, get the wounded out, land one specific hit, keep them talking.
3. **What ends the scene** — a timer, an arrival, a withdrawal, an objective met.

If you catch yourself tracking a legendary NPC's hit points, you've made a mistake. Track **rounds remaining** instead.

---
---

### PART THREE — SPECIAL ENEMY TYPES

#### White Zetsu — *Fodder, or Social Horror*
| | |
|---|---|
| **Health** | 35 |
| **AC** | 13 |
| **Actions** | 1 |
| **Damage** | 1d10+2 |

**Perfect Impersonation.** Assumes the exact form, voice, and surface memories of any humanoid it has touched. Detecting it requires an **Insight check at DC 18**, a **Byakugan (automatic)**, or negative-emotion sensing.
**Earth Merge.** Bonus Action to sink into any solid surface.

**Deploy two ways and never both at once:** twenty of them as an attrition wave, **or** exactly one, replacing an NPC the party trusts, for three sessions before anyone notices.

#### Edo Tensei — *a template, not a statline*

Apply to any profile above, then change three things:

1. **Cannot die.** Reduced to 0 Health, it fully regenerates at the start of its next turn.
2. **No resources.** Ignore Chakra and Stamina entirely. It casts freely, forever.
3. **Ends only by:** a sealing technique, total immobilization (buried, encased, bound), or the controller releasing it.

**Compelled but conscious.** Many reanimated shinobi are fighting their own bodies. A full scene of the party reaching one — **DC 20 Persuasion, and it should take the whole scene, not one roll** — can win a round of hesitation, a deliberate miss, or an outright refusal.

> **Design rule:** an Edo Tensei encounter **must have a non-combat win condition.** Give the party a sealing scroll, a fūinjutsu specialist, terrain that can bury it, or an emotional argument that lands. Without one the fight has no ending and the table will feel it.

#### Puppets & Constructs — *Fodder that scales*
| | |
|---|---|
| **Health** | 25 each |
| **AC** | 15 |
| **Damage** | 1d8+3, **plus poison** (CON save DC 15 or paralyzed 1 minute) |

The puppeteer is the real target. **Chakra threads have a range** — cut the line of sight or close the distance and the puppets drop. Every puppet fight should have that solution available and unstated.

#### Summons — *Terrain, not enemies*
A boss summon is a **battlefield event**. It changes the ground, blocks a route, or forces the party to fight somewhere new. Give it one attack that reshapes the map per round and let the actual fight happen around it.

---
---

### PART FOUR — BUILDING AN ENCOUNTER

#### Step 1 — Decide the role
Fodder, Rival, Wall, or Story. Write it down before anything else.

#### Step 2 — Set the objective
**This matters more than the enemy's stats.** Never make the objective "reduce them to 0" unless the fight is a Rival.

| Objective type | Example |
|---|---|
| **Survive** | Hold for 5 rounds until reinforcements |
| **Reach** | Get to the bridge, the scroll, the wounded |
| **Protect** | Keep the client alive; the enemy targets them, not you |
| **Deny** | Stop the ritual, the signal, the seal |
| **Escape** | Break contact and get out |
| **Learn** | Survive long enough to identify the gimmick |

#### Step 3 — Give it a clock
Rounds until reinforcements arrive, the poison takes hold, the ritual completes, the building collapses. **Naruto is a genre about time running out.**

#### Step 4 — Build the exit
Every Wall and Story encounter needs a visible way out. Signal it before the fight starts, or the party will assume there isn't one and fight to a TPK out of politeness.

#### Step 5 — Decide the cost
See **Book IV §5's Cost table**. Something should be spent even in victory.

---
---

### PART FIVE — SCALING ON THE FLY

The asymmetry rule means you can adjust mid-fight without cheating. Nobody is auditing an NPC's chakra bar.

**If the party is losing and shouldn't be:**
- The enemy's technique "costs more than expected" and they hesitate a round
- Reinforcements arrive for the party
- The enemy achieves their actual objective and withdraws — they were never trying to kill anyone
- A combo gets interrupted (Rule 5 works both directions)

**If the party is winning too easily:**
- The enemy was holding back; they open a gate, drop a mask, activate a dōjutsu
- A second enemy arrives
- The terrain changes
- The enemy switches from fighting to **completing their objective**, which is worse

**If the party flees:**
Let them. Print it on the wall if you have to: **"Retreat is not failure. Survival is a victory of its own."** A party that escapes a Wall and comes back at Chūnin rank to win is the single best arc this system produces.

---
---

### PART SIX — SIGNATURE GIMMICK LIBRARY

The most useful thing you can give a named enemy. Each of these is worth more than a hundred hit points.

| Gimmick | Effect | Counter the party can find |
|---|---|---|
| **Absolute defense** (sand, Susanoo) | Automatically negates the first hit each round | Overwhelm with speed or multiple attackers |
| **Intangibility** (Kamui) | Phases through one attack per round | Time it — they must solidify to attack |
| **Immortality** (Kakuzu, Hidan) | Multiple lives; drops but gets back up | Find the actual number and exceed it |
| **Water body** (Hōzuki) | Physical damage passes through | Lightning; or dehydrate them |
| **Mist / silent killing** | Attacks from concealment, automatic crits | Clear the mist, or fight by sound |
| **Poison** | The clock keeps running after they die | Get the antidote, or the antidote-maker |
| **Sealed chakra** (Gentle Fist) | Shuts down the party's techniques | Taijutsu; or don't get hit |
| **Puppet swarm** | Attacks from every angle | Cut the threads or reach the master |
| **Bloodline element** | Ignores an expected resistance | Learn what it actually is |
| **Reanimation** | Cannot be killed | Sealing, burial, or conversation |

**Rule of thumb:** every named enemy gets exactly one gimmick, and it must have a discoverable counter. The encounter is the party finding it.

---
---

### PART SEVEN — QUICK CONVERSION TABLE

For turning any character in **Book III §1–3** into a usable threat:

**Combo limits for every profile are consolidated in Book IV §2, Part Twelve.** Most NPC profiles sit one action below the equivalent PC rank — the players' combo ceiling is their edge, and everything else on the NPC sheet is the counterweight.

| Compendium description | Use this profile | Likely role |
|---|---|---|
| "Young shinobi," "genin," "child" | Genin | Fodder / Rival |
| "Squad leader," "chūnin" | Chūnin | Rival |
| "Specialist," "interrogator," "sensor" | Tokubetsu Jōnin | Rival |
| "Jōnin," "clan head," "commander" | Jōnin | Wall or Rival |
| "ANBU," "hunter-nin," "Root" | ANBU | Wall |
| "Missing-nin," "Akatsuki," "S-rank" | S-Rank | Wall |
| "Kage," "Sannin," "Hanzō" | Kage | Wall / Story |
| "Madara," "Minato," tailed beast | Legendary | **Story only** |

**Then add the gimmick.** The profile makes them functional; the gimmick makes them memorable.


---
---

# §5 — GM TOOLKIT

Tables, generators, campaign frames, and hooks. **All [GM].** Built for improvisation at the table.

---
---

### PART ONE — THE MISSION GENERATOR

Roll or choose one from each column. The combination usually suggests the whole mission.

#### d12 — Client

| d12 | Client |
|---|---|
| 1 | A merchant who is lying about his cargo |
| 2 | A minor daimyō's retainer, terrified and over-formal |
| 3 | The village mission desk, with a sealed scroll and no explanation |
| 4 | A civilian family who pooled everything to afford a D-rank |
| 5 | A rival village, under a joint-operation treaty nobody trusts |
| 6 | A monastery or shrine with a problem they won't name |
| 7 | A retired shinobi calling in an old favor |
| 8 | The Kage, personally — which means it is worse than the rank suggests |
| 9 | A missing-nin offering information for safe passage |
| 10 | A child who walked into the village alone |
| 11 | An intelligence handler who will not give their name |
| 12 | Nobody. The squad found the situation themselves. |

#### d12 — Objective

| d12 | Objective |
|---|---|
| 1 | Escort a person through hostile territory |
| 2 | Retrieve an object before someone else does |
| 3 | Destroy infrastructure — a bridge, a depot, a seal |
| 4 | Deliver a message that must not be read |
| 5 | Assassinate a specific individual |
| 6 | Capture a target alive |
| 7 | Reconnoiter an enemy position without engaging |
| 8 | Guard a location for a fixed period |
| 9 | Investigate the disappearance of another squad |
| 10 | Extract a defector or an embedded agent |
| 11 | Verify or disprove an intelligence report |
| 12 | Break a siege, a seal, or a genjutsu affecting an area |

#### d12 — Complication

| d12 | Complication |
|---|---|
| 1 | The mission is one rank higher than briefed |
| 2 | The client is the actual threat |
| 3 | An enemy squad has the identical objective |
| 4 | A squad member's personal history is directly involved |
| 5 | The target is a child, or someone the party will not want to kill |
| 6 | The intelligence is deliberately false, planted by their own side |
| 7 | Terrain or weather closes the route behind them |
| 8 | A named enemy from a previous mission has returned |
| 9 | Civilians are present and will not leave |
| 10 | A time limit is discovered mid-mission (poison, ritual, convoy) |
| 11 | Completing the mission requires breaking the shinobi code |
| 12 | The party is being observed and evaluated by their own village |

#### d8 — The Cost
*Every mission should spend something.*

| d8 | Cost |
|---|---|
| 1 | A technique is exposed to an enemy who will remember it |
| 2 | An NPC the party liked dies |
| 3 | The party's reputation with a faction drops |
| 4 | A piece of equipment or a summon contract is lost |
| 5 | The party learns something they'd rather not know about their own village |
| 6 | A PC's clan or family obligation is triggered |
| 7 | The mission succeeds and makes things worse |
| 8 | Someone the party spared comes back |

---
---

### PART TWO — NPC GENERATOR

#### d10 — Village of Origin
1–3 Konoha · 4 Suna · 5 Iwa · 6 Kumo · 7 Kiri · 8 Ame · 9 A minor country · 10 Missing-nin, village unclear

#### d10 — Specialty
1 Elemental ninjutsu · 2 Taijutsu · 3 Genjutsu · 4 Medical · 5 Sensor · 6 Weapons/kenjutsu · 7 Sealing · 8 Puppetry · 9 Summoning · 10 Poison

#### d12 — Defining Trait

| d12 | Trait |
|---|---|
| 1 | Speaks only when necessary, and then too bluntly |
| 2 | Compulsively cheerful, and it is armor |
| 3 | Superstitious about a specific ritual before missions |
| 4 | Treats every conversation as an interrogation |
| 5 | Openly resentful of a specific other village |
| 6 | Carries a photograph, a headband, or a name they won't explain |
| 7 | Chronically late and unbothered by it |
| 8 | Deeply religious in a world that mostly isn't |
| 9 | Talks about food constantly, including mid-combat |
| 10 | Refuses to use their clan's techniques |
| 11 | Formal to the point of stiffness with everyone, including friends |
| 12 | Cannot stop teaching, whether or not anyone asked |

#### d10 — What They Want
1 Promotion · 2 To protect a specific person · 3 To be forgiven · 4 Revenge on a named individual · 5 To leave the shinobi life entirely · 6 To surpass a rival · 7 Money, straightforwardly · 8 To find someone who disappeared · 9 To prove their clan's worth · 10 Nothing. They stopped wanting things.

#### d8 — Secret
1 They are a spy for another village · 2 They failed a mission and covered it up · 3 They carry a suppressed kekkei genkai · 4 They are Root · 5 They know something about a PC's past · 6 They are dying · 7 They have already defected in everything but paperwork · 8 They are a White Zetsu (Era C only)

---
---

### PART THREE — ENCOUNTER TABLES BY ERA

#### Era A — The Third War (d12)

| d12 | Encounter |
|---|---|
| 1 | An enemy scouting pair — they run rather than fight, and they report |
| 2 | A supply convoy, lightly guarded, that the party is not authorized to touch |
| 3 | A field hospital, overwhelmed, asking for any hands |
| 4 | The aftermath of a battle: survivors from *both* sides, all wounded |
| 5 | A trapped forest — explosive tags on a hundred trees |
| 6 | Refugees from a minor country, blocking the route |
| 7 | An enemy jōnin, alone, who offers a temporary truce |
| 8 | A sealed scroll on a dead courier — whose side's? |
| 9 | The party's own reinforcements, who are three days late and will not explain |
| 10 | An Iwa ambush using terrain the party can't counter |
| 11 | A ceasefire that both sides intend to break |
| 12 | A child in an enemy uniform |

#### Era B — The Interbellum (d12)

| d12 | Encounter |
|---|---|
| 1 | A bounty hunter with a Bingo Book and bad information |
| 2 | Bandits who used to be shinobi |
| 3 | An Akatsuki member passing through, entirely uninterested in the party |
| 4 | A Root operative shadowing the party's mission |
| 5 | A Kiri bloodline refugee seeking asylum |
| 6 | An Otogakure lab, abandoned in a hurry |
| 7 | A rogue experiment of Orochimaru's, loose |
| 8 | A village official taking a bribe |
| 9 | A dead hunter-nin, and a missing corpse |
| 10 | A genjutsu affecting an entire village, which nobody has noticed |
| 11 | An old Third War battlefield, still seeded with traps |
| 12 | Someone who recognizes a PC from a mission they shouldn't remember |

#### Era C — The Fourth War (d12)

| d12 | Encounter |
|---|---|
| 1 | A White Zetsu wearing a squadmate's face |
| 2 | A reanimated shinobi from the party's own village |
| 3 | A collapsed section of the line and no orders |
| 4 | Wounded from three different villages who won't be triaged together |
| 5 | A sealing team, out of scrolls |
| 6 | One of Naruto's shadow clones, arriving with news and leaving |
| 7 | A reanimated enemy who is trying to help |
| 8 | Enemy jinchūriki chakra on the horizon |
| 9 | A supply drop that landed in enemy territory |
| 10 | A Zetsu-infiltrated squad that has been reporting for two days |
| 11 | An order from HQ that the party's commander disagrees with |
| 12 | Silence — the mind-link has gone down |

---
---

### PART FOUR — CAMPAIGN FRAMES

#### Frame 1 — "The Kannabi Squad" *(Era A, Levels 1–8)*
**Premise:** A genin cell on the Iwa front, under a jōnin sensei who will not survive the campaign.
**Structure:** Six to eight missions of escalating cost, ending with a bridge, a supply line, or a mountain pass that decides the front.
**Themes:** The shinobi code vs. comrades. Children given adult authority.
**The turn:** Around session five, the sensei dies and a PC takes command mid-mission. Field-promote them on the spot.

#### Frame 2 — "The Mask" *(Era B, Levels 8–15)*
**Premise:** The party is ANBU. Their names are removed from the roster. Their missions do not exist.
**Structure:** Episodic black ops with a slow-building through-line: something inside Konoha is rotten, and the trail runs toward Root.
**Themes:** Loyalty to the village vs. loyalty to the truth.
**The turn:** One PC is offered a place in Root, with the tongue seal. Whether they accept is the campaign.

#### Frame 3 — "The Bloody Mist" *(Era B, Levels 5–12)*
**Premise:** Kirigakure. At least one PC carries a kekkei genkai and is hiding it.
**Structure:** Survive the purges, find the resistance, decide whether to fight for the village or destroy it.
**Themes:** A state at war with its own people.
**The turn:** They discover the Mizukage is not acting of his own will — and cannot prove it to anyone.

#### Frame 4 — "Third Division" *(Era C, Levels 10–18)*
**Premise:** One squad inside Kakashi's short-range division.
**Structure:** Four acts matching the war's reveals (**Book III §2, Part Five**). Keep them in one sector; the rest of the war arrives as news.
**Themes:** Unity between enemies. Fighting your own dead.
**The turn:** A squadmate is revealed as a White Zetsu — and has been for three sessions.

#### Frame 5 — "The Long Shadow" *(Cross-era, Levels 1–20)*
**Premise:** Start in Era A as genin. Timeskip to Era B as jōnin and ANBU. Land in Era C as division officers.
**Structure:** Three acts, two timeskips. Between acts, players write what their characters did in the intervening years, and the GM turns those answers into Era C's complications.
**Themes:** Consequence. The children you teach in Act Two fight beside you in Act Three.
**The turn:** An NPC the party spared in Act One is an antagonist in Act Three — or a reanimation in the enemy's front rank.

#### Frame 6 — "Bingo Book" *(Era B, Levels 6–16)*
**Premise:** The party are missing-nin. Their headbands are scratched. Everyone is hunting them.
**Structure:** A pursuit campaign — no home base, no resupply, no backup. Every village is hostile and every job is dirty.
**Themes:** What is a shinobi without a village?
**The turn:** Akatsuki notices them, and extends an offer.

---
---

### PART FIVE — ADVENTURE HOOKS

#### Era A
1. The squad's own supply depot is being resold to Iwa by someone in Konoha logistics.
2. An Iwa jōnin surrenders and asks for asylum — carrying the disposition of three fronts.
3. Rin's medical corps needs an escort to a village that no longer exists on any map.
4. A Konoha squad went silent in the Land of Grass; the party finds their gear, arranged neatly.
5. The party is ordered to *fail* a mission, and not told why.
6. Sakumo Hatake's old squadmate wants his name cleared, and has evidence.
7. Suna and Konoha both want the same water source. The party arrives to negotiate. So does a Suna squad.
8. A Kiri unit is escorting something in a sealed container through neutral territory.

#### Era B
1. A Konoha genin's forehead protector turns up in an Otogakure laboratory.
2. An Uchiha asks the party — quietly, deniably — what they think of the Hokage.
3. A hunter-nin's corpse-disposal seal fails, and a missing-nin's body is recovered intact.
4. Someone is buying Third War battlefield salvage at absurd prices.
5. An entire village has been under a genjutsu for two months and is content.
6. A Root operative approaches a PC with a mission the Hokage has explicitly forbidden.
7. Yugakure's spa town has a body problem, and a Jashinist.
8. Jiraiya needs someone expendable to check a lead in the Land of Rain.

#### Era C
1. The sealing scrolls in the party's sector have been swapped for blanks.
2. A reanimated shinobi from the party's village is asking for them by name.
3. Two divisions have received contradictory orders, both apparently from HQ.
4. A Zetsu impostor has been feeding the mind-link false reports for a day and a half.
5. The party must escort a Hyūga sensor to the front — and the sensor is nine years old.
6. An Iwa squad refuses to take an order from a Konoha commander, in the middle of an engagement.
7. A reanimated Akatsuki member offers a trade: information for a clean sealing.
8. The party finds a survivor from a squad that was reported wiped out — and cannot verify them.

---
---

### PART SIX — BINGO BOOK ENTRIES **[GM template]**

Hand these out as props. Note that Bingo Books are **reliable for identity and unreliable for capability** — perfect for generating dangerous overconfidence.

```
────────────────────────────────
NAME:          [Name]
ORIGIN:        [Village] — DEFECTED [year]
THREAT RATING: [A / S]
BOUNTY:        [amount] ryō
KNOWN ABILITIES:
  • [Two or three techniques — deliberately incomplete]
LAST CONFIRMED SIGHTING:
  [Location, and how long ago]
STANDING ORDER:
  [ ] Capture alive
  [ ] Eliminate and dispose of remains
  [ ] Do not engage — report only
NOTES: [One line of dangerously outdated information]
────────────────────────────────
```

**Sample "Notes" lines that will get someone killed:**
- *"Relies exclusively on Water Release. Fire users recommended."*
- *"Operates alone."*
- *"Believed to be at reduced capability following injury."*
- *"Non-combatant. Support classification."*

---
---

### PART SEVEN — SESSION ZERO

#### Decide as a table
1. **Which era.** This determines everything, especially what NPCs can say (**Book III §4**).
2. **What the party is.** A genin cell, an ANBU unit, a mixed Allied squad, missing-nin.
3. **Village and clan spread.** All one village is simplest. Mixed-village works well in Era C and is *very* hard in Era A.
4. **Tone.** *Naruto* runs from broad comedy to genuine atrocity, often in the same chapter. Agree how far each way you're going.
5. **Dōjutsu and jinchūriki.** Both are strong. Both are campaign-defining. Decide before, not during.

#### Lines to establish
The setting includes child soldiers, state-sanctioned massacre, forced human experimentation, hereditary slave-marking, and mass civilian death. **None of that is incidental — it's the setting's argument.** Agree what the table wants on screen and what stays off it.

#### Ask each player three questions
1. **Who taught you?** Every shinobi has a sensei. Name them; the GM will use them.
2. **What did the war take from you?** In Era A this is present tense. In Era C it's the reason they enlisted.
3. **What would make you break the code?** Write it down. The campaign will come for it.

---
---

### PART EIGHT — RUNNING IT WELL

#### Five things that make a Naruto game feel right

1. **Fights are short and cost something.** Three to four rounds. Someone spends a resource they wanted to keep.
2. **The flashback is a legitimate move.** Mid-combat, cut to why this matters. It's the genre's signature and it works at the table.
3. **Talk to your enemies.** Half the setting's conflicts resolve through conversation *during* the fight. Let the party try. Sometimes let it work.
4. **Every technique has a name, and people say it.** This is not optional. Have NPCs announce their jutsu.
5. **Teachers die and students continue.** The generational handoff is the whole thesis. Build at least one into every campaign.

#### Two things to avoid

1. **Don't let the famous characters solve it.** Minato, Itachi, and Madara should be weather, not cavalry.
2. **Don't explain the secrets.** See **Book III §4**. The setting's power comes from what people don't know, and the reveals only land if the ignorance was played honestly.

#### Mandatory Arc Beats **[GM — standing rule]**

Every session, or every major narrative arc if a session runs light, needs **1–2 dedicated spotlight moments per PC** that actively move their individual storyline forward — **without the player having to be the one who brings it up.** The GM carries this, not the table. A player shouldn't have to lobby for their own arc to get screen time.

Current PCs and what their beat looks like:

- **Ardo — The Seam.** Proactively seed environmental hints, visions, or NPC interactions tied to what's sealed in him. Ardo's player doesn't carry the burden of raising it alone — see Book III/`characters/ardo.md` Part Six.
- **Souji — Bloodline & Transformation.** Include active triggers, physical symptoms, lore drops, or encounters that test, hint at, or develop the Senju thread and the still-uncontrolled awakening — see `characters/souji.md` Part Ten.
- **Suzume — Sharingan & Arc.** Give her specific narrative challenges, emotional beats, or combat realizations that force her to grapple with the evolution, cost, and lore of the Sharingan — see `characters/suzume.md`.

This is a floor, not a ceiling — players can still initiate their own arc moments same as always. It just means the GM never gets to leave a PC's thread untouched for a full session because nobody happened to ask.

---
---
