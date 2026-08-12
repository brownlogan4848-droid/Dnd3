# Shinobi Chronicles — Naruto Campaign

An unofficial Naruto tabletop campaign ("Shinobi Chronicles") with its own fully custom ruleset. This material is **not** the D&D 5e system implemented by the `/dm:dnd` plugin under `skills/dnd/` — it's a separate, self-contained game world and rules set, kept here for reference and as the live record of an in-progress campaign ("The Long Shadow").

## Why it's separate from `skills/dnd/`

The `/dm:dnd` plugin's scripts (`character.py`, `combat.py`, `lookup.py`, etc.) are built around standard D&D 5e mechanics and the bundled 5e SRD dataset. Shinobi Chronicles uses a different engine entirely:

- **Three resources** — Chakra, Stamina, and a fill-from-zero Special bar — instead of D&D spell slots/hit dice.
- **Combo-slot combat** — up to N actions per turn (by rank), each technique costing 1–4 slots, with Chain Momentum, Clashes, and a Counter Window system.
- **Rank progression** — Genin → Chūnin → Jōnin → S-Rank → Kage — instead of D&D character levels (though a level number tracks alongside rank for resource scaling).
- **Its own jutsu rank ladder** (E through S, plus unranked kekkei genkai/dōjutsu), sourced from the Naruto databooks rather than the D&D SRD.

Nothing here wires into the plugin's Python scripts or SRD data. It's Markdown reference material plus two player-character sheets, meant to be read directly (e.g. pasted into a Claude Project's custom instructions, or read by an AI GM) rather than executed by the plugin's tooling.

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
  ardo.md                       Chūnin — hidden Uzumaki, Body of Indra, Wind affinity
  suzume.md                     Chūnin — Mangekyō Sharingan (right eye)
  souji.md                      Chūnin — hidden Senju, Body of Ashura, Earth affinity

the-seam.md                   Ardo's Other Power Systems, split out of his sheet:
                                Hokorobi · Kōfū/Uzufū/Sakauzu · Sōgan + the Vision
                                economy and dōjutsu trees · Arakawa & Aragami ·
                                the Bequest · Shiokaze · Uzushio
squad-two-journey.md          Running log of Roku, Souji and Suzume while Ardo is
                                underground in Ryūchi Cave
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

Live campaign: ***The Long Shadow*** — Era A (Third Great Ninja War, ~Year −15), Konoha. **Session Eight has closed.** Planned to run through a timeskip and resume in Era C.

**Cell 409** is, un-asked-for and unannounced, the Indra/Ashura cycle running again: Ardo chose Body of Indra and turned out to be hidden Uzumaki; Souji chose Body of Ashura and turned out to be a lost branch-line Senju; Suzume is Uchiha in blood and Body Origin both. Nobody engineered that at character creation.

**Where everyone stands after Session Eight — "Training Ground Six":**

| | State |
|---|---|
| **Ardo** | Chūnin. Carries Suzume's Mangekyō in his left socket permanently — **it never deactivates**, and he is the only one paying a Vision cost for it. The entity behind his seal spent itself saving her and is **dormant**; it was doing his chakra control his entire life, so he now runs on 荒れ川 **Arakawa**, an unregulated river where transformations can cost him a limb. **Must learn senjutsu as treatment.** |
| **Suzume** | Chūnin. Took 99 damage against 80 Health shielding Souji and lived on a four-minute margin. **Mangekyō awakened as she died**; technique 迎え火 **Mukaebi** named but unbuilt. Left socket carries Ardo's ordinary eye — 相眼 **Sōgan**, a closed two-way circuit nobody in Konoha has seen before. Awake, critical, entirely herself. |
| **Souji** | Genin. Failed his own bloodline's three-save test by three points and 不倒樹 **Futōju** took him. Hiruzen put him down personally with Enma. **根の記憶 Ne no Kioku is permanent** — one real piece of bloodline knowledge per session from here on. Awake two days and has not spoken to anyone. |

**Standing GM rule:** *Mandatory Arc Beats* (Book IV §5, Part Eight) — 1–2 GM-initiated spotlight moments per PC per session, the GM's job to deliver rather than the player's to request.

**Session Eight closed with the whole cell leaving.** Cell 409 is designated **遊撃班 Yūgekihan** — a roving unit, independent, long-range, unattached to any front — by Hiruzen's own seal. All three said yes by choice, out loud, on the record. Roku goes with them as jōnin of record, explicitly *not* as their leash. Hiruzen's four conditions: real designation rather than wandering, irregular reporting, Roku, and — set independently by Souji four hours earlier, neither knowing the other said it — **ask Suzume properly, awake, with a real door to refuse through.**

**Why it's the road and not an escape:** senjutsu is not in Konoha. All three gates of the only actual treatment for Ardo's condition are outside the walls.

**Live threads:** the Uchiha taboo — Suzume's eye is in a non-Uchiha's head, unsanctioned, and Hiruzen calls that an *incident* rather than a scandal if it surfaces during the war · Danzō withdrew his classification request and made Roku deliver the news, which Hiruzen reads correctly as repositioning rather than retreat · 荒神 **Aragami**, the thing being *grown* in Ardo out of natural energy and an unguarded seal, not a tailed beast and with nobody inside it to negotiate with · the Handler and the Shepherd's judgment, pending from Session Seven · and the boy who walked out past the walls looking for answers and never came home, whose name Hiruzen would not say.

**Planned:** a timeskip, resuming in **Era C**.

See `characters/ardo.md`, `characters/suzume.md`, and `characters/souji.md` for full mechanics, session logs, and open threads.
