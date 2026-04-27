# WORLD.md — consistency and gap analysis
*Run against draft 76 · 2026-04-22*

This audits [[WORLD]] against the key invariants in [[CLAUDE]], the checklist in [[WORLDBUILDING_RULES]], and the decision registry in `decisions.json`. It does not propose content — it flags what is consistent, what is drifting, and what is genuinely missing.

---

## 1. Invariant consistency

WORLD.md draft 76 does not contradict any of the 14 key invariants in [[CLAUDE#Key invariants (never contradict)|CLAUDE.md]]. Each invariant was checked against the section that most directly encodes it:

| Invariant | WORLD.md anchor | Status |
|-----------|-----------------|--------|
| Vein moves energy, does not generate it | L49–51 | Consistent. Energy-continuum framing in L85–87 reinforces it. |
| Dense substrate / diffuse field = same phenomenon | L37–47 | Consistent. Articulated explicitly ("same thing at different concentrations"). |
| Attunement = bone antenna + neural translator | L201 | Consistent. Two-component mechanism stated; heritability "like height" at L227. |
| Biological barrier tied to field concentration | L21, L205, L579 | Consistent across resource, overexposure, and liberation-war sections. |
| Coalition did not win liberation war; they held | L577–581 | Consistent. Explicit: "partition because the Order could not dislodge an entrenched force." |
| Mechanical speed = hard ceiling | L735 | Consistent. Phase 3 apparatus is "clockwork approximation" of attunement. |
| Degradation two-mode (temporary vs permanent) | L211 | Consistent, though not named as "two-mode" in prose — see §4 below. |
| Matter form orthogonal to capability arc | L79 | Consistent. Explicitly stated. |
| Shape = internal geometric coherence, not orientation | decisions.json D005 decided_text | **Consistent but under-surfaced in WORLD.md** — see §4. |
| Size drops out at personal scale | L79 | Consistent (weight budget at manufacture). |
| Order ceiling is cultural taboo, not physical | L93–101 | Consistent. Societies preserve exotic-state knowledge. |
| Two-layer institutional blindness (reporting + complacency) | L271–273 | Consistent. Named explicitly. |
| Religious arm escaped family control | L259 | Consistent. "Instrument to quid pro quo" — real fracture, not by design. |

**No invariant violations found.** The document's discipline around invariants is strong.

---

## 2. Cross-section consistency

### 2.1 Resolved tensions (verified)

- **Pre-liberation demographics vs. current demographics.** Pre-liberation 30/70 att/non-att (L363) with 80%+ of non-attuned leaving (L365) yields ~68/32 in the current Order — matches the stated ~70/30 (L365) within rounding. Coalition ~5% attuned (L371) is consistent with defector-lineage dominance plus 1% emergence compounding over 8–10 generations (L233).
- **Two-thousand-year Order / 8–10 generation liberation.** L553 and L565 agree; liberation placed ~250–300 years ago is consistent across the historical sequence.
- **Liberation war vs. post-partition extraction.** L581–583 explicitly separates offensive apparatus use during the war from extraction-at-scale after partition — preventing the invariant violation that would otherwise follow from "barrier erosion began during the war."
- **Selective retention, not biological change.** L365 explicitly flags the demographic inversion as a departure artifact, distinct from the desensitization mechanism in L213. This is a live trap the document avoids cleanly.

### 2.2 Soft tensions — not contradictions, but worth flagging

1. **D008 decided_text drift.** The decision's title and summary frame it as "Attuned Coalition members erased from founding records" (this is the Coalition's buried history). Its `decided_text`, however, is about Order founding-figure mythology and the secret societies' remainder. The Coalition-side erasure is covered by D010 (Coalition buried history). D008 appears to have evolved during the session and absorbed Order-side content without the title/summary updating to reflect it. Not a WORLD.md contradiction, but a registry hygiene issue that makes cross-referencing harder.

2. **Founding catastrophe scope and the "two-thousand-year" timeline.** L553 says the founding catastrophe coincides with the Order's founding (~2000 years ago). L555 says the catastrophe "was not a single event but a period." This is consistent but leaves an unresolved edge: was there a pre-Order civilization that discovered exotic states and fractured into the Order during/after the catastrophe, or did the catastrophe happen *to* an existing proto-Order? The current prose is compatible with both readings, which is likely deliberate but should be noted before anything downstream is built on one reading.

3. **Contact prohibition feasibility.** L489–490 says the prohibition is "enforceable in principle" because non-attuned are 30% of the Order. But 30% of a population is not a rump minority — it's a structural demographic. The line "manageable in secure interior territory; leaks near occupied zones" is doing a lot of work. D034 session notes suggest this was settled, but the prose underplays the enforcement problem that 30% creates.

4. **Transmission rate precision.** L369 says "20–30% transmission failures are the source population for the Order's internal underclass" — but L265 describes the internal underclass as "a small cohort, never large enough to exert collective pressure." 20–30% of attuned Order families producing non-attuned children is not a small cohort in absolute terms. The tension resolves if most failures are reabsorbed invisibly rather than remaining in underclass status, but the prose doesn't make that mechanism explicit.

5. **The "secret societies know more" claim.** L101 says the societies have "probably assembled enough to know the institutional account is wrong... and to have a working theory." L567 says societies preserve exotic-state knowledge as "institutional memory of capabilities the Order's general population can no longer access." These are compatible but lean on different kinds of preservation (historical reconstruction vs. living practice). The document doesn't say whether individual society members who practice exotic states personally experience the desensitization trend documented at L567, or whether their practice exempts them. This matters for D025.

### 2.3 Under-surfaced invariants

Two invariants from [[CLAUDE]] are stated in decisions.json but not clearly labeled in WORLD.md prose:

- **Degradation is two-mode.** WORLD.md discusses recoverable vs. permanent damage in overexposure (L211) but does not explicitly identify this as the two-mode model tied to substrate behavior. The substrate recovery and shape-coherence degradation discussions (D005 decided_text) are also two-mode but not surfaced in prose. A reader working only from WORLD.md would have to assemble this across three places.
- **Shape = internal mirror-face coherence, not orientation.** L71 mentions shape axis briefly; L77 describes personal composite "mirror faces internal." The coherence-not-orientation framing lives in D005 decided_text and is not visible in WORLD.md prose. If a writer reads only WORLD.md they could reasonably interpret "shape" as orientation.

These are not contradictions — they are places where the canonical definition in decisions.json is more precise than the prose, which makes drift possible in future edits.

---

## 3. Faction parity check

Using the [[WORLDBUILDING_RULES#Faction parity checklist|faction parity checklist]]:

| Check | Order | Coalition | Parity |
|-------|-------|-----------|--------|
| Institutional depth | Four branches (families, religious arm, military, secret societies). Religious arm (D037) and societies (D025) are flagged thin. | Three-tier government + constitutional court + industry giants + research frontier. | **Asymmetric depth on non-state institutions.** Coalition has industry giants at full operational picture (D024). Order has no economic actor equivalent at similar depth — the closest is "the founding families as landholders," which is described politically, not economically. |
| Internal contradiction | Ceiling vs. strategic need; secret societies' preserved capability vs. institutional acknowledgment cost (L533–535). | Attuned emergence vs. founding identity (L309–311); industry giants as "reliable financial supporters and consistent internal saboteurs" (L307). | **Both factions have strong internal fractures.** Parity held. |
| Legibility from inside | Covered — Order custodianship framing (L457, L473). | Covered — biology-is-not-merit framing (L475). | Parity held. |
| Structural blind spot | Two-layer blindness named explicitly (L271–273). | Extraction-as-depletion-mechanism invisible to military/economics split (L299–301). | Parity held; both sides have documented institutional blind spots with the same causal structure. |
| Cost of organization | Performance pressure, practitioner overextension, internal underclass shame (L265, L425–429, L529). | Anchor-holding for those who don't climb (L437); captured-independence court (L317); attuned citizens managing concealment (L415, L433). | Parity held. |
| Mirror check | | | **Two missing mirrors**: (1) Coalition's daily life (D023 open) has no equivalent depth to Order daily life (L381–389, grandmother-rule, death belief, etc.). (2) Order has no documented economic actor at industry-giants depth. |

### Parity gaps

1. **Coalition daily life (D023, open, high).** This is the single largest parity gap. The Order's folk layer is developed in depth — early attunement feats as family events, substrate talismans, grandmother-rule safety wisdom, death belief as cosmological register. The Coalition gets a paragraph (L393–395): Vein is fuel in important things, safety rules for children, coal-and-steam in the home. The registers are asymmetric: the Order's is intimate and cosmological; the Coalition's is flat and industrial. This is likely correct in direction — the Coalition's Vein relationship *is* industrial — but the asymmetry makes the Coalition feel thinner as a culture than the Order, not as a doctrine. This parity gap is the priority queue's #2 item and it is the right call.

2. **Order non-state economic actor.** The Coalition has the industry giants at extensive depth (L325–357). The Order's comparable actor is not documented. Candidates the prose hints at but does not develop:
   - Landed founding families' estate economies (L257 mentions land as a power base; nothing further)
   - Merchant guilds or craft institutions moving goods across Order interior
   - Whatever organizes the apparatus-dismantling occupation labor (L483)
   
   Not a current decision. If Order characters operate outside the four named branches, there is currently no institutional texture for them.

3. **Coalition religion/non-religion posture.** The Coalition's shame category around mystical Vein-register (L435) is developed. The Coalition's relationship to non-Vein religion is absent. A 250–300-year-old rationalist civilization descended from Order-subjugated non-attuned people would have specific religious history — what faiths did the pre-liberation non-attuned majority hold? Did the founding identity suppress them, absorb them, or leave them alone? Currently unaddressed.

---

## 4. Open decisions vs. WORLD.md state

10 open decisions are registered. Their current prose-state in WORLD.md:

| ID | Title | Prose state |
|----|-------|-------------|
| D001 | Resource name | Placeholder `[OPEN]` at L17. Correct — nothing to fix. |
| D006 | Exotic states beyond plasma | Placeholder `[OPEN]` at L87. Correct. |
| D007 | Animal attunement | Placeholder `[OPEN]` at L189. Correct. |
| D009 | Faction final names | Placeholder `[OPEN]` at L249. Correct. |
| D020 | Bloodline consolidation mechanism | Referenced in "What is not yet decided" (L778). No in-line flag in the relevant historical section (L227 discusses it without flagging the mechanism as open). |
| D023 | Daily life | Referenced in "What is not yet decided" (L781). **Not flagged in the culture sections themselves.** A reader reading the Coalition daily-life paragraph at L393 has no signal that this is thin. |
| D025 | Secret societies full picture | Referenced at L776. Not flagged at L263 where societies are introduced. |
| D036 | Gas-phase / biological barrier | Referenced at L784. Partial flag via D005 decided_text session notes, not in WORLD.md prose. |
| D037 | Religious arm full picture | Referenced at L777. Not flagged at L259 where the arm is introduced. |
| D038 | Overexposure external presentation | Referenced at L775. Not flagged in the overexposure mechanism prose (L205–215). |

### Pattern

Placeholder `[OPEN]` markers exist in-line where the placeholder is the content (names, beyond-plasma states, animal attunement). Decisions where existing prose is *partial* do not have in-line flags — a reader following links from WORLD.md learns about openness only via the "What is not yet decided" list at the document's bottom.

**Recommendation**: add in-line `[OPEN: Dxxx]` markers at D023, D025, D036, D037, D038 anchors so that a reader hitting partial content in-situ knows the rest is pending. This is the same pattern used at L87 and L189 and works well there.

---

## 5. Metadata sync issues

(This is the focused scope of the `audit` skill; listing here rather than running it now because the user asked for content analysis.)

1. **`decisions.json` `meta.doc_version`** = `draft 74`. WORLD.md is at draft 76. Stale.
2. **INDEX.md Files table** says WORLD is at Draft 74 (L10). Header says "Generated from draft 76" (L2). Internal inconsistency.
3. **INDEX.md decided table header** says `### Decided (26)` (L62). The table actually contains 27 rows. Count is wrong by one (D014 was added and the count wasn't incremented, or similar).
4. **INDEX.md has two "In progress" sections** (L94 and L96). One says `(0)` and is empty; the other has D022. Merge into a single section.
5. **Stale `world_md_line` values in `decisions.json`** (selected):
   - D008 → 211 (bio section) vs. actual content at ~L279 (founding figures myth structure)
   - D010 → 251 (Order section heading) vs. actual content at ~L287 (Coalition buried history)
   - D011 → 311 (Coalition body) vs. actual content at L595–605 (war trigger)
   - D013 → 539 (wartime distortion) vs. actual content at L611+ (Geography)
   - D014 → 633 (eastern seaboard) vs. actual content at L641+ (Peripheral actors)
   - D034 → 415 (Coalition margins) vs. actual content at L479+ (Cross-faction encounters)
   - D035 → 311 (Coalition body) vs. actual content at L359+ (Demographics)
6. **`world_md_line: null` on decided entries that are written in**: D015, D019, D026, D027, D028, D029, D030, D031, D032, D033. These were written when the decisions were integrated but not back-filled into the registry.
7. **CLAUDE.md `Current state and priorities` priority queue is stale**. It lists D013, D002/D003, D008, D011, D012, D024 — all of which are now decided. The actual current priorities (per INDEX.md) are D022 in-progress, then D023, D020, D037, D036.

---

## 6. Content gaps

Separating from registered open decisions — these are things WORLD.md gestures toward but does not decide, and that are not currently tracked in `decisions.json`.

### 6.1 Infrastructure gaps

1. **Order communication infrastructure.** L667 says "telegraph and early telephone" is the baseline tech level. Does the Order have telegraph? Or does the Order substitute attunement-based communication at comparable functional scope? The two factions' ability to coordinate across a contested front depends on this and it is currently unspecified.
2. **Rail and long-distance transport in the Order.** L667 names rail as the backbone. Written for both factions or just Coalition? Order territory spans the Order interior, eastern seaboard, northern territories, and SW coastal enclave — some separated by contested corridor. How does movement work?
3. **Currency, trade, and cross-faction economic contact.** Extractive networks (L657) move material between factions. What do they exchange? How does the Order pay the Coalition's shadow economy operators? What is the currency situation — gold, paper, something else? This is adjacent to D014 but deeper than what D014 resolves.

### 6.2 Cultural gaps

4. **Coalition religion / philosophical successor to displaced faith.** Noted in §3 above.
5. **Order education.** How does a non-attuned Order child experience school? How does an attuned child? Both cultures have implied early education (grandmother-rule wisdom, apparatus safety rules) but no institutional education is described.
6. **Art, music, sport, entertainment.** Both factions. The world is at early-industrial-to-inter-war tech; both would have newspapers, theater, sport, developing cinema. None of this is currently present.
7. **Medicine beyond attunement-healing and the iron pathway.** L667 mentions "no antibiotics." What is the Coalition's medical practice like outside apparatus-assisted work? What does the Order do for non-attuned injuries beyond what attunement can reach?

### 6.3 Structural gaps

8. **Order economic non-state actor.** Noted in §3.
9. **Coalition head of state / executive authority.** The three-tier government is described in detail but the actual executive — who is the federal-tier leader, how are they elected, term limits, war-powers authority — is not specified.
10. **Order succession and mortality at senior levels.** Founding families are a shifting coalition (L257). How do family leadership transitions work? When a senior attuned member dies, what happens to that family's standing? The demographics section (L369) touches on lineage transmission but not on power succession.
11. **SW coastal enclave and autonomous zones.** L635 describes the enclave as "effectively autonomous" but does not resolve who speaks for it, who administers it, or how it relates to the Order's formal branches. Similar for the northern territories (L631).

### 6.4 Physics / mechanics edges

12. **Apparatus scale thresholds.** L739–741 describes the installation → vehicle → personal arc. Concrete examples of capability that has / has not reached each scale are mentioned (liquid substrate at prototype, gas theoretical) but not inventoried. If a writer wants to know whether a given capability is vehicle-scale in the current era, there is no checklist.
13. **What does "attuned children playing with degraded apparatus" involve?** L597 names this as the war trigger. The interaction mechanism is called "unknown" — correctly so, for plot reasons — but the broader question of whether attuned non-practitioners can accidentally interact with Coalition apparatus is a physics question with mechanical implications.
14. **Mercury poisoning as narrative element.** Mercury is central to Coalition apparatus (L721, L729). Real-world mercury is a serious industrial poison. The Coalition's occupational-health story around mercury is unaddressed.

---

## 7. Priority recommendations

The INDEX.md priority queue is well-ordered for the decision-level work. This analysis suggests the following to pair with it:

1. **Registry hygiene pass.** Fix the INDEX.md/decisions.json/CLAUDE.md drift documented in §5 before the next decision session. This is ~30 minutes of work and prevents drift from compounding.
2. **In-line `[OPEN: Dxxx]` markers** at the five anchors in §4 (D023, D025, D036, D037, D038). Keeps WORLD.md self-describing without requiring a reader to jump to the bottom.
3. **Before or during D023 (daily life)**, decide the Coalition religion/non-religion posture (§6.2 item 4). It will otherwise force itself into daily life content and be resolved under writing pressure rather than deliberately.
4. **Before character work**, decide the Order non-state economic actor (§6.3 item 8). The current decision queue (D020, D037, D025) covers the Order's institutional branches but not its economic institutions.
5. **D008 title/summary correction** in decisions.json to match its current decided_text (Order-side content). Alternatively, split D008 and D010 cleanly — one for Order founding figures, one for Coalition buried history. Currently they overlap in awkward ways.

---

## 8. Summary

WORLD.md draft 76 is internally consistent at the invariant level, with strong discipline around the Vein's physics and the faction asymmetries. Cross-section consistency is largely intact; the soft tensions in §2.2 are hygiene issues, not contradictions.

The main gaps are (a) parity asymmetry in faction daily life (D023), (b) under-documentation of non-state Order institutions, and (c) metadata drift across the three canonical files. None of these threaten the world's load-bearing structure. All are tractable.

The document is in good shape for the current decision work to continue. The registry hygiene pass in §7 item 1 is the highest-leverage small intervention.
