---
description: Away mode — push a native notification to my phone (Claude app) whenever something new lands
---

Enable away mode:

1. Run `touch ~/.claude/.away` (this arms a per-message reminder via the plugin's hook).
2. Until the user runs `/back`: end EVERY turn by calling the PushNotification tool with a
   one-line outcome (what landed, what failed, what you need). Applies to every response,
   including background-task notifications. Does not expire or lapse on topic change.
3. If Remote Control is not connected, tell the user to run `/remote-control` NOW (before
   they leave) so pushes reach the Claude app on their phone — you cannot enable it yourself.

Confirm in one line that away mode is armed.
