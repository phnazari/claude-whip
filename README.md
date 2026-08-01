# claude-whip

Two things, zero configuration:

1. **No yap.** Every prompt is auto-suffixed with a brevity instruction. Claude leads with
   the answer. No preamble, no recap, no "hope this helps".
2. **`/away` mode.** Leaving your desk? `/away`. Claude pushes a one-line notification to
   your phone (native Claude app, via Remote Control) every time something new lands — a
   build finishing, tests failing, a long task completing. `/back` when you return.

## Install

```
/plugin marketplace add phnazari/claude-whip
/plugin install whip
```

## Requirements

`/away` pushes need Remote Control (`/remote-control`) — the plugin reminds you if it isn't connected.
