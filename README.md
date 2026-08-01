# claude-whip

Solving actual problems of Claude with zero overhead and full transparency. This plugin is literally ~5 lines of code.
Two things, zero configuration:

1. **No yap.** Every prompt is auto-suffixed with a brevity instruction, telling claude: **no yap**!
2. **`/away` mode.** Leaving your desk? `/away`. Claude pushes a one-line notification to
   your phone (native Claude app, via Remote Control) every time something new lands. `/back` when you return.

## Install

```
/plugin marketplace add phnazari/claude-whip
/plugin install whip
```

## Requirements

`/away` pushes need Remote Control (`/remote-control`). The plugin reminds you if it isn't connected.
