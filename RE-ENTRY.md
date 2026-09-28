# Re-entry guide
*Written 2026-09-28 against draft 77 · 28 of 39 decisions decided · last real work: D022 (Founding Catastrophe, Suppression, Verification) and D039 added as open*

Read this first after a long break. It is a map, not a source of truth. [[WORLD]] is canonical; [[CLAUDE]] holds the invariants and edit rules.

---

## 1. The project in five lines

- Speculative-fiction worldbuilding for a tactical turn-based RPG. World first; game concerns are audited afterward ([[GAME_DESIGN]]), never used as gates.
- Two factions fight over territory valued by **Vein** concentration. The Vein *moves* energy, it does not generate it, and both sides deplete the same reservoir.
- **Attuned Order**: oligarchic, ~2000 years old, biologically attuned (bone piezoelectricity + neural coupling). Its ceiling is cultural taboo.
- **Forge Coalition**: constitutional federal democracy, mechanical apparatus. Its ceiling is mechanical speed. It escaped the Order and held territory. It did not win.
- The tone is analytical, not narrative, and no proper nouns get invented (names are open decisions).

## 2. Thirty-minute re-read order

1. [[CLAUDE]] — invariants and edit rules (already auto-loaded in Claude sessions, but read it yourself once).
2. [[WORLD#What this document is for|WORLD: What this document is for]], then [[WORLD#The resource|The resource]] and [[WORLD#The two factions — overview|The two factions — overview]].
3. [[WORLD#The historical sequence|The historical sequence]] (contains the newest content: founding catastrophe, Suppression, Verification).
4. [[WORLD#What is not yet decided|What is not yet decided]] — the living gap list.
5. [[WORLDBUILDING_RULES]] — the checklist to run on anything new.
6. Skim only when needed: [[working/MATERIALS_BASELINE|MATERIALS_BASELINE]], [[working/refinement_axis|refinement_axis]], [[REFERENCES]].
7. Optional: [[WORLD_ANALYSIS]] — the last full consistency audit (against draft 76): no invariant violations found.

## 3. Where things stand

**Recently written into WORLD.md (drafts 74–77):** industry giants (D024), peripheral actors (D014), founding catastrophe (D022, draft 76), the Suppression/Burning and Verification (D022, draft 77).

**Last commit:** added D039 (inter-war conflict history) as an open decision point. A new artifact, `artifacts/atrocity_timeline_v1.html`, is the D022 workshop tool. `artifacts/continent_geography_workshop.html` supports D013.

**Open decisions (11):**

| ID | Title | Priority | Depends on |
|----|-------|----------|-----------|
| D023 | Daily life — ordinary people on each side | high | D017, D013 (both decided) |
| D020 | Bloodline consolidation mechanism | medium | D016 (decided) |
| D037 | Religious arm — full operational picture | medium | — |
| D025 | Secret societies — full operational picture | medium | — |
| D036 | Gas-phase substrate × biological barrier | medium | — |
| D038 | Vein overexposure — external presentation | medium | D028 (decided) |
| D039 | Inter-war conflict history (+1760–1970) | medium | D013, D022 (both decided) |
| D006 | Exotic states of matter beyond plasma | medium | — |
| D001 / D007 / D009 | Resource name / animal attunement / faction names | low | — |

## 4. Recommended next move

**D023 — daily life.** It is the only high-priority open item, both dependencies are decided, and it closes the known asymmetry (Coalition daily life is thinner than the Order's). Run it with `/resolve D023`.

Good follow-ups, in order: D039 (now unblocked, and it feeds the atrocity registry), then D020 → D037 (Order character work depends on these).

## 5. The working loop

1. `/resolve <id>` — diagnostic first, resolve in dependency order, small decisions over large text blocks.
2. Check the result against the invariants and [[WORLDBUILDING_RULES]]. Check faction parity.
3. Write into **all** affected files: WORLD.md (bump the draft number), `decisions.json` (edit via code, verify it parses, clear `refactor_flags`), and INDEX.md.
4. **Commit before moving on**, with the draft number: `draft 78 — <what>`.
5. `/audit` periodically for a consistency pass.

## 6. Housekeeping: known drift to fix

Found while writing this. None of it is content-breaking, but [[INDEX]] is stale.

- INDEX says WORLD is at **draft 74**. It is at **77** (the header of INDEX itself says "generated from draft 77").
- INDEX's section headed "Decided (26)" lists 28 rows.
- INDEX priority queue skips item 2, and doesn't list D038 or D039 in it.
- `decisions.json` titles contain mis-encoded dashes when printed on Windows (the `—` shows as `�`). Check the file's encoding if that appears in diffs.
- `.obsidian/workspace.json` shows as modified in git. It is noise from Obsidian, so consider adding it to `.gitignore`.

## 7. Don't

- Don't make game design decisions. Flag them in [[GAME_DESIGN]].
- Don't resolve deferred decisions unasked.
- Don't write narrative prose or invent proper nouns.
