# SHINOBI CHRONICLES — PROJECT ARCHITECTURE

**Read this first.** It tells you which file owns which fact, which file wins when two disagree, and where to write when the game state changes.

This is a **modular knowledge system**, not a pile of documents. Every mechanic has exactly one authoritative home. Every other mention of it is a pointer.

---
---

# 1. THE AUTHORITY LADDER

When two files disagree, the **higher tier wins**. No exceptions, no interpretation.

| Tier | Authority | Files | Governs |
|---:|---|---|---|
| **1** | **CORE RULES** | `compendium/book-4-the-game.md` | Every general mechanic: resources, action economy, combos, clashes, DCs, damage, conditions, mastery, jutsu creation, NPC design. **If Book IV says it, that is the rule.** |
| **2** | **SETTING MECHANICS** | `compendium/book-1-world.md` · `book-2-power-bloodline.md` · `book-3-people-secrets.md` | Subsystems Book IV delegates *by name*: clan rosters, jinchūriki, senjutsu, curse marks, summons, equipment, information horizons. Authoritative **only where Book IV explicitly defers**. |
| **3** | **TECHNIQUE DATA** | `jutsu-compendium/*` | Canonical rank, Japanese name, and description of every existing technique. Never invent a rank — look it up here. |
| **4** | **CHARACTER MECHANICS** | `characters/<name>-jutsu.md` · `characters/<name>-transformations.md` | One PC's techniques and forms. May **override Tier 1–3 for that character only**, and must say so explicitly with a reason. |
| **5** | **CHARACTER STATE** | `characters/<name>.md` | Who they are, what they can do, what is permanently true of them. Points outward for detail. |
| **6** | **LIVE STATE** | `campaign/campaign-state.md` | Current values only. Never rules. **Overrides every sheet's printed "current" number, always.** |
| **7** | **NARRATIVE RECORD** | `campaign/session-log.md` · `characters/<name>-story.md` · `campaign/npcs.md` | What happened, what each character knows, who they know. **Carries no mechanical authority.** |
| **—** | **DERIVED / NON-AUTHORITATIVE** | `compendium/book-0-index.md` · `CUSTOM_INSTRUCTIONS.md` · `README.md` | Convenience summaries. **These never win an argument.** If one disagrees with Book IV, Book IV is right and the summary is stale — fix it. |

## The character-override rule

A character file may contradict Book IV **only** when all three hold:

1. It is tagged **[GM]** or **[GM — formalized]**.
2. It states plainly what general rule it is overriding.
3. The override is scoped to that character.

Everything else in a character file is subordinate to Book IV. A character sheet that quietly restates a general rule with different numbers is **stale, not an override** — correct it to match Book IV.

## Sourcing tags — unchanged, used project-wide

| Tag | Meaning |
|---|---|
| **[SHEET]** | Printed on an official sheet, or derived directly from Book IV. Authoritative. |
| **[M]** / **[DB]** | Manga canon / Japanese databook. |
| **[A]** / **[MV]** / **[N]** | Anime-only / movie-only / novel. |
| **[INF]** | Reasonable extrapolation, not directly stated. |
| **[GM]** | Table ruling — homebrew, not canon. |
| **[CONFLICT]** | Sources disagree; both readings preserved, deliberately unresolved. |
| **[DECISION NEEDED]** | A genuine ambiguity this audit could not resolve. **Requires a human ruling.** Never silently resolved. |

---
---

# 2. STATIC vs DYNAMIC — the single most important split

**Static** = rules, definitions, technique mechanics, lore, permanent traits. Changes only when the *design* changes.
**Dynamic** = anything that changes during play.

> ## Every dynamic value lives in `campaign/campaign-state.md` and nowhere else.

| Data | Owner | Everyone else |
|---|---|---|
| Max Chakra / Stamina / Health, and the formula | Character sheet | — |
| **Current** Chakra / Stamina / Health / Special | **`campaign/campaign-state.md`** | Do not print a current value on a sheet |
| Attributes, proficiency, DCs, Defense | Character sheet | — |
| A technique's cost, damage, range, effects | `<name>-jutsu.md` | Sheet lists **name + rank only** |
| A technique's **current mastery tier and XP** | **`campaign-state.md`** | Jutsu file lists the ladder, not the position on it |
| Transformation mechanics, costs, drawbacks | `<name>-transformations.md` | Sheet lists **name + owned/locked** |
| **Which transformation is active right now** | **`campaign-state.md`** | — |
| Ardo's Vision economy (the rules) | `ardo-transformations.md` | — |
| **Ardo's current Vision meter** | **`campaign-state.md`** | — |
| Current injuries, conditions, ryō | **`campaign-state.md`** | — |
| What a character knows | `<name>-story.md` | — |
| What happened in a session | `campaign/session-log.md` | Story trackers summarise *that character's* slice |

**Why this matters:** before this audit, Suzume's current Chakra appeared in four places with three different values, and Ardo's Vision loss rate was printed as "−1 per day" in one file and "−1 per month" in another. Both are the class of error this split exists to make impossible.

---
---

# 3. THE FILE MAP

```
campaigns/shinobi-chronicles/
│
├── ARCHITECTURE.md ................ THIS FILE. Authority ladder + navigation.
├── README.md ...................... Repo orientation. Points at campaign-state for status.
├── CUSTOM_INSTRUCTIONS.md ......... GM system prompt. Points at files; does not restate rules.
│
├── compendium/ .................... STATIC — rules and setting
│   ├── book-0-index.md ............ Quick-reference tables. DERIVED, non-authoritative.
│   ├── book-1-world.md ............ §1 Timeline · §2 Geography · §3 Politics · §4 Shinobi System
│   ├── book-2-power-bloodline.md .. §1 Chakra/Power · §2 Clans · §3 Tailed Beasts · §4 Summons & Gear
│   ├── book-3-people-secrets.md ... §1 Era A cast · §2 Era C cast · §3 Orgs · §4 Information Horizons
│   └── book-4-the-game.md ......... ★ TIER 1 RULES AUTHORITY
│
├── jutsu-compendium/ .............. STATIC — canonical technique data by rank
│   ├── 01-e-rank.md ... 07-outside-the-ranks.md
│   └── expansions/
│
├── characters/ .................... Per-PC. Four files each, one job each.
│   ├── ardo.md ......................... SHEET — identity, stats, current capability index
│   ├── ardo-jutsu.md ................... ★ authoritative for Ardo's techniques
│   ├── ardo-transformations.md ......... ★ authoritative for Ardo's forms, dōjutsu, Vision, Arakawa
│   ├── ardo-inheritance.md ............. the estate, the archive, the trustee, what is sealed
│   ├── ardo-story.md ................... goals · knowledge · relationships · consequences · threads
│   ├── suzume.md / -jutsu / -transformations / -story
│   ├── souji.md  / -jutsu / -transformations / -story
│   └── _TEMPLATE-sheet.md · _TEMPLATE-jutsu.md · _TEMPLATE-transformations.md · _TEMPLATE-story.md
│
└── campaign/ ...................... DYNAMIC + shared narrative
    ├── campaign-state.md .......... ★ TIER 6 — the only place live values live
    ├── session-log.md ............. Canonical shared session spine
    ├── npcs.md .................... NPC roster, deduplicated
    └── archive/
        └── squad-two-journey.md ... CLOSED. Historical log, superseded.
```

## Naming convention

`characters/<name>.md` is the sheet. `characters/<name>-<aspect>.md` is a specialist file for that character. Kebab-case throughout, matching the compendium.

*(If you are looking for the files as named in the original refactor brief: `[Character]_Jutsu.md` → `<name>-jutsu.md`; `[Character]_Transformations.md` → `<name>-transformations.md`; `[Character]_Story_Tracker.md` → `<name>-story.md`.)*

---
---

# 4. HOW THE FILES CONNECT

```
                    ┌──────────────────────────┐
                    │   book-4-the-game.md     │  TIER 1 — every general rule
                    └────────────┬─────────────┘
                                 │ delegates named subsystems to
                    ┌────────────▼─────────────┐
                    │  book-1 / book-2 / book-3│  TIER 2 — setting mechanics + lore
                    └────────────┬─────────────┘
                                 │ techniques looked up in
                    ┌────────────▼─────────────┐
                    │    jutsu-compendium/     │  TIER 3 — canonical technique data
                    └────────────┬─────────────┘
                                 │ instantiated per character by
   ┌─────────────────────────────▼──────────────────────────────┐
   │  <name>-jutsu.md          <name>-transformations.md        │  TIER 4
   └─────────────────────────────┬──────────────────────────────┘
                                 │ indexed by
                    ┌────────────▼─────────────┐
                    │       <name>.md          │  TIER 5 — the sheet
                    └────────────┬─────────────┘
                                 │ live values read from
                    ┌────────────▼─────────────┐
                    │  campaign-state.md       │  TIER 6 — overrides every printed current value
                    └────────────┬─────────────┘
                                 │ narrated by
   ┌─────────────────────────────▼──────────────────────────────┐
   │  session-log.md    <name>-story.md    npcs.md              │  TIER 7 — no mechanical weight
   └────────────────────────────────────────────────────────────┘
```

---
---

# 5. NAVIGATION — where to look, by question

| The question | Go to |
|---|---|
| "How does X work in general?" | **Book IV**, then Book 0's quick-ref to find the section fast |
| "What rank is this technique?" | **jutsu-compendium**, by rank file |
| "What can this character do?" | `<name>.md` for the index → `<name>-jutsu.md` for the numbers |
| "What does this transformation cost?" | `<name>-transformations.md` |
| "How much Chakra do they have *right now*?" | **`campaign/campaign-state.md`**. Only there. |
| "Does this character know about X?" | **`<name>-story.md` → Knowledge Ledger.** Never assume from another sheet. |
| "Who is this NPC?" | `campaign/npcs.md`, then Book III for canon figures |
| "What happened last session?" | `campaign/session-log.md` |
| "What are they actually trying to do?" | **`campaign/campaign-state.md` → THE MISSION**, then each `characters/<name>-story.md` Part Two. **Threads are what happens *to* them; goals are what they *want*. Do not summarise the campaign from the threads alone.** |
| "Can this NPC say this out loud?" | **Book III §4 — Information Horizons.** *What they may know.* |
| "Would a person say it *like that*?" | **`CUSTOM_INSTRUCTIONS.md` → DIALOGUE, PART ONE** + the **VOICE INDEX** at the top of `campaign/npcs.md`. *How they talk.* **These are different questions and both must be checked.** |
| "Two files disagree" | **Section 1 of this file.** Higher tier wins. Then fix the loser. |

---
---

# 6. HOW TO UPDATE STATE — the write rules

**During play, you will almost only ever write to `campaign/campaign-state.md`.** That is by design.

| When this happens | Write to | Do NOT touch |
|---|---|---|
| Resources spent, damage taken, Special gained | `campaign-state.md` | Character sheets |
| A condition, injury, or transformation starts/ends | `campaign-state.md` | Transformation files |
| Mastery XP gained on a technique | `campaign-state.md` (mastery table) | The jutsu file's ladder |
| A character **learns a new technique** | `<name>-jutsu.md` (full entry) **and** the sheet's index line | — |
| A character **unlocks a transformation tier** | `<name>-transformations.md` status field | — |
| A character levels or ranks up | `<name>.md` (recompute from Book IV formulas) **and** `campaign-state.md` | — |
| A character **learns a fact** | `<name>-story.md` Knowledge Ledger | Other characters' story files |
| A session ends | `campaign/session-log.md`, then each `<name>-story.md` | — |
| A **general rule** changes | `book-4-the-game.md`, then propagate to Book 0 + CUSTOM_INSTRUCTIONS | — |

### The knowledge rule — the one that is easiest to break

> **A character knows something only if their own `<name>-story.md` Knowledge Ledger says so.**

Do not grant knowledge because another PC's file records it, because an NPC knows it, because the session log narrates it from a third party's view, or because it is written down in this project at all. The Knowledge Ledger distinguishes **Confirmed** / **Believes (may be wrong)** / **Suspects** / **Does not know**, and the last category is load-bearing.

### Recomputing a character — the formulas (Book IV §1 Part Seven)

```
Chakra Max   = 100 + 20×(Level−1) + 10×CON mod   → then Body Origin → then clan multiplier
Stamina Max  = 100 + 20×(Level−1) + 10×CON mod   → then Body Origin
Health       = 30 + 10×(Level−1) + 2×CON mod×Level
Defense      = 10 + DEX mod
Save DC      = 8 + proficiency + governing attribute mod
Skill mod    = governing attribute mod + proficiency (if proficient)
```

Never hand-adjust a derived number. Change the input and recompute. Continuity patches that pin an old value are how the three-strata problem happened in the first place.

---
---

# 7. WHAT THIS AUDIT CHANGED

Full change record: **`AUDIT-REPORT.md`**.

Structural summary:

- **Rule hierarchy created.** It did not exist. Four files independently defined the same core mechanics.
- **Static/dynamic split enforced.** Live values consolidated into `campaign-state.md`.
- **Character sheets decomposed** from 700–1600-line monoliths into sheet + jutsu + transformations + story.
- **Contradictions resolved** across Book IV, Book II, and all three character sheets — each one traced through every file that referenced it.
- **Broken references repaired**, including the missing D-rank jutsu file and the `Naruto_PC_Sheet_*.md` / `File NN` paths.
- **Duplication removed** — NPC dossiers, clan mechanics, and combat rules each now have one home.
- **Nothing was deleted.** Everything moved. Where a fact existed in several conflicting versions, the resolved version is in the authoritative file and the superseded reading is preserved as a dated note.
