# PC SHEET — SUZUME

> **This sheet carries identity, fixed statistics, permanent traits, and an index of what she can do.**
> It carries **no current values** and **no technique mechanics.**

| Need | File |
|---|---|
| **Current Chakra / Stamina / Health / Special / conditions** | **`campaign/campaign-state.md`** |
| **Technique costs, damage, DCs, ranges** | **`suzume-jutsu.md`** |
| **Sharingan, Mangekyō techniques, dōjutsu trees, Sōgan** | **`suzume-transformations.md`** |
| **Goals, knowledge, relationships, threads, session history** | **`suzume-story.md`** |

> ## ⚠ THIS SHEET WAS REBUILT BY THE ARCHITECTURE AUDIT.
> The previous version carried **three unreconciled strata** — Level 1, Level 5 and Level 13 text all live simultaneously, contradicting each other on her age, her rank ceiling, her Sharingan stage, her Medical capability, her Genjutsu proficiency and her unlocked tiers. **Every contradiction is resolved and documented** in `suzume-jutsu.md` and `suzume-transformations.md` under *Corrections Applied*.

---
---

# PART ONE — IDENTITY

| Field | Value |
|---|---|
| **Name** | **Suzume** — *sparrow* |
| **Age** | **27** |
| **Rank** | **Jōnin · Level 13** |
| **Village** | Konohagakure |
| **Unit** | **遊撃班 Yūgekihan.** *(Formerly Cell 409.)* **Field medic** |
| **Clan** | **UCHIHA by blood.** Clanless on every document that exists. **The clan has never claimed her** — not at birth, not through the unexplained migraines, not when her eyes opened over Rai Inuzuka's body |
| **Body Origin** | **Body Origin — Uchiha-aligned.** Blood and origin point the same direction |
| **Nature affinity** | **Lightning (雷 / Raiton)** |
| **Dōjutsu** | **MANGEKYŌ SHARINGAN — right eye.** Left socket carries **Ardo's transplanted ordinary eye** |
| **Specialty** | **War medic · genjutsu · precision Lightning · predictive taijutsu** |

## Who she is now

**Thirteen years a war medic**, and war medics are not gentle people. The girl who ran three kilometres for help because she was not strong enough is a long way behind her.

She lost a patient in Year −10 on a table she built out of a door. **She stopped keeping count in Year −8**, which she later described as the worst decision she ever made.

**In Year −6 she kept Rokka Uehara alive for six days in a cave.** He survived and never returned to the front.

---
---

# PART TWO — CORE STATISTICS

## Attributes `[SHEET]` — *27-point buy*

| Attribute | Score | Mod | Governs |
|---|---:|---:|---|
| **STR** | 10 | **+0** | Physical force — *deliberately her weakness* |
| **DEX** | 14 | **+2** | Speed, agility, hand seals, taijutsu |
| **CON** | 12 | **+1** | Durability, stamina, chakra |
| **INT** | 14 | **+2** | Ninjutsu, analysis |
| **WIS** | 15 | **+2** | Perception, **medical** |
| **CHA** | 16 | **+3** | Presence, **genjutsu** — *was 11. Eight years, and a nightmare she built herself* |

## Resource maxima `[SHEET]`

*Book IV §1 Part Seven formulas. **Current values are in `campaign/campaign-state.md`.***

| Resource | Max | Working |
|---|---:|---|
| **Chakra** | **350** | 100 + 20×12 + 10×CON 1 |
| **Stamina** | **350** | 100 + 20×12 + 10×CON 1 |
| **Health** | **176** | 30 + 10×12 + (2 × 1 × 13) |
| **Special** | 0 / **100** | Starts empty, fills |
| **Defense** | **12** | 10 + DEX |
| **Initiative** | **+2** | DEX |
| **Movement** | **30 ft** | Standard |
| **Proficiency** | **+5** | Level 13 |

> **[RESOLVED]** The old sheet retained a **"Health Continuity Ruling"** pinning her at **35 Health** — a Level-1 value held to avoid disturbing an encounter that ended thirteen years ago. **It is void.** So are the "LIVE COMBAT SNAPSHOT" lines showing 110/110 Chakra. **Never hand-patch a derived number; change the input and recompute.**

## Save DCs `[SHEET]` — *DC = 8 + proficiency + governing attribute*

| Discipline | Governing | DC |
|---|---|---:|
| **Ninjutsu** | INT | **15** |
| **Taijutsu** | DEX | **15** |
| **Genjutsu** | CHA | **16** |
| **Medical** | WIS | **15** |

---
---

# PART THREE — SKILLS & PASSIVES

| Skill | Bonus | Source |
|---|---:|---|
| **Genjutsu** | **+8** | CHA +3 · prof +5 — **her actual specialty** |
| **Medical** | **+7** | WIS +2 · prof +5 — **war medic, thirteen years** |
| **Taijutsu** | **+7** | DEX +2 · prof +5 |
| **Stealth** | **+7** | DEX +2 · prof +5 |
| **Perception** | **+7** | WIS +2 · prof +5 |
| **Shurikenjutsu** | **+7** | DEX +2 · prof +5 |
| Strategy | +2 | INT, not proficient |

## Passives

**UCHIHA CLAN TRAIT** `[SHEET]` — **Advantage on sight-based Perception checks.** Grants the Sharingan progression. **No raw attribute modifier.**

**CLINICAL PRECISION** `[GM — formalized]` — When she has time to calmly assess rather than react to a surprise, **advantage on Medical and Perception checks.**

---
---

# PART FOUR — COMBO & ACTION ECONOMY `[SHEET]`

**Combo limit: 5 slots (Jōnin).** **Max jutsu rank: B, plus one A-rank signature** — her signature is **無戸の間 Muto no Ma.**
After any combo she still gets **one Bonus Action and one Reaction.**

| Basic / E / D | C / B | A | S |
|---|---|---|---|
| **1 slot** | 2 slots | 3 slots | 4 slots |

> **⚠ One element-specific restriction, and it is deliberate:** **no Lightning Release technique above C-rank.** This is **not** a rank ceiling — she is Jōnin, and her genjutsu and medical work run to A- and B-rank. It applies to Lightning only, so her Lightning stays a scalpel.

**Chain Momentum · Interruption (Rule 5) · Counter Window · Clash · Overcharge:** standard, Book IV §2. No character-specific variation. **Pushing through an interruption costs 30 Special or a feature. There is no free save.**

**Reactions** — usable at any moment, one per round.

| Means | Cost | Notes |
|---|---|---|
| **Substitution** | 8 Ch / 5 St | Native Reaction. Her primary escape |
| **Brace** | 8 St | Reduce one action by **1d6 + 1** (CON) |
| **Sharingan Reaction** | 3 Ch/round upkeep | **Impose disadvantage on one enemy attack** |

## GOING BEYOND `[GM]`

She may overdraw one resource to **zero** and pay the shortfall from **Health at 4:1.** The resource hitting 0 is an Interruption — her turn ends and she is **Exhausted** until she rests.

---
---

# PART FIVE — CAPABILITY INDEX

> **Names and ranks only.** All mechanics in **`suzume-jutsu.md`** and **`suzume-transformations.md`**.

## Techniques

| Jutsu | Rank | Slots |
|---|---|---|
| Clone · Transformation · Substitution · Rope Escape | E | 1 |
| Body Flicker · Leaf Whirlwind | D | 1 |
| Basic Taijutsu / kunai | — | 1 |
| **PT-TAI-01 Mirrored Opening** | *unranked* | 1 |
| **雷遁・脈糸 Pulse Thread** *(+ Split Current)* | D | 1 |
| **脈錠 Nerve Lock** | C | 2 |
| **灯無 Summoning — 宵 Yoi** | C | 2 |
| **断脈 Danmyaku · "Severed Pulse"** | **B** | 2 |
| **無戸の間 Muto no Ma · "The Doorless Room"** | **A — SIGNATURE** | 3 |

**Medical ninjutsu — full.** Diagnosis, triage, surgical and chakra-based repair, stabilisation. **Advantage on all Medical checks with 癒し眼 Iyashime open.**

## Dōjutsu — `suzume-transformations.md`

| | Status |
|---|---|
| **万華鏡写輪眼 Mangekyō Sharingan**, right eye | **AWAKENED, Session Eight** |
| **迎え火 Mukaebi** | **BUILT.** The lamp |
| **無戸の間 Muto no Ma** | **BUILT.** The same room with the lamp taken out |
| **Her tree** — 見立て Mitate · 癒し眼 Iyashime | **I–II UNLOCKED.** III (Sharingan Genjutsu) and IV (**静かな部屋 The Quiet Room**) **LOCKED** |
| **相眼 Sōgan** — 血染み · 合わせ目 · 遠見 | **I–III UNLOCKED.** IV (一心 Isshin) **LOCKED** |

> ## ★ SHE HAS NO VISION TRACK AND WILL NEVER GO BLIND.
> Native tissue, native body, awakened correctly. **Ardo pays for both of them.** Her tiers cost him nothing; the shared Sōgan tree costs him all of it.

---
---

# PART SIX — EQUIPMENT

| Item | Count | Notes |
|---|---:|---|
| Kunai | ~10 | |
| Shuriken | ~15 | |
| **Medical kit** | 1 | Field dressing and supplies. **Thirteen years of restocking** |
| Case notes | 1 set | Long-term medical / migraine observations, kept since before the awakening |
| Headband | 1 | Konohagakure |

**Ryō: see `campaign/campaign-state.md`.** *(Flagged there as stale.)*

---
---

# APPENDIX — FAST REFERENCE

```
SUZUME · JŌNIN · Level 13 · age 27 · Konohagakure · 遊撃班
Uchiha by blood, clanless on paper · Lightning 雷 · WAR MEDIC
MANGEKYŌ SHARINGAN, right eye · Ardo's ordinary eye, left socket

STR 10 (+0)   DEX 14 (+2)   CON 12 (+1)
INT 14 (+2)   WIS 15 (+2)   CHA 16 (+3)        Prof +5

CHAKRA  350      STAMINA 350      SPECIAL 0/100
HEALTH  176      DEFENSE  12      INIT +2      MOVE 30 ft

DC — Ninjutsu 15 · Taijutsu 15 · GENJUTSU 16 · Medical 15
COMBO 5 slots (Jōnin) · MAX RANK B + one A-signature (無戸の間)
   ↳ LIGHTNING ONLY is capped at C-rank. Deliberate. Not a rank ceiling.

SKILLS  Genjutsu +8 · Medical +7 · Taijutsu +7
        Stealth +7 · Perception +7 · Shurikenjutsu +7

PASSIVES
  Uchiha Clan Trait — advantage on sight-based Perception
  Clinical Precision — advantage on calm Medical/Perception assessment
  Sharingan — adv. vs genjutsu · reads hand seals
              Reaction: disadvantage on one enemy attack · 3 Ch/round

── COMBAT KIT ───────────────────────────────────────
Basic Taijutsu        —   —        Action   +7 hit, 1d6
Mirrored Opening      —   —        Action   +7, ADV if target already acted
                                             on hit: costs them tempo
Pulse Thread          D   8/5      Action   1d8 Ltg, CON 15 or −10ft & no Reaction
  ↳ Split Current     D   —        two pulses, or two targets within 10 ft
Nerve Lock            C  15/9      Action   2d8 Ltg, CON 15 or Slowed, 45 ft, 2 slots
Summoning · 宵 Yoi     C  20/10     Action   silent recon · DIAGNOSTIC LISTENING
                                             she tells you everything she finds
断脈 DANMYAKU          B  35/18     Action   cuts what's UNDER the skin. No wound.
                                             The limb stops being a limb. 2 slots
無戸の間 MUTO NO MA    A  40 Special Action   SIGNATURE. Eye contact, CHA vs DC 16.
                                             A perfect safe room with NO DOOR.
                                             Nothing happens. That is the technique.
                                             Only breakable from OUTSIDE. 3 slots
迎え火 MUKAEBI         —  Special    —        THE LAMP. Reaches a mind that can't be
                                             reached. She is a light, not a hand.
                                             8 Ch/round upkeep. Hostile minds refuse.

REACTIONS  one per round, usable at any moment
  Substitution 8 Ch / 5 St · Brace 8 St → reduce one action by 1d6+1
  Sharingan → impose disadvantage on one enemy attack
GOING BEYOND  overdraw to 0, shortfall from Health at 4:1

INTERRUPTION  prone / silenced / stunned / grappled / blinded /
              any resource at 0  →  COMBO ENDS
              push through: 30 Special or a feature. No free save.

** NO VISION TRACK. SHE WILL NEVER GO BLIND. ARDO PAYS. **

── WHERE EVERYTHING ELSE LIVES ──────────────────────
  suzume-jutsu.md ............ every technique's real numbers
  suzume-transformations.md .. Sharingan · Mukaebi · 無戸の間 · trees
  suzume-story.md ............ goals · KNOWLEDGE LEDGER · threads
  campaign/campaign-state.md   EVERY CURRENT VALUE. Read it first.
```
