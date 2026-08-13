# ARCHITECTURE AUDIT — FULL REPORT

**What was inspected, what was found, what changed, and what remains unresolved.**

Structure and navigation: **`ARCHITECTURE.md`**. This file is the change record.

---
---

# 1. SCOPE

**Everything under `campaigns/shinobi-chronicles/` — ~870 KB across 20 files.** Every file was read, not sampled.

The `skills/dnd/` plugin, `dice-server/`, `tests/` and `design-mockups/` were **not touched.** They are a different system (D&D 5e + SRD) with no coupling to this campaign, as the README already documented.

---
---

# 2. THE HEADLINE FINDINGS

| # | Finding | Severity |
|---:|---|---|
| **1** | **No rule hierarchy existed.** Four files independently defined the same core mechanics with no statement of which wins | **Critical** |
| **2** | **No static/dynamic separation.** Live values were duplicated 3–5 times per character, drifting apart | **Critical** |
| **3** | **Suzume's sheet carried three unreconciled strata** — Level 1, Level 5 and Level 13 text all live at once, contradicting each other on nine separate facts | **Critical** |
| **4** | **Six genuine mechanical contradictions** in the rules layer, including two inside a single file | **High** |
| **5** | **`02-d-rank.md` was referenced by two files and did not exist** — and D-rank is where all three PCs actually operate | **High** |
| **6** | **Character sheets were 700–1600-line monoliths** carrying eight unrelated responsibilities each | **High** |
| **7** | **Save DCs were frozen at Level 1 values** across all three characters — every technique in the game was rolling against the wrong number | **High** |
| **8** | **Four techniques violated Book IV's own cost bands**, one by more than half | **Medium** |
| **9** | **Three named techniques had no mechanics at all** after years of play | **Medium** |
| **10** | **NPC dossiers were duplicated across two or three character sheets** and had drifted | **Medium** |
| **11** | **The most recent session was unrecorded anywhere** — including a PC becoming a jinchūriki and another PC defecting | **Medium** |
| **12** | **Broken path references** — `Naruto_PC_Sheet_*.md`, `File 07/13/17` | **Low** |

---
---

# 3. RULE CONTRADICTIONS — RESOLVED

Each was traced through **every** file that referenced it, not just the one where it was found.

## 3.1 Pushing through an interruption

| Source | Said |
|---|---|
| Book IV §1 Part Six · §2 Part Five · Book 0 · `ardo.md` | **30 Special, or a feature. "There is no free save."** |
| Book IV §2 Part Twelve — the printed quick-reference card | *"CON save, or 25 Stamina (1/combo)"* |

**RESOLVED: 30 Special or a feature.** Three sources against one, and the body text explicitly forbids a free save — **which a CON save is.** The card was stale and is corrected.
**Propagated to:** Book IV §2 card · Book 0 · CUSTOM_INSTRUCTIONS · all three sheets.

## 3.2 The Special spend menu — two menus, one price collision

Book IV §1 listed *"add +1 damage die = 20 Special."* Book IV §2 listed *"Heavy Strike, +2 damage dice = 20 Special."* **Same price, different product**, with no statement they were alternatives. Book 0 had propagated §2's version and silently dropped two §1-only entries.

**RESOLVED: §2 wins** — it is the combat-authoritative section and already had downstream propagation. **The two menus are merged into one master table at Book IV §1 Part One**, which now explicitly says it is the only spend menu in the system. §2 Part Four is labelled as the combat subset. The §1-only entries (*ignore a cost*, *auto-succeed a save*) are preserved and priced against their neighbours.

## 3.3 Jinchūriki — where DM control begins

| Source | Said |
|---|---|
| Book IV §1 Part Seven | *"Three or more tails… the DM takes the character"* |
| Book II §3 Part Five | **3 tails: still the player's** (3d10, save DC rises to 17). **4+: DM control** |

**RESOLVED: Book II wins.** It is the specific, complete treatment, and the three-tail stage exists so a player *feels the slide* for a round before losing the wheel — deleting it removes the best beat the subsystem has. **Book IV now delegates in full and states no thresholds of its own.**

**This was not academic.** A PC became a jinchūriki in the most recent session. Book II §3 Part Five is now marked authoritative, and an **adult-sealing clause** was added — the existing text assumed infant hosts, and this host is 23.

## 3.4 The Senju clan passive referenced a subsystem that does not exist

Book IV's Legendary Clans table read: *"Recover extra HP whenever spending **Hit Dice** during a rest."* **This system has no Hit Dice.** It runs Chakra/Stamina/Health with percentage recovery.

Meanwhile `souji.md` carried **Mastery of the Earth**, a working Senju passive established in play, which the sheet itself flagged as needing reconciliation.

**RESOLVED:** the printed clan trait is restated in this system's terms (**+25% max Health on a long rest**) and **unified with Mastery of the Earth**. Souji's sheet is no longer an unacknowledged override — it now matches the printed trait.

## 3.5 D-rank Stamina band printed two ways

Book IV §1 said the band was extrapolated from *"D: 8–12 / **5–6**"* while every table in the same file said **5–8**.

**RESOLVED: 5–8.** No printed D-rank technique respects 5–6 — Body Flicker is 8/6 and Gale Fist is 10/6.

## 3.6 The duplicated Reactions block

`CUSTOM_INSTRUCTIONS.md` carried the *"Reactions are usable at any moment"* rule **twice**, in two different wordings, one of which still said a lost-reach Displace **ends the combo** — contradicting the house rule adopted in Session Six (*the attacker gets one reroll*).

**RESOLVED:** merged into one block carrying the current house rule.

---
---

# 4. CHARACTER-LEVEL CONTRADICTIONS — RESOLVED

## 4.1 Suzume — the three strata

Her sheet had never been reconciled after two rank-ups. **Nine contradictions, all live simultaneously:**

| Fact | Contradictory values found | Resolved to |
|---|---|---|
| **Age** | 27 · 22 · "AGE 12" | **27** |
| **Max jutsu rank** | "C-rank ceiling" · "Maximum Jutsu Rank: D" · Book IV's "B + one A" | **B + one A-rank signature** *(she already owned both)* |
| **Sharingan stage** | "2 Tomoe" ×3 · "Mangekyō" ×2 | **Mangekyō, right eye** |
| **Mangekyō status** | "AWAKENED" · "Locked, Level 14" | **Awakened** |
| **Medical** | +7 · +4 · +5 · *"no Medical Ninjutsu, cannot announce a healing jutsu"* | **+7, full medical ninjutsu** |
| **Genjutsu** | +8 "her actual specialty" · "Untrained, no proficiency" · +0 | **+8** |
| **Dōjutsu tiers** | "none unlocked" · "two unlocked" | **I–II unlocked** |
| **Sōgan tiers** | unstated · "two unlocked" | **I–III unlocked** |
| **Health** | 176 · a "continuity ruling" pinning **35** | **176.** The pin is void |
| **迎え火 Mukaebi** | "named, unbuilt, mechanics to be built" · "BUILT" over nine months | **Built** |

**In each case the resolution followed the file's own later evidence** — the Ryūchi Cave and timeskip logs sitting further down the same document.

## 4.2 Save DCs frozen at Level 1 — all three characters

Every technique with a save was rolling against a stale number:

| Character | Was | Now |
|---|---|---|
| **Ardo** | DC 12, DC 13 | **DC 15** — affects Storming Thunder God, Barometric Tsunami, Storm-God's Iron Grip, Splendor |
| **Souji** | Root Grip *"DC (10)"* | **DC 15** |
| **Ardo / Souji / Suzume** | Attack bonuses +4 / +5 | **+7** — Level-1 values on Level-13 characters |
| **Suzume** | Taijutsu damage **1d6 − 1** | **1d6** — the −1 assumed STR −1; her STR is 10 (+0) |

## 4.3 Ardo — Vision loss rate off by a factor of thirty

`ardo.md`'s appendix: **"−1 VISION PER DAY no matter what."**
`the-seam.md`'s detailed treatment: **−1 per month uncovered, 0 while covered.**

**RESOLVED: −1 per month.** The detailed treatment is authoritative and had been *deliberately rescaled* to a decades-long clock in an earlier revision (commit `339d221`). The appendix was never updated.

**This one mattered enormously** — at the appendix rate Ardo would have gone blind years ago.

## 4.4 Ardo — a deleted table still live in the appendix

The appendix carried Arakawa's **10–14 EMERGENT** result (荒神 Aragami forms, three saves, fail two and it takes him) that `the-seam.md` had **explicitly deleted and declared void.**

**RESOLVED:** 10–14 is **SLIP**. The three saves (CON 15 / WIS 17 / CON 19) **must not be rolled.**

## 4.5 Ardo — stale rank gates from two promotions ago

| Was | Now |
|---|---|
| Storm-God's Iron Grip: *"requires Kōfū — B sits above the Chūnin max rank of C"* | **Gate removed.** He is Jōnin; B is his native ceiling |
| Kōfū override: *"overrides his normal Chūnin ceiling"* | **Overrides his Jōnin ceiling** |
| Kōfū activation: *"2 of his 4 slots at Chūnin"* | **2 of his 5 (Jōnin)** |
| Splendor: *"full Genin combo"* | **3 of his 5 slots** |
| Appendix header: *"ARDO · Chūnin · Level 5"* directly above *"age 23 · JŌNIN"* | **Jōnin, Level 13** |
| 潮風 Shiokaze: *"OWNED, NOT YET ENTERED"* | **Owned and entered** — contradicted by Daisen, which prefixes it as 大仙・潮風 and cannot exist without it |

---
---

# 5. COST-BAND VIOLATIONS — CORRECTED

Four techniques violated Book IV's own rank/cost bands. **None declared an override or gave a reason**, so under the new hierarchy they are errors rather than deliberate exceptions.

| Technique | Violation | Fix | Method |
|---|---|---|---|
| **Barometric Tsunami** | C-rank at 12 Ch / 6 St / **1 slot** — below the C band on all three axes (15–25 / 8–14 / **2 slots**) | **Reranked to D** | Its output (2d8, one target, linear) genuinely reads D. **Least invasive** |
| **Storm-God's Iron Grip** | B-rank at **14 Ch / 10 St** — under half the B floor (30–45 / 15–22) | **Repriced to 30 / 15** | Its effect (3d10 + aerial control + stun + Reaction-castable) genuinely is B |
| **Thunder Gods Gale** | C-rank at **28 Ch** — above the C ceiling of 25 | **Repriced to 25 / 14** | |
| **Storming Thunder God** | C-rank at **15 St** — above the C ceiling of 14 | **Repriced to 25 / 14** | |
| **Nerve Lock** *(Suzume)* | C-rank at **14 Ch**, slot cost never recorded | **15 Ch / 9 St, 2 slots** | |

> **Each correction records the alternative.** Barometric Tsunami could equally be repriced up rather than reranked down; Storm-God's Iron Grip could be reranked to C rather than repriced up. **The choices made preserve each technique's *feel* at the cost of its label.** Both are defensible and the table can flip either.

---
---

# 6. TECHNIQUES THAT HAD NO MECHANICS

Three named techniques had been in play for years with **no costs, no slots, and in one case no numbers of any kind.**

| Technique | Had | Given |
|---|---|---|
| **貫根 Kankon** *(Souji, B-rank)* | Nothing | **35 Ch / 18 St, 2 slots** — middle of the B band |
| **朽木 Kuchiki** *(Souji, A-rank signature)* | Nothing | **55 Ch / 28 St, 3 slots** — middle of the A band |
| **断脈 Danmyaku** *(Suzume, B-rank)* | Nothing | **35 Ch / 18 St, 2 slots** |
| **息吹 Ibuki** *(Souji)* | *"his Stamina and Health at a bad exchange rate"* | **2 Stamina + 1 Health per 1 Health delivered** |
| **無戸の間 Muto no Ma** *(Suzume, A-rank signature)* | *"Cost: Special, and the memory"* | **40 Special, 3 slots, Genjutsu DC 16** |
| **倒木 Tōboku** *(Souji)* | *"—/10"*, no rank | **Unranked, 10 Stamina, 1 slot** |

**Design intent was preserved in every case.** *"There is no way to make it efficient because it is not supposed to be"* is a design statement, not a number — so a number was supplied that *implements* it rather than replacing it.

---
---

# 7. STRUCTURAL CHANGES

## 7.1 The authority ladder — created

Seven tiers, in `ARCHITECTURE.md` §1. **Book IV is Tier 1.** Book 0 and CUSTOM_INSTRUCTIONS are explicitly marked **derived and non-authoritative** — both now carry that warning at the top.

**A character file may override Book IV only when it is tagged [GM], names the rule it overrides, and is scoped to that character.** Everything else in a character file that contradicts Book IV is stale, not an override.

## 7.2 The static/dynamic split — enforced

**`campaign/campaign-state.md` created** as the single home for every live value. Character sheets now carry **maxima and formulas only.** Verified: **zero current-value leakage** remains in any character file.

## 7.3 Character sheets decomposed

| Character | Before | After |
|---|---|---|
| **Ardo** | `ardo.md` 1,210 lines + `the-seam.md` 900 lines | `ardo.md` **273** · `-jutsu` 423 · `-transformations` 582 · `-inheritance` 333 · `-story` 231 |
| **Suzume** | `suzume.md` **1,593 lines** | `suzume.md` **248** · `-jutsu` 213 · `-transformations` 239 · `-story` 177 |
| **Souji** | `souji.md` 723 lines | `souji.md` **248** · `-jutsu` 247 · `-transformations` 192 · `-story` 188 |

**Nothing was deleted.** Every fact moved to the file that owns it.

`the-seam.md` — a character-owned file sitting at the campaign root, named for a diagnosis the campaign has since proven wrong — became a **redirect stub** listing where each of its sections went.

## 7.4 Shared files created

- **`campaign/npcs.md`** — NPC dossiers deduplicated from two or three character sheets each. Campaign-original NPCs only; canonical figures stay in Book III.
- **`campaign/session-log.md`** — the canonical spine, Sessions 1–12, **including the previously unrecorded Session Twelve.**
- **`campaign/archive/squad-two-journey.md`** — moved; it was a closed log sitting at the root.
- **Four templates** in `characters/`, with format rules encoding the lessons of this audit.

## 7.5 The missing D-rank file

**`jutsu-compendium/02-d-rank.md` created.** It was referenced by `book-0-index.md` and by Book IV §1 — which even named three techniques as living in it — and did not exist, while **all three PCs operate primarily at D-rank.**

It also resolves a tracked gap: **Genjutsu Release (Kai)** appeared in no rank file, leaving the setting's most important defensive technique homeless. **Ruled to D-rank** as a placement decision, flagged as overturnable.

And it flags one thing Book IV got half-wrong: **Decapitating Airwaves** is named as a D-rank alternative and is widely assumed to be Wind Release — which would break Ardo's core constraint that *no Wind Release exists below C-rank.* **The databooks rank it D and list no nature**, so it is recorded as shape manipulation of ordinary air, preserving both facts.

---
---

# 8. THE UNRECORDED SESSION

**Session Twelve — Year 0, October 10th — existed nowhere in the project**, despite containing:

- A PC **becoming the Nine-Tails jinchūriki** by transferring a seal off a newborn.
- The **death of the Fourth Hokage and Kushina Uzumaki.**
- A PC **defecting and attempting to kill two others.**
- The party dropping from **three members to two.**

**Now recorded** in `session-log.md`, all three story trackers, `campaign-state.md`, and `npcs.md`. **This is also what made the jinchūriki contradiction (§3.3) urgent rather than theoretical.**

---
---

# 9. DECISION POINTS

## 9a. RESOLVED BY TABLE RULING — Year 0

**Five of the eleven were ruled on and are now applied throughout the project.**

### ① Ardo's Max Vision → **65 / 100**

The ledger reconciles the ruling with the canonical 87 rather than overwriting it:

| | | Running |
|---|---:|---:|
| Start | | **100** |
| Recorded Mangekyō-grade uses *(Mukaebi 3 · Ryūchi day one 4 · the stone 6)* | −13 | **87** ← *canon, unchanged* |
| 相眼 Sōgan **II** and **III**, unlocked in the Ryūchi year | −10 | **77** |
| Thirteen years of the Kakashi discipline | −12 | **65** |

**−12 across 156 months at −1/month uncovered ≈ 92% discipline.** Exactly the trade the arc was always about.
**Consequence: Burning Clarity band 69–40 is now ACTIVE** — +1 to all Perception and Reaction timing, and colour going wrong on that side. **He is 26 points from the band where the eye starts paying him to kill it faster.**
**Applied in:** `campaign-state.md` · `ardo-transformations.md` · `ardo.md`.

### ② Ardo's own dōjutsu tree → **all four tiers unlocked at the transplant, at no Vision cost**

**He did not climb the tree; it arrived complete, in the socket.** *"See what I see"* was a build order, not an aspiration.

**Why it costs nothing:** the −5-per-tier charge prices a shinobi *forcing* a dōjutsu to grow. **Nothing here was forced** — it was given, at once, by someone dying who knew exactly what she was giving. **The cost was paid by her, in a different currency, and the ledger has no column for it.**

**Consequence:** Mikiri, Inyomi, Hanshun and Utsushi have been **passive and always running since Session Eight**, per the eye-never-deactivates rule. He has never switched them on and cannot switch them off. **This also resolves ① cleanly** — the tree's unlock predates the canonical 87, so its cost is already inside it.

### ③ 飛雷神・瞬 Hiraishin no Shun → **requires the eye uncovered. Priced.**

| | |
|---|---|
| **Per mark** | **Nothing.** Marking is a look — Sharingan-grade perception, same class as his own tier tree |
| **Per combat he marks in** | **−1 Max Vision.** Once or thirty times, same cost |
| **Waiting with it uncovered** | **−1 per month.** *The expensive one* |

> **The technique is free. The posture is not.** It does not charge him for using it — **it charges him for being ready to use it.** Minato solved that problem with years of pre-placed marks; Ardo replaced the planning with an eye, and the eye is the price.
>
> **And the 92% discipline that produced 65 was built over thirteen years in which he had no reason to break it.** He learned Shun hours before October 10th. **None of that history predicts how he handles it now.**

### ④ Who holds Souji → **DELIBERATELY UNRESOLVED. A standing mystery, not a gap.**

**The party believes Danzō. That belief is reasonable, load-bearing, and may be wrong.** Four readings are live and all textually supported: Danzō straightforwardly · **Orochimaru with Danzō as cover** · someone else with both names as noise · or **nobody, and he is attributing a choice he made alone.**

**Handling rules recorded in `campaign-state.md`:** never confirm or deny on the party's behalf · let them chase Danzō and let the trail be *nearly* right · Book III §4 limits every NPC's answer, **and nobody in Konoha has the whole picture, including Hiruzen** · the Ishinuma contract is the honest route, and Gensai refusing to answer is itself information · **when it resolves, it should cost something to learn.**

**Applied as a BELIEF, not a fact, in both PCs' Knowledge Ledgers** — Suzume's flagged specifically, since she is the one who asked about Orochimaru twice and got *"he's a colleague"* both times.

### ⑤ SOUTA → **thirteen years written. Held offstage.**

Waited two years without spending the money · took the **wartime Academy intake** and graduated late and barely, because his chakra is unremarkable and always was · spent the war as a **quartermaster** — convoy routing, transit papers, refugee registries, casualty reconciliation, **moving people and goods across borders that were not supposed to be crossed** · mustered out at Year −5 · has spent **the last eighteen months looking for his sister on paper**, which is the one thing the war made him very good at.

**Alive, ~25, and not in Konoha on October 10th.** His sister's fate stays unresolved.

> **He is the ordinary person** — no bloodline, no dōjutsu, no bijū, no estate — **and the only such person either PC ever personally saved and then simply left.**
>
> **He is also precisely what they now need and cannot get:** they are chasing a defector across a continent **with no headband authority by Hiruzen's own terms**, and Souta moves people across hostile borders on paper, professionally, and has for a decade.
>
> **⚠ Held offstage by ruling.** Not to contact Ardo or Suzume yet. *Ardo has not thought about him in years, and Souta has thought about Ardo constantly, and neither of those is a betrayal.*

## 9b. STILL OPEN — no ruling yet

| # | Question | Where | Why it stays open |
|---:|---|---|---|
| **6** | **Has 朽木 Kuchiki been taught to keep what it takes?** Flagged on three sheets for years as *"a moral architecture, not a law of physics"* | `souji-transformations.md` | The character's live arc. A scene, not a ruling |
| **7** | **Does the Ishinuma contract still answer Souji?** Gensai's house signed a sentence he may no longer believe | `souji-jutsu.md` | Also the party's most plausible route to finding him — **and now the honest route to ④** |
| **8** | **Sky-Torrent Downfall's rank.** Reads A-rank+ by output; the invention gates are nowhere near met | `ardo-jutsu.md` | The source already flagged this as an open campaign question. **Preserved, not overwritten** |
| **9** | **Ryō, all three characters.** 12,000 / 12,000 / 6,000 — **unchanged for thirteen years**, Souji's still annotated *"Genin-standard, no windfalls yet"* | `campaign-state.md` | Bookkeeping the table abandoned; not the audit's to fabricate |
| **10** | **The Shepherd's judgment and the Handler's interrogation.** *"Pending"* since Session Seven — **thirteen in-world years** | `npcs.md` | Genuinely open plot, now visible rather than buried |
| **11** | **Where Roku is.** Off the front since Year −6, in Konoha, which has just burned | `npcs.md` | Unaddressed by the source material |

**Pre-existing `[CONFLICT]` tags were left alone.** Lightning Blade vs Lightning Cutter, Fireball vs Phoenix Sage Fire, Hōzuki Hydrification, and every canon-source disagreement in Book 0 remain **deliberately unresolved**, as the project intends. Book 0's conflict log is now split into *canon conflicts* (preserved), *session-zero decisions* (open), and *mechanical contradictions* (resolved).

---
---

# 10. VALIDATION PERFORMED

| Check | Result |
|---|---|
| **All derived statistics recompute from Book IV formulas** | ✅ **9/9 pass** — every Chakra, Stamina and Health maximum for all three characters |
| **All save DCs = 8 + prof + attribute** | ✅ **12/12 pass** |
| **Broken internal file references** | ✅ **None** |
| **Current values leaking into character sheets** | ✅ **None** |
| **NPC dossiers duplicated across character files** | ✅ **None** — narrative mentions remain, which is correct |
| **Core mechanics redefined outside Book IV** | ✅ **None** — character files now point rather than restate |
| **`Naruto_PC_Sheet_*.md` / `File NN` references** | ✅ **Removed** |
| **Every character has sheet + jutsu + transformations + story** | ✅ **3/3** |
| **Every technique on a sheet has a full entry in a jutsu file** | ✅ |
| **Every named transformation has a status field** | ✅ |

---
---

# 11. WHAT WAS DELIBERATELY NOT CHANGED

- **Established canon.** No character fact, story event, relationship, or plot thread was altered. Where a fact existed in several conflicting versions, the resolved version is in the authoritative file and **the superseded reading is preserved as a dated note** — the project's own convention.
- **Voice.** The source material is written with a strong and deliberate register. Restructured files keep it.
- **Intentional design.** Suzume's Lightning cap at C-rank, the Grief/Rage Distinction, Ardo's Wind problem, Souji's Clanless restriction, the *"NPCs do not follow player rules"* asymmetry, and the *"do not let him learn the word 渦潮"* constraint were all identified as **deliberate and load-bearing**, and preserved exactly.
- **Canon `[CONFLICT]` tags.** Source disagreements are a feature.
- **The `skills/dnd/` plugin.** Out of scope and uncoupled.
