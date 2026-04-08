# CLAUDE.md

This is a speculative fiction worldbuilding project for a tactical turn-based RPG. The world is built first; game design concerns are audited against it afterward, not used as gates.

## Project overview

Two factions fight over territory whose value is determined by concentration of **the Vein**, a finite geological energy resource.

- **The Attuned Order**: Oligarchic institution organized around biological sensitivity to the Vein. Founding families hold political authority. Religious arm escaped family control. Military split between family-placed and risen commanders. Secret societies perform subordination while accumulating capability.
- **The Forge Coalition**: Constitutional federal democracy that developed mechanical apparatus to interact with the Vein at extraction concentrations. Three tiers of elected government, partially elected constitutional court, four political tensions (attuned emergence, war aggression, science speed, industrialization costs).

## Files

This is an Obsidian vault. Files use `[[wiki-links]]` for navigation; use `[[file#heading|display text]]` for section links.

### Canonical
- [[WORLD]] — Prose document. **The source of truth.** Currently at draft 74. Claude Code may edit this directly with user approval.
- `decisions.json` — Structured registry of all decisions (open, in-progress, decided). Update via code, verify after every edit.
- [[INDEX]] — File registry, section map, decision tables, priority queue, key invariants, process notes. Keep in sync with WORLD.md and decisions.json after each significant update.

### Reference
- [[GAME_DESIGN]] — Game design concerns as future audit checklist. Not active blockers for worldbuilding.
- [[working/MATERIALS_BASELINE|MATERIALS_BASELINE]] — Canonical material reference. Full profiles for all story-present materials. WORLD.md links out to it.
- [[working/refinement_axis|refinement_axis]] — Refined substrate four-axis development by era.
- [[WORLDBUILDING_RULES]] — Quality checklist. Run against decisions and new content: Vein system laws, faction parity, narrative utility test, common failure modes.
- [[REFERENCES]] — Tonal and structural references. The five threads at the top are worldbuilding constraints, not just tone.

Working documents either graduate to WORLD.md (content merged in, file removed) or become standalone reference docs that WORLD.md links to. MATERIALS_BASELINE is an example of the latter.

### Artifacts (HTML interactives — open in browser or embed in Obsidian)
- `artifacts/materials_taxonomy_v4.html` — Interactive materials taxonomy
- `artifacts/coalition_political_compass.html` — Political compass visualization
- `artifacts/coalition_capability_arc_v2.html` — Capability arc grid
- `artifacts/refinement_profile_builder.html` — Radar tool with presets

## Key invariants (never contradict)

- The Vein does not generate energy. It moves energy. Both factions deplete the same reservoir.
- Dense substrate and diffuse field expression are the same phenomenon at different concentrations.
- Attunement = bone piezoelectricity (antenna) + neurological coupling (translator). Both heritable like height.
- Biological barrier tied to field concentration — Coalition extraction lowers both.
- The Coalition did not win the liberation war. They escaped and held territory.
- Mechanical speed is the hard ceiling preventing Coalition apparatus from matching Order at human scale.
- Degradation is two-mode: temporary (recovers at rest) and permanent (requires reprocessing). Do not collapse.
- Matter form is orthogonal to the capability arc — affects speed/efficiency, does not unlock capability tiers.
- Shape = internal geometric coherence of mirror faces, not orientation relative to apparatus.
- Size drops out at personal scale — weight budget fixes it at manufacture.
- Order institutional ceiling is cultural taboo, not physical limit. Secret societies preserve exotic state knowledge.
- The Order's institutional blindness is two-layer: reporting incentives + founding catastrophe complacency.
- The religious arm escaped family control — a real institutional fracture, not by design.

## Edit rules

- **WORLD.md**: Edit directly with user approval. Increment draft number in the document when making changes. Write in the analytical register used throughout the document — not narrative, not flowery.
- **decisions.json**: Edit via code. Always verify the file parses after editing. When adding decisions, follow the existing schema (id, title, status, category, priority, world_md_line, summary, depends_on, blocks). Use `decided_text` for decided items, `session_notes` for in-progress context. Some decided entries carry `refactor_flags` — these point to WORLD.md sections that need updating. Check and clear them when writing that content into WORLD.md.
- **INDEX.md**: Keep in sync after WORLD.md or decisions.json changes. Update section map, decision tables, and priority queue.
- **Git**: Commit after each significant update. Use draft number in commit message (e.g. "draft 50 — wartime distortion section"). **When a decision is locked, write it into all affected files first, then commit — before moving to the next decision or topic.**

## Formatting Conventions
- Maintain Obsidian-compatible wiki-links ([[Page Name]]) when editing Markdown files. Preserve existing cross-links and add new ones when content references other documents.

## Working style

- **Diagnostic before drafting**: Resolve decisions in dependency order before writing prose. Small decisions preferred over large text blocks.
- **Parallel faction development**: When adding to one faction, check the other for parity. Both sides should stay at comparable depth.
- **Consistency matters**: Before adding new content, check it against key invariants and existing WORLD.md content. Flag contradictions immediately.
- **Story utility as criterion**: Worldbuilding decisions evaluated against whether they can function in narrative, not just internal consistency.
- **Defer when complex**: Genuinely complex gaps get flagged for dedicated sessions rather than resolved piecemeal.

## Current state and priorities

### Recently completed
- Culture layer (D034): cross-faction encounters, interrogation, indoctrination pipeline, folk psychology — all written into WORLD.md
- Wartime folk culture distortion (draft 52–53): performance pressure, death belief, non-attuned calcification, secret society tension (Order); borrowed clarity, meritocracy/death, veteran dissonance (Coalition)
- D019 decided: materials taxonomy complete, lives in MATERIALS_BASELINE
- D035 decided: Order demographics (30/70 att/non-att pre-liberation; 70/30 current Order)

### Priority queue
1. Geography and site distribution (D013)
2. Story structure decisions: D002/D003, D008, D011, D012
3. Industry giants full operational picture (D024)

## What not to do

- Do not make game design decisions. Flag game-relevant implications in [[GAME_DESIGN]].
- Do not resolve deferred decisions without being asked. They were deferred for a reason.
- Do not write narrative prose. WORLD.md is analytical and descriptive.
- Do not invent proper nouns. Faction names, character names, place names are all open decisions.
