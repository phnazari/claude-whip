---
name: read-self-handoff
description: Read the latest self-handoff note back after /compact, so the conversation can resume with session-specific detail intact. Use after the user runs /compact (paired with write-self-handoff), or whenever the user asks to "read the latest self_handoff" / "restore the handoff" / "load the handoff back".
---

# Read the self-handoff back

`/compact` strips session-specific detail. This skill reads the latest handoff file written by
`write-self-handoff` so you can resume with full context.

## Flow

1. List `docs/self_handoff/` and pick the **latest** file (highest date, then highest counter).
   If the directory doesn't exist or is empty, tell the user there's no handoff to load and stop.
2. Read it.
3. Confirm to the user in 1–2 sentences what you've loaded back (the gist — what we were doing,
   the immediate next step). Don't dump the whole file.
4. **Then stop.** Do not auto-resume work — wait for the user to direct you. They might want to
   switch tasks; the handoff is context, not a queue.
