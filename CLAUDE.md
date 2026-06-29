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

---

## What Will Be Added Over Time

- Rules references and summaries (Strider Mode mechanics, journey rules, council rules)
- Culture and calling deep-dives, potentially PDF-backed
- New adversary stat blocks in `_Assets/Reference/Adversaries/`
- Session notes as new Phase files under the active campaign
- NPC and faction notes as the campaign develops
- Possibly new campaigns in their own top-level folders (copied from `New Company/`)

---

## How to Help

When asked to help with this vault:

- **New session notes:** Use `_Assets/Templates/Phase-Template.md` as the structure. Match the existing phase files in `Hamar and Leylin/Phases/` for formatting and YAML.
- **New reference material:** Match the style of existing files in `_Assets/Reference/`. Use callout blocks for rules excerpts. Don't reproduce copyrighted text — summarize or reference PDF page numbers.
- **Character updates:** Edit the YAML frontmatter in `PCs/` files to track stat changes. The company sheet Dataview queries read from these.
- **New adversaries:** Follow the YAML stat block format in `_Assets/Reference/Adversaries/` — the TOR 2E Statblocks plugin renders these.
- **Rules questions:** Reference `_Assets/Reference/Rules.md` and `_Assets/Reference/TOR Cheat Sheet.md` before asking to look elsewhere.

When in doubt about structure, look at how existing files in the campaign are organized rather than inventing new conventions.
