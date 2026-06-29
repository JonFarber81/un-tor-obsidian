# tor_vault

A personal [Obsidian](https://obsidian.md) vault for playing **The One Ring 2nd Edition (TOR2e)** by Free League Publishing — specifically **Strider Mode**, the solo/duet rules for playing without a dedicated Loremaster.

---

## What This Is

This vault is a living play-space: part rulebook index, part campaign journal, part reference library. As the game grows, so does the vault — new reference material, PDF annotations, house rules, and session notes all live here.

**Current campaign:** Hamar (Dwarf Treasure Hunter) and Leylin (Hobbit Messenger), operating out of the Shire under the patronage of Bilbo Baggins. Currently in the Trollshaws, tracing a web of ancient maps and competing factions centered on a mysterious antagonist called the Spider.

---

## Vault Structure

```
tor_vault/
├── _Assets/                    # Shared infrastructure — don't put campaign content here
│   ├── Templates/              # 9 templates for characters, sessions, encounters, etc.
│   ├── Reference/              # Game rules, cultures, callings, weapons, adversaries
│   │   └── Cultures/           # Per-culture breakdowns + PDF references
│   ├── PDFs/
│   │   ├── official/           # Place TOR2e rulebook PDFs here (not included, copyright)
│   │   └── custom/             # Custom reference PDFs
│   └── Images/                 # Character portraits, location banners, tokens
│
├── Hamar and Leylin/           # Active campaign folder
│   ├── An Unlikely Duo.md      # Company sheet (Dataview auto-lists PCs & phases)
│   ├── Factions.md             # Faction notes and relationships
│   ├── PCs/                    # Player character sheets
│   ├── NPCs/                   # Non-player characters
│   └── Phases/                 # Numbered session notes (AP = Adventure, FP = Fellowship)
│
└── New Company/                # Blank campaign starter — copy this for new campaigns
```

---

## Key Conventions

**Phase numbering:** `[Season].[Number] AP/FP - Title` — e.g., `2.1 AP - The Trollshaws`. AP = Adventure Phase, FP = Fellowship Phase.

**YAML frontmatter:** All PC, NPC, and Phase files use structured YAML properties. Dataview queries in company sheets pull from these — keep them consistent with the templates.

**PDF references:** The PDF++ plugin embeds annotated excerpts from rulebooks. PDFs go in `_Assets/PDFs/official/` and are linked by filename from reference notes.

**Templates:** Always create new content from `_Assets/Templates/`. Copy the appropriate template, rename, and fill in — don't create files from scratch.

---

## Plugins Required

| Plugin | Purpose |
|--------|---------|
| Dataview | Auto-populates PC/phase lists on company sheets |
| Dice Roller | In-note TOR dice rolls |
| TOR 2E Statblocks | Renders YAML adversary blocks |
| Obsidian Excalidraw | Visual combat tracker |
| PDF++ | Embeds rulebook excerpts |
| Solo RPG Toolkit | Strider mode oracle/randomizers |

This vault is built on top of [un-tor/un-tor-obsidian](https://github.com/un-tor/un-tor-obsidian) — see that repo's `Readme.md` and `Getting Started.md` for initial Obsidian setup.

---

## Legal

Personal notes and references for non-commercial fan use. The One Ring is © Free League Publishing. No copyrighted rules text is reproduced — PDF excerpts are embedded locally via PDF++ and require you to own a copy of the rulebooks.
