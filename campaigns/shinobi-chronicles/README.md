# Shinobi Chronicles — Naruto Campaign

An unofficial Naruto tabletop campaign ("Shinobi Chronicles") with its own fully custom ruleset. This material is **not** the D&D 5e system implemented by the `/dm:dnd` plugin under `skills/dnd/` — it's a separate, self-contained game world and rules set, kept here for reference and as the live record of an in-progress campaign (**"The Long Shadow"**).

> ## → Start with **`ARCHITECTURE.md`**.
> It carries the **authority ladder** (which file wins when two disagree), the **file map**, the **static/dynamic split**, and the **write rules** for updating game state. Reading it first will save you reverse-engineering the structure.

## Why it's separate from `skills/dnd/`

The `/dm:dnd` plugin's scripts (`character.py`, `combat.py`, `lookup.py`, etc.) are built around standard D&D 5e mechanics and the bundled 5e SRD dataset. Shinobi Chronicles uses a different engine entirely:

- **Three resources** — Chakra, Stamina, and a fill-from-zero Special bar — instead of D&D spell slots/hit dice.
- **Combo-slot combat** — up to N actions per turn (by rank), each technique costing 1–4 slots, with Chain Momentum, Clashes, and a Counter Window system.
- **Rank progression** — Genin → Chūnin → Jōnin → S-Rank → Kage — instead of D&D character levels (though a level number tracks alongside rank for resource scaling).
- **Its own jutsu rank ladder** (E through S, plus unranked kekkei genkai/dōjutsu), sourced from the Naruto databooks rather than the D&D SRD.

Nothing here wires into the plugin's Python scripts or SRD data. It's Markdown reference material meant to be read directly — pasted into a Claude Project's custom instructions, or read by an AI GM — rather than executed by the plugin's tooling.

## Layout

```
ARCHITECTURE.md               ★ READ FIRST. Authority ladder, file map, write rules
AUDIT-REPORT.md               What the architecture audit changed, and why
CUSTOM_INSTRUCTIONS.md        GM system prompt (two versions: full + compact)

compendium/                   STATIC — the setting bible and the rules
  book-0-index.md               Quick-reference tables. DERIVED, non-authoritative
  book-1-world.md               §1 Timeline · §2 Geography · §3 Politics · §4 Shinobi System
  book-2-power-bloodline.md     §1 Chakra · §2 Clans · §3 Tailed Beasts · §4 Summons & Gear
  book-3-people-secrets.md      §1 Era A cast · §2 Era C cast · §3 Orgs · §4 Information Horizons
  book-4-the-game.md            ★ TIER 1 RULES AUTHORITY

jutsu-compendium/             STATIC — every canonical technique, by rank
  01-e-rank.md … 07-outside-the-ranks.md
  expansions/                   Databook-verified additions · E/D gap-fill surveys

characters/                   Four files per PC, one job each
  ardo.md                       SHEET — identity, stats, capability index
  ardo-jutsu.md                 ★ his techniques
  ardo-transformations.md       ★ his forms, dōjutsu, Vision economy, Arakawa
  ardo-inheritance.md           the Seam, the estate, the Whirlpool Archive
  ardo-story.md                 goals · KNOWLEDGE LEDGER · relationships · threads
  suzume.md / -jutsu / -transformations / -story
  souji.md  / -jutsu / -transformations / -story
  _TEMPLATE-*.md                Standard templates for adding a character

campaign/                     DYNAMIC + shared narrative
  campaign-state.md             ★ THE ONLY PLACE LIVE VALUES LIVE
  session-log.md                Canonical shared session spine
  npcs.md                       NPC roster, deduplicated
  archive/
    squad-two-journey.md        CLOSED. Historical, superseded

the-seam.md                   Redirect stub — contents moved into characters/
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
| **[DECISION NEEDED]** | A genuine ambiguity requiring a human ruling. Never silently resolved. |

## Campaign status

> **Live status, party state, and current resources: `campaign/campaign-state.md`.**
> That file is the single source of truth and this section deliberately does not duplicate it.

**Where the campaign stands:** ***The Long Shadow*** — **Year 0, October 10th.** The Third Great Ninja War is over; the war that mattered lasted one night. **Konoha is burning.** The Nine-Tails is sealed, Minato and Kushina are dead, Souji has defected, and the campaign is at the end of Act One with the Era C timeskip ahead.

**遊撃班 Yūgekihan** — an independent long-range unit, unattached to any front, sent where Konoha officially is not. **It is now two people.**

They were, un-asked-for, the Indra/Ashura cycle running again: Ardo took Body of Indra and is Uzumaki; Souji took Body of Ashura and is a lost branch-line Senju; Suzume is Uchiha in blood and Body Origin both. **Nobody engineered that at character creation, and on October 10th it started running the way it historically runs.**

**Standing GM rule:** *Mandatory Arc Beats* (Book IV §5, Part Eight) — 1–2 GM-initiated spotlight moments per PC per session, **the GM's job rather than the player's to request.**
