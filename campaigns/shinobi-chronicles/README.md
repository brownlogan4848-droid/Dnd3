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

Live campaign: ***The Long Shadow*** — Era A (Third Great Ninja War, ~Year −15). **Session Nine in progress, and the party is split.** Planned to run through a timeskip and resume in Era C.

**Cell 409** is, un-asked-for and unannounced, the Indra/Ashura cycle running again: Ardo chose Body of Indra and turned out to be hidden Uzumaki; Souji chose Body of Ashura and turned out to be a lost branch-line Senju; Suzume is Uchiha in blood and Body Origin both. Nobody engineered that at character creation.

### The split

Session Eight ended with the whole cell leaving Konoha as **遊撃班 Yūgekihan** — a roving unit, by Hiruzen's own seal, all three by choice. One day out, all three attempted uncontracted summoning. Souji and Suzume signed contracts. **Ardo rolled a reverse summon and was taken to 龍地洞 Ryūchi Cave**, on another landmass, alone.

| | Where they are |
|---|---|
| **Ardo** | **Underground with the snake sages**, learning senjutsu as *treatment* rather than as power. See `the-seam.md` |
| **Roku, Souji, Suzume** | **Walking northeast**, three to four months on foot past the Land of Frost, navigating by Suzume's half of a paired eye. See `squad-two-journey.md` |

### Where everyone stands

| | State |
|---|---|
| **Ardo** | Chūnin, 8. Carries Suzume's Mangekyō permanently — **it never deactivates**, and he is the only one paying a Vision cost. Runs on 荒れ川 **Arakawa**, an unregulated river, because the entity that was quietly doing his chakra control for eight years spent itself saving her. Natural energy has been entering him unguarded for six weeks and the endpoint is **stone**. Contracted to no one; Ryūchi Cave teaches him anyway, because he is interesting |
| **Suzume** | Chūnin, 12. Took 99 damage against 80 Health shielding Souji and lived on a four-minute margin. **Mangekyō awakened as she died**; 迎え火 **Mukaebi** named but unbuilt. Signed with the owls of 灯無, who report everything they find whether or not you asked. **She pays no Vision and nobody has told her Ardo does** |
| **Souji** | Chūnin, 10. Failed his own bloodline's three-save test by three points; 不倒樹 **Futōju** took him and Hiruzen put him down with Enma. **根の記憶 is permanent** — a real piece of bloodline knowledge every session, in his own furious voice. Signed with the tortoises of 石沼, a house that keeps a ledger **running both directions** |

### The Bequest **[the reframe that changed the campaign]**

What was called a monster growing in Ardo is not one. The seal's inward-facing linework was never built to keep something in — **it was built to keep something from being taken.** A dying woman in a burning house wrote a will on her own infant, and the thing inside was a **trustee**, administering an estate for eight years until the child could carry it. **荒神 Aragami is the inheritance coming out of trust.**

The danger was never possession. **It is inheritance velocity**, and the trap is atrophy rather than conquest.

**Standing GM rule:** *Mandatory Arc Beats* (Book IV §5, Part Eight) — 1–2 GM-initiated spotlight moments per PC per session, the GM's job to deliver rather than the player's to request.

### Live threads

- **The Uchiha taboo** — Suzume's eye is in a non-Uchiha's head, unsanctioned. Hiruzen calls that an *incident* rather than a scandal if it surfaces during the war.
- **Danzō withdrew rather than retreated**, and made Roku deliver the news personally.
- **潮風 Shiokaze**, the fourth coil — the original form every transformation Ardo ever "invented" was a copy of. Found, breathing, **not taken.**
- **Two names nobody will say.** Monuke has refused three times to name the last human who stood in Ryūchi Cave. Hiruzen would not name the boy who walked out past Konoha's walls looking for answers and never came home.
- The Handler and the Shepherd's judgment, both pending from Session Seven.

See `characters/`, `the-seam.md`, and `squad-two-journey.md` for full mechanics, session logs, and open threads.
