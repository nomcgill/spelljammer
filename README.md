# The Next Jump

This directory contains all the context, plot and organizational material for a D&D 5e Spelljammer campaign called "The Next Jump".

Nolan runs the campaign and is the only person with access to this repo. The other reader is the AI agent that maintains these files. Documents refer to him by name rather than as "you" or "the DM", so that both readers always know who is meant.

## What this directory is for

This is the **source of truth** for the campaign. Anything that has happened at the table, or that Nolan has decided is true, lives here in Markdown. The goal is that he never has to dig through a pile of raw session notes to answer "wait, who was that guy?" or "what did we leave unresolved?"

The agent has two jobs here:

1. **Answer questions.** Nolan asks things in chat — about a character, an NPC, a dangling plot thread, what happened three sessions ago — and the agent answers quickly from these files.
2. **Keep the documentation current.** Nolan drops new information in chat (session notes, decisions, character changes) and the agent files it into the right documents.

## Where the campaign stands

Season 1 ran seven sessions. The party escaped Warden's Maw and spent the whole season trying to reach the Rock of Bral. In the finale a plasmoid warship disabled and boarded their Damselfly. Marfa Ruth beamed them out, Korran hijacked a small ship from the mothership, and **everyone finally made it to Bral**. There, Pip plans to gather allies for a revolution against his usurping brother, the plasmoid king.

Season 2 is under way, and its main plot driver is **Korran's past**. Matt isn't playing, so the party is **Korran (Brad), Luckyluciano (Nicole) and Pip (Drew)**. Tamenik went home to Freelin Corporation in Session 1.

In Session 1 the party docked on Bral and told Marfa Ruth their whole story over breakfast. When she asked for help with **the Case of the Missing Stromboli**, a Kenku assassin attacked and then disintegrated itself. Session 2 prep is in [`season2/session2-brainstorm.md`](season2/session2-brainstorm.md). Start with [`plot/timeline.md`](plot/timeline.md) for the story so far, and [`plot/open-questions.md`](plot/open-questions.md) when prepping the next session.

## Setting and rules

The campaign uses [Spelljammer: Adventures in Space](https://www.dndbeyond.com/sources/dnd/sais) as its setting, but **only loosely**. Nolan departs from the book freely on both setting and rules — Season 1 includes homebrew like the ship's hyperspace drive, and the deck plan his players use does not match the book's ship stats.

So: **the table beats the book.** What happened in play and what Nolan has decided are canon. Published Spelljammer material is background colour, useful for filling gaps and suggesting ideas, never a correction. The agent should not "fix" notes to match the book, flag a deviation as an error, or assume a book detail applies unless Nolan has confirmed it.

The agent also cannot read the book's text — it is behind a paywall — so it knows the setting only in general terms and has no access to exact stat blocks, deck plans, or rules text. When a specific number or mechanic matters, Nolan pastes it in. Published creature stats quoted in this repo were looked up from public references, with the source noted.

## Structure

| Path | Contents |
| --- | --- |
| [`plot/`](plot/) | The timeline, every open and resolved thread, the questions still to answer, and the [Season 2 plan](plot/season2-planning.md) (including Nolan's hook bank) |
| [`player-characters/`](player-characters/) | One file per PC: player, build, background, and what they did in Season 1 |
| [`npcs/`](npcs/) | One file per named NPC. Start at [`npcs/README.md`](npcs/README.md) for the roster |
| [`locations/`](locations/) | One file per place. Start at [`locations/README.md`](locations/README.md) for what's returning and what was Season 1 only |
| [`ships/`](ships/) | One file per ship. Start at [`ships/README.md`](ships/README.md) for what's active and what's undecided |
| [`bestiary/`](bestiary/) | Every encounter with its roster and stat summaries, one file per season |
| [`factions.md`](factions.md) | The organisations, and which PC each one has a claim on |
| [`items.md`](items.md) | Treasure, magic items, and what the party is actually carrying |
| [`house-rules.md`](house-rules.md) | Homebrew: hyperspeed, Blackstar Fever, ship combat, creature reskins |
| [`season1/`](season1/) | Session notes, opening prompt, and Session 0 recap |
| [`season2/`](season2/) | Season 2 [session notes](season2/session-notes.md), plus per-session plans and brainstorms |

Original source material lives in Google Docs and is linked from the files that draw on it — the [main session notes doc](https://docs.google.com/document/d/18MwI1hvspOiyi9dtMP8RiN7W1wXKQThmwJ8ilMqnvCg/edit) and three per-character backstory docs.

## Conventions

These exist so the documents stay trustworthy over a long campaign.

- **Naming.** Directories and files are lowercase kebab-case, one subject per file: `player-characters/first-last.md`, `npcs/first-last.md`.
- **Raw notes are never edited or deleted.** The Google Docs remain the authoritative originals. Curated documents are derived from them and link back, so any claim can be traced to its source.
- **Never invent lore.** If something is unclear or missing, the agent asks, or marks it `[unconfirmed]` rather than guessing. A plausible-sounding fabrication in a source-of-truth document is worse than a gap.
- **Contradictions get raised, not resolved.** Where the notes disagree with themselves, both versions are recorded in [`plot/open-questions.md`](plot/open-questions.md) and Nolan decides which is canon.
- **Track what the party knows.** Where it matters, files separate established knowledge from what the players haven't learned — so Nolan can see at a glance what has actually been revealed at the table and avoid contradicting himself.
- **Session notes are history; everything else is present tense.** The session log describes what happened and doesn't change. Character, NPC, location and ship files describe how things stand *now* and get rewritten as the campaign moves.
- **Track seasons in place.** Files stay where they are across seasons; nothing is moved or archived without asking Nolan first. Instead:
  - Every NPC, location, ship and PC file has an `**Appears in:** Season 1` line under its title. Add `Season 2` (and so on) when the subject shows up in a later season.
  - Timeless material (stats, who someone is, what a place is, family) and current status sit at the top of a file. What happened in play goes under a `## Season N` heading at the bottom, one per season, with `###` subsections.
  - The index pages — [`npcs/README.md`](npcs/README.md), [`locations/README.md`](locations/README.md), [`ships/README.md`](ships/README.md) — say what carries forward (`Yes`, `Season 1 only`, or `Undecided`). Only Nolan moves something out of `Undecided`.
  - [`plot/timeline.md`](plot/timeline.md) has one `## Season N` section per season, [`plot/threads.md`](plot/threads.md) tags each thread with the season it opened, and [`items.md`](items.md) notes when each item was acquired.
- **Preserve links.** Nolan's notes contain external links (D&D Beyond, Google Docs, maps); carry them through into the curated docs.
- **Cross-reference generously.** Relative Markdown links between PCs, NPCs, locations, ships and the sessions they appear in are what make this browsable.

## Workflow

When Nolan gives new information in chat, the agent:

1. Identifies which documents are affected.
2. Updates them, creating new files or folders as needed.
3. Reports back briefly on what changed, and flags anything contradictory or ambiguous rather than silently picking an interpretation.

Contradictions with existing notes get raised, not resolved unilaterally — Nolan decides what is canon.

When Nolan is planning or asks for inspiration, the agent checks **[Nolan's hook bank](plot/season2-planning.md#nolans-hook-bank)** first and draws on those ideas. Any new hook Nolan mentions gets added there.
