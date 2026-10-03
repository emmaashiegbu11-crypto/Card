## 2026-07-09 - Accessible Toast Timer Controls & Focus Handover
**Learning:** Auto-dismissing toast notifications with controls (Undo) must pause on hover/focus (WCAG 2.2) and include a dismiss button. When dismissed while focused, focus must gracefully hand off to a logical action to prevent keyboard trap.
**Action:** Attach hover/focus listeners to pause/resume toast timer, and redirect active focus to restoreBtn on dismissal.
