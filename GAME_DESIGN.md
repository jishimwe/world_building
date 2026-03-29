# GAME_DESIGN.md
*Last updated: session — D031/D032/D033 additions; concern 1 licensed capabilities note; concern 4 Coalition progression principle*
*Companion to WORLD.md (draft 37) and decisions.json*

---

## What this document is for

This document holds concerns, requirements, and open questions that arise specifically from the fact that this world is being built for a game. It is not a design document — it does not specify mechanics, systems, or implementation. It is a filter that sits alongside the worldbuilding work and asks: is what we are deciding gameable? Does it produce the things a game needs?

Where worldbuilding decisions already answer a game concern, this document notes what exists and what is still missing. Where there is a genuine gap, it flags it as a blocker or a priority and notes what worldbuilding decision would address it. Some game concerns will generate new entries in decisions.json. The concern lives here; the decision it spawns lives there.

Read this alongside WORLD.md before any session that touches visual design, progression systems, UX, or moment-to-moment play feel. If a worldbuilding decision is being made that affects any concern listed here, check this document first.

---

## Core principle

The world has to be gameable. Every worldbuilding decision that produces something unrepresentable, unplayable, or unreadable by a player is a problem — not a fatal one, but a problem that needs to be named and resolved. This document is where those problems live so they do not accumulate silently.

---

## Open concerns

---

### 1. Is the Vein system conducive to graphic expression?

**What the concern is:** The Vein needs to produce visuals that are distinctive, readable under pressure, and expressive enough to carry moment-to-moment gameplay feedback. A system that is only legible through text description or close reading will not work.

**What already exists:**
The visual language section of WORLD.md (section: "The Vein — visual language of field manipulation") is substantially developed and game-ready in its current form for the Order side:
- Six color registers with distinct semantic meanings (blue/green/red/purple/white/black) — each maps to a gameplay state
- Intensity as brightness/completeness of glow — maps to a power level readout
- Glow stability (steady vs. flickering/blooming) — maps to a control readout
- The bleed: color propagating from substrate into affected matter proportionally — maps to area-of-effect feedback
- Substrate mirror faces as the color source — a fixed anchor point in the environment

The substrate itself has a strong visual identity: matte black exterior, mirror-flat fracture faces, color living inside the material rather than radiating from it. The distinction between inert substrate (dark rock) and active substrate (interior mirror faces showing color and movement) is visually concrete.

**What is missing:**
- Coalition apparatus visual signature. WORLD.md describes it as "looks like industry" — true but insufficient for a graphics brief. The specific visual signatures of apparatus in operation are not yet defined: conduit heat shimmer, quartz array glow, indicator state visuals (tin color change, mercury surface behavior, glass stress patterns), steam venting. The apparatus needs its own visual language to the same degree the Order manipulation does.
- Field manipulation geometry. The color registers describe *what* is happening but not *what shape it takes in space*. Does a red manipulation have a visible geometry — a cone, a wave, a sphere of influence? Does the bleed have a falloff shape? Does blue suppression visually contract while red overdriving visually expands? None of this is decided.
- Environmental expression without substrate. WORLD.md notes that field manipulation without visible substrate produces "environmental wrongness" — stone cracking without cause, air shimmering with sourceless heat, frost spreading. These are listed as effects but their visual treatment is not specified. How much of this is particle, how much is post-process, how much is geometry deformation?
- Licensed-but-undescribed capabilities. The existing physics already licenses a significant capability set that has not been written out or given visual treatment: fire and freezing (moving matter up and down the energy continuum is the Vein's core operation), concussive force (rapid phase transition produces explosive pressure — water to steam is 1700x volume expansion), healing and biological enhancement (green register working with living tissue), directed vibration (already implied by the quartz transducer mechanism). These capabilities exist in the world. They have no visual language yet, no described expression, no gameplay shape. They need a dedicated pass before visual design work begins — not because they are new decisions but because they are decided facts that haven't been translated into representable form.

**Downstream decisions needed:**
- Field manipulation geometry (shape/volume/falloff of effects in space) — not currently in decisions.json, needs an entry
- Coalition apparatus visual signature — can be added as a subsection to WORLD.md's apparatus section once the visual language question is answered
- Licensed capability visual language — a dedicated pass translating fire/freeze/concussion/healing/vibration into described visual expressions for both factions

**Priority:** High. This should be addressed before any visual design work begins.

---

### 2. How does the Vein color the world — palette and environmental identity?

**What the concern is:** Beyond the active-manipulation color registers, the Vein needs to produce a consistent environmental palette that makes a Vein site look and feel different from everywhere else. A game needs to communicate "you are entering Vein territory" through environmental language, not text.

**What already exists:**
- Substrate's stable appearance: matte black, dense, slightly wrong weight, mirror-flat fracture faces. A visual anchor that is distinctive and consistent.
- Vein sites as hyper-alive ecologies: larger growth, more intense color, unusual animals, ambient field energy feeding everything. This implies a palette direction — saturated, intense, slightly wrong — but does not specify it.
- The six manipulation color registers (blue through black) are available as environmental color keys if Vein sites bleed the field's color register into their ambient palette.
- Vein-adjacent minerals: high-energy crystalline phases that are visually unusual by definition — phases that don't exist in ordinary geology, which means unusual refraction, unusual surface properties, unusual color.
- Phosphorus glow as the first observable signal: cold light at night, no combustion, concentrated near Vein sites. This is already an environmental visual with a specific quality (cold, blue-white, sourceless).

**What is missing:**
- The ambient color palette of an active Vein site during normal (non-combat, non-manipulation) operation has not been decided. Is the substrate's black the dominant tone, with color emerging from it? Is the site visually neutral until manipulation begins? Does the ecology's hyperactivity produce a specific palette — more saturated greens, unusual animal coloration?
- The contrast between rich sites and depleted sites has narrative weight (depletion is visible) but no specific visual treatment. What does a worked-out site look like compared to an untouched one?
- Day/night visual distinction. Phosphorus glow is a night signal. What does a Vein site look like at night vs. day?

**Downstream decisions needed:**
- Ambient site palette and environmental color identity — generates a worldbuilding decision about how the field expresses visually at low concentration (below manipulation threshold)
- Depletion visual treatment — ties to existing WORLD.md content on depleted substrate (mirror faces going dark and still) but needs expansion to the site level

**Priority:** Medium. Needed before environment art direction is locked, not before systems work.

---

### 3. How do we create kinetic dynamism?

**What the concern is:** The Vein system as described is physically consequential but relatively slow — it operates through material state changes, thermal effects, and biological processes. A game needs moment-to-moment kinetic energy: things that move, pulse, react, and feel alive in real time. This concern is about whether the system as designed can produce that, and what needs to be added or emphasized to make it work.

**What already exists:**
- The bleed propagates outward from substrate as intensity increases — this is inherently dynamic, a spreading effect
- Glow stability (flickering, blooming) implies animation — the glow is not static
- Phase transitions are inherently dramatic: liquid substrate appearing while the contact end remains solid, stone spalling, steam expansion at 1700x volume
- The cascade principle (WORLD.md: "a practitioner does not do a thing to one material and stop there") implies chain reactions — kinetic consequences propagating through an environment
- Loss-of-control events (flickering/blooming glow, excess propagating unpredictably) imply dynamic escalation
- Coalition apparatus failure cascade: designed failure points going in sequence — lead fuses transitioning, glass cracking, bronze damping stages saturating — is an inherently dynamic sequence

**What is missing:**
- The feel of field manipulation in motion has not been described. Does pushing field energy through a metal conduit produce visible propagation — a wave of heat moving down the conduit, visible to an observer? Or does it express only at the terminus?
- The temporal character of Order manipulation has not been specified for gameplay purposes. Is green healing a pulse, a sustained glow, a spreading wave from contact point? Is red damage instantaneous or does it build? Does blue suppression visually contract the affected area?
- Environmental reactivity to field presence. WORLD.md describes ecology adapting over geological time. What does an environment do in real time near active manipulation — do plants respond, do animals flee, does the air change? This is kinetic texture, not just background.
- The quartz transducer array vibrating at audible frequency during high-intensity operation is a dynamic physical event — this is mentioned as a sound but its visual expression is not described.

**Downstream decisions needed:**
- Temporal character of manipulation (pulse vs. sustained vs. wave) — needs a decision, currently undecided
- Environmental real-time reactivity — needs a decision; ties to existing ecology content but needs a real-time layer
- Propagation visibility through metal conduits — ties to D029 (metal conduction) but the visual expression of that propagation is not specified

**Priority:** High. Kinetic dynamism is a core gameplay feel question. Should be addressed before combat and ability design begins.

---

### 4. Gear setup and progression — Order and Coalition

**What the concern is:** A game needs progression systems. Both factions need equipment, tools, and upgrade paths that are grounded in the world's logic and produce meaningful player choices. This concern is about whether the worldbuilding provides enough foundation to build those systems on.

**What already exists:**
*Order side:*
- Mastery hierarchy is well-defined: novice → experienced → master, differentiated by attunement granularity (precision and control, not raw power). This maps cleanly onto an ability progression model.
- Color register access could map to progression: novice accesses green and red, master accesses purple, extreme practitioners reach white or black. Gate registers behind progression.
- The damage model (neurological + structural antenna damage as two independent tracks) provides a character health/condition system with meaningful differentiation.
- Overexposure as a resource/risk system: exposure load, attunement fatigue, the three-variable interaction (intensity × duration × current state). This is a ready-made stamina/overload system.

*Coalition side:*
- Operator expertise levels (novice/experienced/master) map to a progression model with the same structure as Order mastery but through a completely different mechanism (indicator literacy vs. attunement depth).
- Apparatus component quality (iron vs. steel vs. copper vs. silver) provides a natural equipment tier progression — better metals mean better performance and different failure characteristics.
- Lead fuse quality, quartz array precision, Vein-phase lining quality — all of these are component variables that could drive equipment differentiation.
- The two apparatus configurations (boiler vs. forge) provide a playstyle fork within the Coalition progression.

**What is missing:**
- Personal portable equipment for Order practitioners is not described. What does a practitioner carry? What physical objects, if any, mediate their field use? The attunement is biological, but do they carry substrate? Instruments? Protective gear? The gear layer for Order practitioners is completely open.
- Personal portable equipment for Coalition operators is partially implied (operators carry spare lead fuses as standard kit, replacement seals) but not systematized. What does a Coalition field operative carry vs. a site operator?
- The relationship between individual Coalition operators and the large fixed apparatus is not resolved for gameplay purposes. Can a player carry a portable version of the apparatus? Is Coalition gameplay necessarily site-based? If field operatives exist (the liberation war implies they do), what do they use away from fixed extraction infrastructure?
- Progression pacing — what does early-game vs. late-game look like for each faction? What is being unlocked and when?
- Cross-faction gear interaction — can Order practitioners interface with Coalition apparatus? Can Coalition operators exploit Order practitioners' biological vulnerabilities in a systematic way?

**Coalition progression principle (D033).** Coalition capabilities follow the infrastructure → vehicle → personal arc. This has direct implications for how Coalition progression is structured: the most powerful Coalition capabilities are always installation-scale, and personal-scale versions are always the least powerful instance. A Coalition player's progression arc is therefore partly about gaining access to larger and more powerful installations, not just improving personal gear. The personal kit is the starting point; the installation is the endgame. This inverts the typical game progression model (personal → powerful personal) and needs to be designed around deliberately. The Order's progression is the inverse — always personal, always embodied, the endgame is a more capable individual not a larger machine.

**Downstream decisions needed:**
- Order personal equipment layer — what practitioners carry, whether substrate is portable in any form, whether instruments are standard kit
- Coalition portable apparatus — what field operatives use away from fixed sites; this is partially a D015 downstream question (refined substrate — D005 — may be relevant here)
- Progression structure for both factions — this is a game design decision more than a worldbuilding one, but it needs worldbuilding foundations before it can be made

**Priority:** High for planning; medium for immediate session work. The foundations exist. The gear layer needs a dedicated session once D005 (refined substrate) is answered.

---

### 5. When should names and appearances be fixed?

**What the concern is:** A game needs finalized names and visual identities before certain production milestones. This concern is about which open naming decisions are blocking production work and when they need to close.

**What already exists:**
- Substrate appearance is fully described (WORLD.md: stable state, active state, depleted state). No decision needed.
- Color register names (blue/green/red/purple/white/black) are working labels that may or may not become final names — they are functional and specific.
- Faction placeholder names (Attuned Order, Forge Coalition) are in use across all documents. D009 in decisions.json flags these as low priority pending cultural development.
- Resource placeholder name (the Vein) is in use. D001 in decisions.json flags this as low priority.
- Attunement has no alternative name being considered.

**What is missing:**
- No visual identity work has been done for either faction at the institutional level — symbols, flags, uniforms, architecture aesthetic, insignia. This is downstream of cultural development that has not happened yet.
- The substrate's active-state visual is described in words but has not been translated into a visual reference. The mirror-face color expression, the bleed, the glow stability system — all described precisely enough to brief an artist, but not yet briefed.
- Character visual archetypes for Order practitioners and Coalition operators are not established. What do they look like? What do they wear? What distinguishes a senior Order practitioner from a junior one visually? What distinguishes a master Coalition operator from a novice?

**Decision dependencies:**
- D001 (Vein name): low priority, not blocking production work yet
- D009 (faction names): low priority, not blocking production work yet
- Visual identity work is blocked on cultural development sessions that have not happened
- Character archetype work is blocked on character development sessions that have not happened

**Recommendation:** Names can stay as placeholders until cultural development sessions happen. The substrate visual and the manipulation visual language are ready to brief now — these do not depend on names. Faction visual identity and character archetypes should be flagged as requirements for the first cultural development session.

**Priority:** Low for names; medium for visual briefing of substrate and manipulation language; high as a pre-production milestone tracker.

---

## Session flags

Things to check at the start of any session that touches the concerns above:

- Before visual design work: concerns 1, 2, 3 must be addressed
- Before combat/ability design: concerns 1, 3, 4 must be addressed
- Before equipment/progression design: concern 4 must be addressed, D005 (refined substrate) should be answered first
- Before pre-production art direction: concerns 1, 2, 5 must be addressed
- Before naming/branding lock: concern 5, D001, D009 must be decided

---

## Decisions spawned by this document

The following decisions.json entries were identified as needed based on concerns in this document. They do not yet exist in decisions.json and should be added when the relevant session begins:

- **Field manipulation geometry** — shape, volume, and falloff of effects in space for Order manipulation. Required before visual design. Blocks concern 1.
- **Temporal character of manipulation** — pulse vs. sustained vs. wave for each color register. Required before ability design. Blocks concern 3.
- **Environmental real-time reactivity** — what an environment does in real time near active field manipulation. Blocks concern 3.
- **Propagation visibility through metal conduits** — does field conduction through apparatus produce visible propagation or only terminus expression? Blocks concern 3.
- **Coalition apparatus visual signature** — the specific visual language of apparatus in operation. Blocks concern 1.
- **Order personal equipment layer** — what practitioners carry; portable substrate question; instrument standard kit. Blocks concern 4.
- **Coalition portable apparatus** — what field operatives use away from fixed sites. Downstream of D005. Blocks concern 4.

---

*Connected documents: WORLD.md · decisions.json · FACTIONS.md (when created) · CHARACTERS.md (when created)*
