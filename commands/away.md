---
description: Away mode — push a native notification to my phone (Claude app) whenever something new lands
---

Away mode is now ON. The user has left their desk. Until they run `/back`:

1. End EVERY turn by calling the PushNotification tool with a one-line outcome
   (what landed, what failed, what you need). Lead with what they would act on.
2. This applies to every response, including background-task notifications you handle.
   It does not expire and does not lapse when the topic changes.
3. First, check whether Remote Control is connected. If it is not, tell the user to run
   `/remote-control` NOW (before they leave) so pushes reach the Claude app on their phone
   — you cannot enable it yourself.

Confirm in one line that away mode is armed.
