# PC SHEET — [NAME]

> **This sheet carries identity, fixed statistics, permanent traits, and an index of what they can do.**
> It carries **no current values** and **no technique mechanics.**

| Need | File |
|---|---|
| **Current Chakra / Stamina / Health / Special / conditions** | **`campaign/campaign-state.md`** |
| **Technique costs, damage, DCs, ranges** | **`[name]-jutsu.md`** |
| **Transformations, dōjutsu, bloodline systems** | **`[name]-transformations.md`** |
| **Goals, knowledge, relationships, threads, history** | **`[name]-story.md`** |

**Sourcing:** `[SHEET]` · `[INF]` · `[GM]` · `[CONFLICT]` · `[DECISION NEEDED]`. Legend: `ARCHITECTURE.md` §1.

---
---

# PART ONE — IDENTITY

| Field | Value |
|---|---|
| **Name** | |
| **Age** | |
| **Rank** | *Rank · Level N* |
| **Village** | |
| **Unit** | |
| **Clan** | *and whether it is known to whom* |
| **Body Origin** | *Indra / Ashura* |
| **Nature affinity** | |
| **Sensei of record** | |
| **Appearance** | |

*A short paragraph on who they are right now — not their whole history. History belongs in the story tracker.*

---
---

# PART TWO — CORE STATISTICS

## Attributes `[SHEET]`

*27-point buy. Applied on top: [clan bonuses] · [Body Origin].*

| Attribute | Score | Mod | Governs |
|---|---:|---:|---|
| **STR** | | | |
| **DEX** | | | |
| **CON** | | | |
| **INT** | | | |
| **WIS** | | | |
| **CHA** | | | |

## Resource maxima `[SHEET]`

*Book IV §1 Part Seven formulas. **Current values are in `campaign/campaign-state.md`.***

| Resource | Max | Working |
|---|---:|---|
| **Chakra** | | 100 + 20×(Level−1) + 10×CON mod → Body Origin → clan multiplier |
| **Stamina** | | 100 + 20×(Level−1) + 10×CON mod → Body Origin |
| **Health** | | 30 + 10×(Level−1) + (2 × CON mod × Level) |
| **Special** | 0 / **100** | Starts empty, fills |
| **Defense** | | 10 + DEX |
| **Initiative** | | DEX |
| **Movement** | 30 ft | |
| **Proficiency** | | By level |

> **Never hand-patch a derived number.** Change the input and recompute. Continuity patches that pin an old value are how sheets rot.

## Save DCs `[SHEET]` — *DC = 8 + proficiency + governing attribute*

| Discipline | Governing | DC |
|---|---|---:|
| **Ninjutsu** | INT | |
| **Taijutsu** | STR *or* DEX — locked to ___ | |
| **Genjutsu** | CHA | |
| **Medical** | WIS | |

---
---

# PART THREE — SKILLS & PASSIVES

| Skill | Bonus | Source |
|---|---:|---|

## Passives

**[NAME]** `[SOURCE TAG]` — effect.

---
---

# PART FOUR — COMBO & ACTION ECONOMY `[SHEET]`

**Combo limit: N slots (Rank). Max jutsu rank: ___.**

| Basic / E / D | C / B | A | S |
|---|---|---|---|
| **1 slot** | 2 slots | 3 slots | 4 slots |

**Chain Momentum · Interruption (Rule 5) · Counter Window · Clash · Overcharge:** standard, Book IV §2. *Note any character-specific variation here, or state that there is none.*

| Reaction | Cost | Notes |
|---|---|---|
| **Substitution** | 8 Ch / 5 St | Native Reaction |
| **Brace** | 8 St | Reduce one action by 1d6 + CON |

---
---

# PART FIVE — CAPABILITY INDEX

> **Names and ranks only.** All mechanics in `[name]-jutsu.md`.

| Technique | Rank | Slots |
|---|---|---|

## Transformations — `[name]-transformations.md`

| Form | Status |
|---|---|

## Permanent conditions

| | |
|---|---|

---
---

# PART SIX — EQUIPMENT

| Item | Count | Notes |
|---|---:|---|

**Ryō: see `campaign/campaign-state.md`.**

---
---

# APPENDIX — FAST REFERENCE

```
[NAME] · RANK · Level N · age N · Village · Unit
[clan] · [Body Origin] · [nature]

STR __ (+_)   DEX __ (+_)   CON __ (+_)
INT __ (+_)   WIS __ (+_)   CHA __ (+_)        Prof +_

CHAKRA  ___      STAMINA ___      SPECIAL 0/100
HEALTH  ___      DEFENSE  __      INIT +_      MOVE 30 ft

DC — Ninjutsu __ · Taijutsu __ · Genjutsu __ · Medical __
COMBO _ slots · MAX RANK _

── COMBAT KIT ───────────────────────────────────────
name              rank  cost    action    effect summary

── WHERE EVERYTHING ELSE LIVES ──────────────────────
  [name]-jutsu.md · [name]-transformations.md · [name]-story.md
  campaign/campaign-state.md   EVERY CURRENT VALUE. Read it first.
```
