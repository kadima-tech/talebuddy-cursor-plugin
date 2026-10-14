# Talebuddy plugin

Connects Grok Bot and Cursor to [Talebuddy](https://talebuddy.io), so your agent can help you plan and write stories: find tales, build concept pages, keep the story ledger (characters, places, lore) current, read your manuscript, and file session notes.

## What's included
- **MCP server**: Talebuddy's hosted server at `https://talebuddy.io/api/mcp`. Nothing runs locally.
- **Skill**: `talebuddy-writing-session`, which guides the agent to read before writing and to confirm before overwriting or deleting anything.

## Setup
Install the plugin, then sign in with your Talebuddy account when prompted (OAuth). No API key needed. Cloud tales require a paid Talebuddy plan.

## Tools
Read-only: `list_tales`, `search_tales`, `get_tale`, `list_ledger_entries`, `get_ledger_entry`, `get_manuscript`.
Additive: `create_tale`, `create_concept_page`, `attach_to_concept_page`, `file_session_notes`.
Can overwrite or delete: `update_tale`, `write_concept_page`, `create_ledger_entries`, `update_ledger_entry`, `delete_ledger_entry`, `delete_tale`.

## Links
- [Privacy policy](https://talebuddy.io/privacy)
- [Talebuddy](https://talebuddy.io)
