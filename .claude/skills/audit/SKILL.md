# Consistency Audit

Audits INDEX.md, WORLD.md, and decisions.json for sync issues, then fixes all problems found.

## Steps

1. **Read INDEX.md, WORLD.md header, and decisions.json** — gather current draft number, decision counts, and all decision IDs with their statuses.

2. **Verify decision IDs** — check that every ID in INDEX.md's decided/open/in-progress tables exists in decisions.json with the matching status. Flag any ID that is:
   - In INDEX but missing from decisions.json
   - In decisions.json but missing from INDEX
   - Present in both but with mismatched status

3. **Check counts and draft numbers** — verify:
   - INDEX.md header "N of M decisions decided" (M = total entries in decisions.json) matches the actual decided count in decisions.json
   - INDEX.md `### Decided (N)` count matches the decided table row count
   - INDEX.md header draft number matches WORLD.md's draft number
   - decisions.json `meta.doc_version` matches WORLD.md's draft number

4. **Check section map** — for each decided entry with a non-null `world_md_line`, confirm the referenced line in WORLD.md is plausibly related. Flag nulls on decided entries that should have been written in.

5. **Flag stale, duplicate, or missing entries** — report all issues before making any changes.

6. **Fix all issues** — edit INDEX.md and decisions.json to resolve every flagged problem. Verify decisions.json parses after editing.

7. **Show a summary** — list each issue found and how it was resolved. If any issues require user judgment (e.g. a decision written into WORLD.md but world_md_line is still null), flag them separately rather than guessing.
