# Resolve Decision

Resolves a numbered decision (e.g. D013) in this worldbuilding project.

## Steps

1. **Read decisions.json** — find the specified decision. Check its `status`, `depends_on`, and `blocks` fields before proceeding. If any `depends_on` entries are not yet decided, flag this and stop.

2. **Read relevant WORLD.md sections** — use `world_md_line` if set, otherwise search for related content. Understand what is already canonical before drafting anything new.

3. **Get the resolution** — if the user provided it, use it. If not, present a diagnostic: what the decision requires, what the options are, what each implies for downstream decisions in `blocks`. Ask the user to decide before writing.

4. **Write canonical content into WORLD.md** — analytical register, not narrative. Increment the draft number in the document header. Add a new section if needed; update an existing one if the decision extends something already there.

5. **Update decisions.json** — set `status` to `decided`, write the resolution into `decided_text`, set `world_md_line` to the correct line number. Remove `session_notes` if present. Clear any `refactor_flags` if the write-in addressed them. Verify the file parses after editing.

6. **Update INDEX.md** — update the draft number references, section map if a new section was added, and move the decision from its current table to the Decided table (update the count).

7. **Commit** — use the draft number in the commit message (e.g. `draft 54 — D013 geography decided`).

8. **Show a summary** — which files changed, what was written, what decisions in `blocks` are now unblocked.

## Schema reminder

```json
{
  "id": "D0XX",
  "title": "...",
  "status": "decided",
  "category": "...",
  "priority": "...",
  "world_md_line": 123,
  "summary": "...",
  "decided_text": "The full resolution...",
  "depends_on": [],
  "blocks": []
}
```
