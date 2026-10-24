# Brain Help

> **Tri-Platform Agent Skill** for Claude Desktop / Code, Grok CLI, and Google Antigravity / Gemini.  
> Second Brain Slash Commands Reference Cheat Sheet — Prints the complete Second Brain slash command cheat sheet directly in chat with syntax, flags, examples, and approval policies.

---

## Overview

`brain-help` provides standardized capabilities across conversational AI platforms:
- Complete command reference table covering all /brain-* triggers.
- Flag syntax documentation (--hops, --tag, --kind, --topK, !durable, !state, !volatile).
- Pre-edit approval policy rules reminder.
- Tri-platform NTFS junctions connecting Claude, Grok, and Antigravity.
- Standard documentation suite: SKILL.md, HOW_TO_USE.txt, IMPLEMENTATION_PLAN.md, and README.md.

---

## Tri-Platform Architecture

Zero duplicate code across platforms. Canonical source resides in `.agents`:
- **Canonical Source**: `C:\Users\<you>\.agents\skills\brain-help`
- **Claude**: `C:\Users\<you>\.claude\skills\brain-help` (NTFS Junction)
- **Grok**: `C:\Users\<you>\.grok\skills\brain-help` (NTFS Junction)
- **Antigravity**: `C:\Users\<you>\.gemini\config\skills\brain-help` (NTFS Junction)

---

## Documentation Suite

- [`HOW_TO_USE.txt`](HOW_TO_USE.txt): Standardized user guide and prompt templates.
- [`IMPLEMENTATION_PLAN.md`](IMPLEMENTATION_PLAN.md): Feature checklist and roadmap.
- [`App Changes Tracker.html`](App%20Changes%20Tracker.html): Interactive visual version log.
- [`SKILL.md`](SKILL.md): Agent system instructions and triggers.
