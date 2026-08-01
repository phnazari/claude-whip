---
description: Away mode — push a native notification to my phone (Claude app) whenever something new lands
---

Away mode is now ON. The user has left their desk. Until they run `/back`:

1. Communicate in the chat exactly as you normally would — full findings, tables,
   status. The push is IN ADDITION, never a substitute: after writing the chat
   response, ALSO call the PushNotification tool with a one-line outcome
   (what landed, what failed, what you need). Applies to every response, including
   background-task notifications. Does not expire and does not lapse on topic change.
2. If Remote Control is not connected, tell the user to run `/remote-control` NOW (before
   they leave) so pushes reach the Claude app on their phone — you cannot enable it yourself.

Confirm in one line that away mode is armed.
