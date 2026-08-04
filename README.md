<h1 align="center">claude-whip</h1>


<p align="center"><img src="assets/logo-v2.png" width="200"></p>


Solving actual problems of Claude with zero overhead and full transparency, in a handful of tiny markdown files. Zero configuration.

## Features

| Feature | What it does |
|---|---|
| **No yap** (hook) | Auto-suffixes every prompt with a brevity instruction: lead with the answer, no preamble, no recap. |
| **`/away`** | Leaving your desk? Claude pushes a one-line notification to your phone (native Claude app) every time something new lands. |
| **`/back`** | You're back; pushes stop. |
| **`/write-self-handoff`** | Before `/compact`: saves session-specific state (job IDs, exact numbers, ruled-out hypotheses, paths) to a dated file on disk. |
| **`/read-self-handoff`** | After `/compact`: reads the latest handoff back and resumes with full context. |

## Install

```
/plugin marketplace add phnazari/claude-whip
/plugin install whip
```

## Requirements

`/away` pushes need Remote Control (`/remote-control`). The plugin reminds you if it isn't connected.
