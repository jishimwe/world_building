# WORLDBUILDING_RULES.md
*Reference checklist — run against decisions and new content before writing.*

---

## The Vein as a power system

**Law 1 — Comprehension before resolution**
A Vein capability can only resolve conflict if its mechanics are already established in WORLD.md. New capabilities introduced to solve a plot problem are a failure mode. If a scene requires something the Vein can do that isn't yet documented, the decision must be made first, then the scene written.

**Law 2 — Limitations over powers**
Every new Vein capability requires a cost, ceiling, or failure mode before it is written in. What the Vein *cannot* do is more load-bearing than what it can. When adding capabilities, ask: what does this break if it works too well? Establish that first.

**Law 3 — Expand before adding**
Do not introduce new Vein phenomena until existing ones are fully developed at both factions. Exotic states (D006), gas-phase interaction (D036), and wildlife attunement (D007) are all expansions of established mechanics — they wait until the established layer is complete enough to anchor them.

**Corollary — asymmetry must be permanent**
The Order-excels-at-human-scale / Coalition-excels-at-installation-scale asymmetry is a key invariant. Any new capability that collapses this asymmetry — making one side redundant at all scales — contradicts the permanent-conflict premise. Flag it immediately.

---

## Faction parity checklist

Run this after adding significant content to either faction. Both sides should stay at comparable depth.

- [ ] **Institutional depth** — does each faction have equivalent development at the same institutional layer? (political structure, military, covert operations, religious/research arm)
- [ ] **Internal contradiction** — does each faction have a tension that could tear it apart from inside, independent of the war?
- [ ] **Legibility from inside** — can a true believer on each side articulate why their faction is right, in terms that don't require them to be stupid or evil?
- [ ] **Blind spot** — does each faction have something it systematically cannot see, for structural reasons rather than stupidity?
- [ ] **Cost** — does each faction pay a real price for the way it is organized? Power structures without costs are not believable.
- [ ] **Mirror check** — if one faction just gained a capability or detail, does the other need an equivalent? (Not identical — equivalent in narrative weight.)

---

## Narrative utility test

Before finalizing any worldbuilding element, ask:

**Can this element generate at least two distinct scene types?**

If an element can only do one thing in a story it is set dressing, not worldbuilding. Two scene types minimum means the element has structural load — it can create conflict, complicate relationships, or reframe earlier events in more than one way.

Examples of elements that pass:
- The industry giants' archive asymmetry: scenes where giants know researchers are close before the researchers do; scenes where a researcher realizes their "discovery" is in a private archive
- The operative's self-understanding as protector: scenes of infiltration; scenes of genuine moral crisis when the protection causes harm

If an element only generates one scene type, either develop it until it generates two or defer it.

---

## Common failure modes — check before writing

**The convenient capability**
A Vein property that appears exactly when the plot needs it and nowhere else. If a capability is real, it has always been real — it has economic, military, and social implications that predate the story. Ask: what would the world look like if this has been true for fifty years?

**The legible villain**
A faction, institution, or individual whose position only makes sense from outside. Everyone operates from inside their own logic. The founding families, the industry giants, the Order's institutional ceiling — all of these must be coherent to people who believe in them. If the only way to explain a position is "they're wrong," the position needs more development.

**The asymmetric wound**
One faction has specific, legible moral failures; the other has abstract ones. Both sides need concrete atrocities that their own members rationalize, not just the side that is meant to seem more ambiguous. (D022 is open for this reason.)

**The solved problem**
A worldbuilding decision that removes tension rather than creating it. The Vein's depletion crisis works because nobody in power knows it's happening — if the right people knew, the war would restructure immediately. Decisions that give powerful actors accurate information about threats to their power tend to resolve tension rather than sustain it.

**The single-purpose element**
An institution, technology, or relationship that exists only to serve one story function. Real systems are overdetermined — they exist for multiple reasons and produce multiple effects. The industry giants work because they are simultaneously the Coalition's most reliable financial supporters and its most consistent internal saboteurs. Single-purpose elements feel invented.

---

## Decision quality checks

Before marking a decision as decided:

- Is it consistent with all key invariants in [[CLAUDE]]?
- Does it generate content for both factions, or does it need a parity check?
- Does it produce at least one new open question that should be registered in decisions.json?
- If it affects an existing WORLD.md section, is that section flagged for update?
- Are all decisions it unblocks still correctly marked as open (not waiting on this anymore)?
