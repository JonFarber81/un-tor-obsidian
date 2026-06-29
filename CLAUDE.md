# CLAUDE.md

This is a personal Obsidian vault for playing **The One Ring 2nd Edition (TOR2e)** in **Strider Mode** (solo/duet, no Loremaster). It's used to track campaigns, reference rules, and store notes. New reference material, PDF annotations, and rules summaries will be added over time.

---

## Game System Context

**The One Ring 2e** uses:
- Three attributes: **Strength**, **Heart**, **Wits** — each with a Target Number (TN)
- **Endurance** (physical vitality) and **Hope** (morale/spiritual stamina)
- 12 skills organized under the three attributes
- **Shadow** (corruption) tracked per character, with individual Shadow Paths
- Two phase types: **Adventure Phase (AP)** for active play, **Fellowship Phase (FP)** for downtime
- **Strider Mode** adds oracle tables and solo-play mechanics on top of the standard rules

**Active campaign:** Hamar (Dwarf Treasure Hunter) + Leylin (Hobbit Messenger), patroned by Bilbo Baggins, currently in the Trollshaws (Phase 2.2).

---

## Vault Structure

```
_Assets/Templates/      # Source of truth for file structure — always use these
_Assets/Reference/      # Rules, cultures, callings, weapons, adversaries
_Assets/PDFs/official/  # User-supplied rulebook PDFs (not in git, copyright)
_Assets/PDFs/custom/    # Custom PDFs and reference sheets

Hamar and Leylin/       # Active campaign
  PCs/                  # Character sheets
  NPCs/                 # NPC files
  Phases/               # Session notes, named [Season].[Num] AP/FP - Title
  An Unlikely Duo.md    # Company sheet (Dataview-powered index)
  Factions.md           # Faction tracking

New Company/            # Blank campaign template — copy for new campaigns
```

---

## File Conventions

**YAML frontmatter** drives Dataview queries — keep properties consistent with templates. Key properties used across files:

- PCs/NPCs: `Culture`, `Calling`, `Company`, `Endurance`, `Hope`, `Shadow`, `Skills`
- Phases: `Company`, `Phase` (number), `Type` (AdventurePhase | FellowshipPhase), `Date`
- Tags: `#PC`, `#NPC`, `#Company`, `#AdventurePhase`, `#FellowshipPhase`

**Phase naming:** `[Season].[Number] AP/FP - Title.md` — the number prefix controls sort order.

**Reference files** in `_Assets/Reference/` follow a consistent callout structure using `[!combat]`, `[!Council]`, `[!Rolls]` blocks. Match this style when adding new reference material.

**PDF references** use the PDF++ plugin syntax to embed page ranges from rulebooks. When adding PDF-backed reference notes, store the PDF in `_Assets/PDFs/` and link by filename.

**Always link to source PDFs** when referencing rules, culture sheets, callings, or any content from a sourcebook. Use the PDF++ inline link format:
- Plain page link: `[[TOR_Core_Rules.pdf#page=42|Core Rules p.38]]`
- Embedded excerpt: `![[TOR_Core_Rules.pdf#page=42&rect=72,454,301,597|label]]`

Known PDFs in `_Assets/PDFs/official/`:
- `TOR_Core_Rules.pdf` — main rulebook (cultures: Bardings p.36, Dwarves p.38, Hobbits p.42, Men of Bree p.40, Rangers p.46, Elves of Lindon p.46)
- `TOR_Peoples_of_Wilderland.pdf` — Beornings p.2, Elves of Mirkwood p.5, Woodmen p.8
- `TOR_Rivendell.pdf` — High Elves of Rivendell p.10
- `TOR_Strider_Mode.pdf` — solo/oracle mechanics
- Other supplements: `TOR_Realms_of_the_Three_Rings.pdf`, `TOR_Moria.pdf`, `TOR_Hobbit_Tales.pdf`, etc.

When writing or updating any reference note, add a `[[PDF#page=N]]` link at the top and use page links inline wherever a rule is cited. If you don't know the page number, read the relevant PDF to find it before writing the note.

---

## What Will Be Added Over Time

- Rules references and summaries (Strider Mode mechanics, journey rules, council rules)
- Culture and calling deep-dives, potentially PDF-backed
- New adversary stat blocks in `_Assets/Reference/Adversaries/`
- Session notes as new Phase files under the active campaign
- NPC and faction notes as the campaign develops
- Possibly new campaigns in their own top-level folders (copied from `New Company/`)

---

## Obsidian CLI

The Obsidian CLI is available at `/Applications/Obsidian.app/Contents/MacOS/obsidian-cli` and connects directly to the running Obsidian app. **Use it whenever possible** instead of raw file tools — it is vault-aware, resolves wikilinks, and handles YAML properties correctly.

Key commands (always pass `vault="un-tor-obsidian"` to target this vault):

```bash
OBS="/Applications/Obsidian.app/Contents/MacOS/obsidian-cli vault=un-tor-obsidian"

$OBS read path="Hamar and Leylin/PCs/Hamar.md"       # read a file
$OBS search "shadow"                                   # search vault text
$OBS files                                             # list all files
$OBS property:read path="..." name="Shadow"           # read a frontmatter property
$OBS property:set path="..." name="Shadow" value="4"  # update a frontmatter property
$OBS create path="..." content="..."                   # create a new note
$OBS append path="..." content="..."                   # append to a note
$OBS backlinks file="Hamar"                            # find all links to a note
$OBS links path="..."                                  # list outgoing links
```

Use `property:set` / `property:read` for all frontmatter changes rather than raw YAML edits. Use `search` before reading files to quickly locate relevant content.

---

## How to Help

When asked to help with this vault:

- **New session notes:** Use `_Assets/Templates/Phase-Template.md` as the structure. Match the existing phase files in `Hamar and Leylin/Phases/` for formatting and YAML.
- **New reference material:** Match the style of existing files in `_Assets/Reference/`. Use callout blocks for rules excerpts. Don't reproduce copyrighted text — summarize or reference PDF page numbers.
- **Character updates:** Edit the YAML frontmatter in `PCs/` files to track stat changes. The company sheet Dataview queries read from these.
- **New adversaries:** Follow the YAML stat block format in `_Assets/Reference/Adversaries/` — the TOR 2E Statblocks plugin renders these.
- **Rules questions:** Reference `_Assets/Reference/Rules.md` and `_Assets/Reference/TOR Cheat Sheet.md` before asking to look elsewhere.

When in doubt about structure, look at how existing files in the campaign are organized rather than inventing new conventions.
