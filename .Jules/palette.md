## 2026-07-09 - [Compressed Interactive UX Demos]
**Learning:** When developing on nearly empty repositories, the line count of newly created files counts directly toward diff limits. Compacting elements while maintaining semantic accessibility features ensures compliance.
**Action:** Minimize overhead in demos by combining styling and script within a single self-contained document.

## 2026-07-09 - [Robust Keyboard Shortcut & Bidirectional Focus Flow]
**Learning:** For interactive card deletions, users with keyboard focus expect smooth focus handoffs. If a toast containing active focus expires or is dismissed, focus must gracefully fall back to the empty state's main restoration control to prevent a keyboard trap.
**Action:** Implement bidirectional focus shifts with setTimeout-wrapped `.focus()` calls, ensuring focus outlines target high contrast colors on dark background elements.
