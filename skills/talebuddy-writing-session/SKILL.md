---
name: talebuddy-writing-session
description: Work on a story in Talebuddy. Use when the user wants to brainstorm, develop characters, places or lore, update a tale's concept pages or ledger, check their manuscript, or wrap up a writing session with notes.
---

# Talebuddy writing session

## Start by finding the tale
- Use `list_tales` or `search_tales` to find the tale the user means, then `get_tale` for its details. Ask only if several tales plausibly match.

## Read before you write
- Check the ledger with `list_ledger_entries` / `get_ledger_entry` before adding characters, places or lore, so you don't create duplicates.
- Use `get_manuscript` to check what's already written. The manuscript is read-only through these tools.

## Making changes
- Prefer additive tools: `create_concept_page`, `attach_to_concept_page`, `create_ledger_entries`, `file_session_notes`.
- These tools can overwrite or delete the author's work, so confirm with the user before calling them: `update_tale`, `write_concept_page` in replace mode, `create_ledger_entries` with `onDuplicateName=merge`, `update_ledger_entry`, `delete_ledger_entry`, `delete_tale`.

## Wrapping up
- At the end of a session, offer to record what was decided with `file_session_notes`.

Cloud tales need a paid Talebuddy plan; if a tool reports that, tell the user rather than retrying.
