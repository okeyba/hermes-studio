---
date: 2026-06-12
pr: pending
feature: Live chat transcript scrolling
impact: The live chat transcript uses native scrolling instead of dynamic virtualization to reduce environment-dependent jumps during streaming responses.
---

`MessageList` now disables `VirtualMessageList` virtualization for the active live chat transcript. `VirtualMessageList` keeps the same exposed scroll API and still defaults to virtualized rendering for history, group chat, and other callers, but can render a native scroll container when `virtualized` is false.
