# Shinobi Chronicles — Naruto Campaign

An unofficial Naruto tabletop campaign ("Shinobi Chronicles") with its own fully custom ruleset. This material is **not** the D&D 5e system implemented by the `/dm:dnd` plugin under `skills/dnd/` — it's a separate, self-contained game world and rules set, kept here for reference and as the live record of an in-progress campaign ("The Long Shadow").

## Why it's separate from `skills/dnd/`

The `/dm:dnd` plugin's scripts (`character.py`, `combat.py`, `lookup.py`, etc.) are built around standard D&D 5e mechanics and the bundled 5e SRD dataset. Shinobi Chronicles uses a different engine entirely:

- **Three resources** — Chakra, Stamina, and a fill-from-zero Special bar — instead of D&D spell slots/hit dice.
- **Combo-slot combat** — up to N actions per turn (by rank), each technique costing 1–4 slots, with Chain Momentum, Clashes, and a Counter Window system.
- **Rank progression** — Genin → Chūnin → Jōnin → S-Rank → Kage — instead of D&D character levels (though a level number tracks alongside rank for resource scaling).
- **Its own jutsu rank ladder** (E through S, plus unranked kekkei genkai/dōjutsu), sourced from the Naruto databooks rather than the D&D SRD.

Nothing here wires into the plugin's Python scripts or SRD data. It's Markdown reference material plus three player-character sheets, meant to be read directly (e.g. pasted into a Claude Project's custom instructions, or read by an AI GM) rather than executed by the plugin's tooling.

## Layout

```
CUSTOM_INSTRUCTIONS.md        GM system prompt (two versions: full + compact)

compendium/                   The Naruto Compendium — setting bible, four books
  book-0-index.md               Index, quick-reference tables, sourcing legend
  book-1-world.md               §1 Timeline & Eras · §2 Geography · §3 Politics · §4 Shinobi System
  book-2-power-bloodline.md     §1 Chakra & Power · §2 Clans & Bloodlines · §3 Tailed Beasts · §4 Summons/Bestiary/Equipment
  book-3-people-secrets.md      §1 Third War Characters · §2 Fourth War Characters · §3 Organizations · §4 Information Horizons
  book-4-the-game.md            §1 The System · §2 Advanced Combat · §3 Jutsu Mastery & Creation · §4 NPC/Threat Design · §5 GM Toolkit

jutsu-compendium/             Every canonical technique, organized by rank
  01-e-rank.md ... 07-outside-the-ranks.md
  expansions/
    databook-verified-rank-additions.md   Databook-sourced additions/corrections
    e-d-gapfill-noncanonical.md           E/D gap-fill + non-canonical rank surveys

characters/                   Player characters, campaign "The Long Shadow"
  ardo.md                       Jōnin 13 — Uzumaki (known), sage, carries the archive
  suzume.md                     Jōnin 13 — Mangekyō (right eye), war medic, genjutsu
  souji.md                      Jōnin 13 — Senju (known), Body of Ashura, Earth

the-seam.md                   Ardo's Other Power Systems, split out of his sheet:
                                Hokorobi · the reconstructions (Kōfū/Uzufū/Sakauzu) ·
                                Sōgan + the Vision economy and dōjutsu trees ·
                                Arakawa · Aragami (closed) · the Bequest · Kikkō ·
                                Shioai · Shiokaze · the Archive · Daisen · Uzushio
squad-two-journey.md          CLOSED. Roku, Souji and Suzume's six-month search for
                                Ardo, and the reunion. Party whole since Year −13
```

## Sourcing conventions used throughout

| Tag | Meaning |
|---|---|
| **[SHEET]** | Printed on an official sheet or directly derived from it. Authoritative. |
| **[M]** / **[DB]** | Manga canon / Japanese databook. |
| **[A]** / **[MV]** / **[N]** | Anime-only / movie-only / novel-supplementary. |
| **[INF]** | Reasonable extrapolation, not directly stated. |
| **[GM]** | Table ruling — homebrew, not canon. |
| **[CONFLICT]** | Sources disagree; both readings preserved, not resolved. |

## Campaign status

Live campaign: ***The Long Shadow*** — **Era A, ~Year −5. The Third Great Ninja War is ending.** An eight-year timeskip has run; the campaign stays here through the war's end before skipping to **Era C**.

**Cell 409 / 遊撃班 Yūgekihan** — an independent long-range unit, unattached to any front, sent where Konoha officially is not. Eight years of that. **Ardo 18 · Souji 20 · Suzume 22. All three Jōnin, Level 13.**

They are, un-asked-for, the Indra/Ashura cycle running again: Ardo took Body of Indra and is hidden Uzumaki; Souji took Body of Ashura and is a lost branch-line Senju; Suzume is Uchiha in blood and Body Origin both. Nobody engineered that at character creation.

### Where everyone stands

| | State |
|---|---|
| **Ardo Uzumaki** | **Sage of no species**, taught anyway by the White Snake Sage. Carries 渦の書庫 — the complete archive of a destroyed clan, thousands of preserved Uzumaki — plus Suzume's Mangekyō and his mother Hikari's own form. **大仙 Daisen** is past S-rank and **cannot hide**, which collides directly with the advice that taught him to. An unnamed Kumo bingo-book entry exists: *wind, sage-class, do not engage alone* |
| **Souji** | Senju in truth, and the tree is complete: **不倒樹** the failure state, **倒木** the sword, **貫根** the root aimed outward, **朽木** which drains an enemy's life and cannot keep a drop of it. **息吹 Ibuki** — his vitality given away, never to himself. Every technique he owns points at somebody else |
| **Suzume** | War medic. **無戸の間** — the doorless room, built out of her own worst three days, breakable only by someone reaching in from outside. **断脈** cuts what's under the skin and leaves no wound. **迎え火 Mukaebi** is the same room with the lamp still in it |
| **Roku** | Off the front for good since Year −6. Suzume kept him alive six days in a cave. He fought the desk and lost |

### The war, and the world

Minato Namikaze — Ardo's *sensei of record*, and weather his entire life — ended the war almost single-handed and is **Fourth Hokage.** Ardo got **six days with him in eighteen years.**

**Kakashi Hatake** took a Sharingan into a non-Uchiha skull at Kannabi Bridge and wears his headband over it. **Neither he nor Ardo knows about the other** — two men in one village doing identical daily arithmetic.

**Orochimaru** was a hero of Konoha for most of the eight years, and near the end was quietly somewhere he should not have been. It made a file, not a headline.

**Danzō** never moved. Twice Root was found adjacent to Cell 409 and withdrew politely. **He is waiting**, exactly as Hiruzen said he would.

### Live threads

- **The Uchiha still do not know** Suzume's eye left the clan. Eight years held, mostly by absence.
- **Four living Uzumaki found. Three were dead ends. One was not** — and Ardo will discuss it with nobody but the archive.
- **The stand of trees remains unvisited.** Twice they got within a week; twice the war moved. Nine members of the archive placed it in the same region, none would say what's there, and **two went quiet in a way Nao refuses to explain.**
- **Ardo is the last library of a destroyed people**, and the nations that erased them have not changed their minds.
- **Three names nobody will say:** the man who signed the snake scroll ninety years ago · the boy who walked out of Konoha and never came home · the syllable Hikari started and did not finish.

**Standing GM rule:** *Mandatory Arc Beats* (Book IV §5, Part Eight) — 1–2 GM-initiated spotlight moments per PC per session, the GM's job rather than the player's to request.

See `characters/`, `the-seam.md`, and `squad-two-journey.md` (closed).
