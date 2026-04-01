# WORLD.md Consistency Audit — 2026-03-31
*Revised with cross-document checks, demographic arithmetic, and omission scan*

---

## Critical (genuine contradictions)

**1. Secret society recruitment vs. family concealment** (L261) -> ✅
High-born individuals with incapacity are described as "worth concealing for the family's sake" — but they're also described as being quietly recruited into secret societies. Secret societies operate under institutional surveillance and families use them to monitor rival branches. How can families simultaneously conceal a member's incapacity AND allow that member to participate in a surveilled institution? The mechanism is absent.
*Resolution: placement in the societies is the concealment mechanism. Membership requires no public attunement demonstration; a role in "sensitive institutional work" provides cover. Clarified in WORLD.md draft 62.*

**2. Exposure model incompleteness** (L205–207) -> ✅
Three variables are cited for attuned exposure risk (intensity, duration, current state). But the same section establishes two separate damage pathways (water/thermal vs. iron/hemoglobin) that scale differently with intensity and "do not respond to the same countermeasures." The pathway a practitioner is managing is effectively a fourth variable — or the three-variable model is a simplification that the text itself contradicts two paragraphs earlier.
*Resolution: three variables govern total load (practitioner's field model); two pathways govern damage character (healer's clinical model). Bridging sentence added at end of L207 in draft 62.*

---

## Cross-document sync issues

**3. Stale [OPEN] marker — substrate recovery** (L65) -> ✅
L65 reads: "Whether anyone has kept records long enough to observe it, and what they have done with that knowledge, is [OPEN: story structure decision]." D004 decided this: substrate recovery is real but unobserved, Order death doctrine encodes it as metaphysics. The death doctrine content IS written into WORLD.md (L343, L431, L487). The [OPEN] marker at L65 should be replaced with the decided answer.

**4. Stale [OPEN] marker — ceasefire collapse trigger** (L527) ->  ✅
L527 reads: "triggered by [OPEN: a specific event to be decided during story structure work]." D011 decided this and the content is written at L537 (five children, apparatus accident). The [OPEN] at L527 should be replaced with a forward reference to the trigger passage.

**5. Stale demographic reference in contact prohibition** (L447) -> ✅
L447 says the prohibition's feasibility "depends on what fraction of the Order's population is non-attuned — a demographic question not yet resolved." D035 resolved this: 70/30 attuned/non-attuned. At 30% non-attuned (a minority), the prohibition is enforceable per the text's own logic. The "not yet resolved" clause is stale.

**6. INDEX.md file table says Draft 59** (INDEX L10) -> ✅
INDEX.md files table shows WORLD.md at "Draft 59" but WORLD.md header says draft 60. The section map at L34 correctly says draft 60, so it's just the files table that's stale.

**7. [REVISIT] marker — tech timeline** (L595) *(not stale — intentional)*
L595 reads: "[REVISIT: tech timeline and gap visibility to be developed further as world takes shape.]" D017's decided_text explicitly flags all three parts for eventual revision. The marker is correct as placed.

**8. decisions.json meta.doc_version says "draft 50"** -> ✅
The `meta.doc_version` field in decisions.json still reads "draft 50". WORLD.md is at draft 60. This is cosmetic but creates a false impression of staleness.

**9. refinement_axis.md references "D005 open"** (refinement_axis L51) -> ✅
Working document still flags D005 as open. D005 has been decided. Stale annotation.

---

## Major ambiguities (gaps in causal logic)

**10. Extraction intensity vs. barrier erosion timeline** (L19, L523) -> ✅
Coalition extraction depletes field concentration; the biological barrier is tied to field concentration. But the timeline of "when did extraction get intensive enough to start eroding the barrier" is never established. The Order observes erosion without understanding it (L26–27), but the causal chain requires a timeframe.
*Resolution: L19 qualified — "far faster" claim now applies specifically to industrial-scale extraction; incidental handling and small-scale experimentation produce no observable concentration change. Consistent with L531 (industrial extraction post-partition). Draft 63.*

**11. Coalition 5% attunement — composition and detectability** (L235, L329) -> ✅
The 5% figure is cited as demographic fact, but the Coalition has no Order-equivalent mechanism for systematic identification. The figure likely excludes undiscovered individuals. More significantly, the text presents emergence and defector ancestry as two co-equal sources, but the arithmetic shows defectors dominate:
- If ~10% of pre-liberation attuned defected, the Coalition's founding attuned fraction was already ~5%
- 1% emergence per generation adds only ~0.2-0.4% per generation to the cumulative fraction
- After 3–4 generations, emergence accounts for roughly 0.6–1.2% of the total, not half
The text's "traces to two sources" framing implies more balance between sources than the math supports.
*Resolution: 5% is world ground truth (authorial layer), not a Coalition census — the Coalition's inability to measure it is already established at L235/L239. Added sentence at L329 clarifying defector lineages dominate numerically; emergence is the rising mechanism, not the dominant source. Draft 64.*

**12. Quartz transduction mechanism** (L173, apparatus section) -> ✅
Quartz is established as the only bidirectional transducer — it can both receive and emit shaped field behavior. How a passive mineral produces directional/shaped output rather than isotropic scatter is the core of Coalition apparatus function and is never mechanistically explained. This may be acceptable as a physics-of-the-world primitive, but if so, it should be flagged as one rather than left as an implicit gap.
*Resolution: crystal axis anisotropy added at L173 — reverse transduction follows the crystal's natural axis, not isotropic scatter. Geological quartz with random orientations produces incoherent noise; apparatus quartz requires controlled element orientation during construction, making it a precision craft. Draft 65.*

---

## Precision issues (underspecified claims)

**13. "Full concentration range" for attunement** (L197) -> ✅
Attunement is described as sensitivity "across its full concentration range." But the biological barrier and desensitization mechanics establish practitioners have an effective operational ceiling. "Full" overstates.
*Resolution: rewritten to "from field-faint concentrations far below Coalition instrument thresholds up through the dangerous intensities that mark the biological barrier." Draft 62.*

**14. Emergence rate timing** (L229–231) -> ✅
Rate has been "climbing across centuries" from "negligible" to ~1%. The transition curve is absent. This matters for Coalition attuned demographics: if the rate was near-zero at liberation, the 5% is almost entirely defector-seeded; if it was already 0.5%, emergence is a significant contributor.
*Resolution: anchor added at L231 — rate was well below current level at liberation, defector lineages substantially outnumbered emergence contribution at founding; post-liberation climb has been steeper, driven by compounding Vein-proximity biological effects. No precise curve needed unless future arithmetic requires it. Draft 66.*

**15. Genealogical rewriting scale** (L225–226, L327) -> ✅
The 70–80% transmission rate produces a 20–30% failure rate. At scale, that's a 1-in-3 to 1-in-5 failure rate — statistically obvious. The text acknowledges "absorbing failures" but undersells how industrialized the rewriting process would need to be. The concealment mechanism needs more weight.
*Resolution: class stratification added. L225 clarified that genealogical rewriting applied to families whose position depended on the hereditary claim. L327 extended to distinguish elite response (institutional cover: re-attribution, placement, record adjustment) from ordinary Order response (social shame, no machinery). The concealment apparatus is targeted, not universal. Shame handles the rest. Draft 67.*

**16. Desensitization vs. demographic inversion** (L211, L321) -> ✅
Biological desensitization ("across generations") and demographic inversion (liberation departure) are two separate mechanisms on different timescales, discussed in proximity in ways that risk conflation.
*Resolution: parenthetical added at L323 explicitly distinguishing the two mechanisms. Draft 62.*

**17. Order demographics inversion — math implicit** (L321–326) -> ✅
The 30/70→70/30 inversion via selective retention is plausible. Running the constraint: for every attuned person who stayed, only ~18% as many non-attuned stayed (relative to base population). This works if 80–87% of non-attuned left and 0–30% of attuned left — consistent with a mass non-attuned departure. The text should either state the departure composition or acknowledge the inversion as approximate.
*Resolution: sentence added at L323 stating ~80%+ of non-attuned departed while most attuned stayed. Draft 62.*

---

## Structural observations

**18. Parallel three-institution conflict** (L443, L451) -> ✅
Both factions exhibit identical three-institution conflict dynamics when handling prisoners. The structural parallel is never acknowledged. The causes do differ (Order: ideological; Coalition: jurisdictional), but the structural rhyme is worth naming.
*Resolution: sentence added after L461 naming what the rhyme reveals — identical coordination failure from different institutional logics; Order conflict is ideological, Coalition conflict is jurisdictional. Draft 69.*

**19. Contact prohibition is not contradictory** *(downgraded from original audit)* -> ✅ no action needed
L447 establishes the prohibition targets non-attuned specifically. L475 confirms attuned are "not subject to the contact prohibition in the same protective register." These are consistent. The original audit flagged this as a contradiction; it is not.

**20. Minor terminology drift — attunement/sensitivity/coupling** (L21, L197, L199, L201) -> ✅
"Sensitivity" is used both for the attunement trait itself (L197: "biological sensitivity") and for the reactive property that causes harm (L21: "overexposure sensitivity"). "Coupling" refers specifically to neurological structures (L199) but "attunement sense" (L201) is used for the trained perception. Context disambiguates in every case, but a reader encountering these terms cold could confuse the trait with the vulnerability. Not a contradiction — a tightening opportunity.
*Resolution: L197 changed from "biological sensitivity" to "biological sense" — consistent with "This is a sense" two sentences later. Frees "sensitivity" to carry only the vulnerability meaning. Draft 70.*

---

## Omission detection (logical entailments not addressed)

**21. Order response to barrier erosion** -> ✅
If the biological barrier is weakening due to Coalition extraction (L19, L203), the Order's military and territorial doctrine should be adapting — or visibly failing to adapt. WORLD.md describes the depletion blindness (L26–27) but never addresses whether frontier practitioners have noticed increased survivability in previously hostile territory, or whether tactical doctrine has changed. The absence is conspicuous.
*Resolution: paragraph added after L271. Practitioners directly and accurately perceive reduced field concentration in the current war — attunement gives them that. What they lack is the causal framework: the Order has no concept of extraction depleting field concentration over time, so the change is attributed to natural variation or Coalition disturbance. The Order gains ground it can perceive but cannot explain, and therefore cannot reason about trajectory. Draft 71.*

**22. Coalition extraction paradox — self-undermining defense** -> ✅
The Coalition's continued extraction makes its own core territory less defensible against Order operations (L22–24, L525). The text identifies this dynamic but never addresses whether any Coalition institution has recognized it. Are there military voices arguing for extraction slowdowns to maintain the barrier? Industrial voices insisting extraction is non-negotiable? This is the Coalition's most dangerous strategic blind spot and the text leaves it entirely unaddressed.
*Resolution: paragraph added at Coalition political landscape section. The blind spot is total — the military reads Order expansion as aggression (not changed conditions), extraction engineers read yield decline as logistics, and the synthesis connecting the two requires cross-domain vocabulary no institution possesses. The strategic variable is invisible as a strategic variable; being set by economic logic alone. Established as starting condition — can be pierced through story. Draft 68.*

**23. Order response to Coalition-territory emergence** -> ✅
Spontaneous emergence at 1% applies to all populations. If it's happening in Coalition territory (L235), it's also happening in contested and Order-adjacent populations. Does the Order know? Do they care? The text covers Coalition's response (geographic marginalization) but is silent on whether the Order monitors, recruits from, or ignores emergence outside its borders.
*Resolution: paragraph added before the Coalition administrative records passage. Order observes attuned Coalition citizens through military/intelligence contact; bloodline framework explains them automatically as hidden ancestry. Emergence-as-phenomenon invisible to the Order. Institutional response fragmented (military: assets; religious arm: persecuted; secret societies: capability) but not systematic. Draft 72.*

**24. Secret society reconstruction of founding catastrophe** -> ✅
The founding catastrophe is mythologized beyond recognition (L93–97). The secret societies preserve exotic state knowledge and operate outside institutional constraints. Has anyone in the societies attempted to reconstruct what actually happened? The text describes their capability and motivation but never addresses whether they've used it on this specific question.
*Resolution: paragraph added after L99. Recent incidents are tractable; founding event harder (too old, too mythologized, documentation in religious arm archives which some societies have tried to access). Reconstruction is a live project — societies hold more accurate account than the institution, probably sufficient to identify the class of event, not sufficient for certainty, and not written where the institution can find it. Draft 73.*

**25. Coalition counterparts at comparable depth**
The Order has: founding families, religious arm, military, secret societies — all described at institutional depth. The Coalition has: elected government, constitutional court, political tensions — described structurally but with less institutional texture. The military, scientific, and industrial institutions appear in the interrogation section (L451–457) but don't have standalone descriptions of their internal politics, recruitment, or failure modes. The industry giants get one paragraph (L315–316) where Order secret societies get multiple detailed sections. Parity gap.

---

## What held up cleanly

- All 12 CLAUDE.md key invariants are consistently applied throughout
- Dense substrate / diffuse field distinction is never collapsed
- The Vein's energy-moving (not generating) character is consistent
- Coalition extraction → barrier erosion causal chain is sound in direction
- Liberation war outcome ("escaped and held") is consistently framed
- Order's two-layer institutional blindness (reporting incentives + catastrophe complacency) is coherent
- Death doctrine content (D004) is well-integrated across multiple sections (L343, L431, L487)
- War trigger content (D011) is detailed and consistent with faction characterization (L537–539)
- Wartime folk culture distortion section (L481–502) — every claim checked against earlier institutional and political sections; all consistent
- MATERIALS_BASELINE and WORLD.md are aligned on substrate properties, grade names, and four-axis model — no material contradictions
- Core terminology ("substrate," "field," "attunement," "depletion") is stable across all 60 drafts
- All [OPEN] markers in WORLD.md have corresponding decisions in decisions.json — no orphaned markers

---

## Priority actions

1. **Fix stale markers** (#3, #4, #5, #6, #8, #9) — done
2. **Resolve #1** (secret society recruitment logic) — done (draft 62)
3. **Resolve #2** (exposure model variable count) — done (draft 62)
4. **Resolve #13** ("full concentration range") — done (draft 62)
5. **Resolve #16, #17** (desensitization/inversion separation, departure math) — done (draft 62)
6. **Address #10** (extraction/barrier timeline) — done (draft 63)
7. **Sharpen #11** (5% composition) — done (draft 64)
8. **Address #22** (Coalition extraction paradox) — needs decision: most critical strategic omission
