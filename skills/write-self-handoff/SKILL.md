---
name: write-self-handoff
description: Write a self-handoff note to disk so post-compact Claude can pick up where pre-compact Claude left off. Use right before the user runs /compact, when context is getting long, or whenever you'd otherwise lose session-specific state (job IDs, exact numbers, ruled-out hypotheses, file paths, things you got wrong). Pair with read-self-handoff after the user compacts.
---

# Write a self-handoff before /compact

`/compact` summarises the conversation and inevitably loses session-specific detail. This skill
writes that detail to disk so post-compact you can read it back via `read-self-handoff`.

## Flow

1. List `docs/self_handoff/` (create it if it doesn't exist). Pick the next filename:
   `docs/self_handoff/YYYY-MM-DD.md`, or `YYYY-MM-DD-1.md`, `-2.md`, … if today already has files.
2. Write a single markdown file that includes **everything that should not be forgotten at /compact**.
   Use whatever structure fits. Lead with what's most load-bearing for resuming work.
