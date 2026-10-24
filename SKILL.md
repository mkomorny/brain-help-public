---
name: brain-help
description: >-
  Prints the complete Second Brain slash command cheat sheet directly in chat.
  Use when the user types /brain-help or wants to see all available brain commands,
  their syntax, flags, and examples. Executes immediately with no approval needed.
---

# Brain Help — Command Cheat Sheet (`/brain-help`)

Execute **immediately**. Print the full command reference table in chat. No MCP tool needed.

---

## 🧠 Second Brain — Slash Command Cheat Sheet

### Core Memory Operations

| Command | Type | Action & Behavior |
| :--- | :--- | :--- |
| `/brain-recall <query>` | Read | Semantic search. Flags: `--hops <0-2>`, `--tag <tag>`, `--kind <semantic\|episodic>`, `--topK <N>` |
| `/brain-get <id>` | Read | Retrieves full untruncated content of a memory by ID |
| `/brain-recent [limit]` | Read | Lists most recent memories (default 5, max 20) |
| `/brain-connections <id>` | Read | Shows all memories linked to a given ID in the knowledge graph |
| `/brain-sync [topic]` | Read | Conversation-opening briefing: tasks, decisions, preferences for a topic |
| `/brain-conversation-transcript` | **Write** | **Archives full procedural dialog & transcript** of current session |
| `/brain-summarize-conversation` | **Write** | **Writes structured executive brief** of current conversation |
| `/brain-save <text>` | **Write** | Directly saves new memory (`#tags`, `!durable\|!state\|!volatile`) |
| `/brain-append <id> <text>` | **Write** | Directly appends dated note to existing memory |
| `/brain-update <id> <new>` | **Write** | Directly replaces existing memory content |
| `/brain-help` | Help | Prints this cheat sheet |

### Advanced Session & Knowledge Workflows

| Command | Type | Action & Behavior |
| :--- | :--- | :--- |
| `/brain-harvest` | Audit | Audits session files & git diff, checks Second Brain coverage, reports unrecorded gaps |
| `/brain-checkpoint` | Handoff | End-of-session 3-part debrief (Accomplished, Decisions, Next Steps) + auto-sync to project memory |
| `/brain-tasks` | Miner | Extracts TODOs, FIXMEs, edge cases, and verbal commitments into a deduplicated task list |
| `/brain-decisions` | ADR | Mines architectural choices & trade-offs ("Why") into durable Architecture Decision Records |
| `/brain-drift` | Guard | Checks if codebase violates brain rules, or if old memories have become obsolete |
| `/brain-link-suggest` | Graph | Discovers unlinked memories across projects sharing tools/techniques and suggests graph edges |
| `/brain-hygiene <topic>` | Cleanup | Audits a topic for duplicate memories, stale drafts, and recommends merges/deprecations |

### Volatility Flags

| Flag | Meaning | Best For |
| :--- | :--- | :--- |
| `!durable` | Permanent, immutable | Architectural choices, core constraints, hardware specs, key preferences |
| `!state` | Evolving (default) | Current project status, active tasks, sprint notes |
| `!volatile` | Temporary, ephemeral | Single-session reminders, scratch notes |

### Common Examples

```
/brain-harvest
/brain-checkpoint Live Actions
/brain-tasks
/brain-decisions
/brain-drift Live Actions
/brain-link-suggest
/brain-hygiene Live Actions
/brain-recall audio dropouts --hops 1
/brain-save Enabled reuseAddress on UDP socket #live-actions #osc !durable
/brain-append mem_8f93a1 Verified on Ableton Live 12.1
```
