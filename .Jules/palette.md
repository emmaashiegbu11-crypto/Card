## 2026-07-09 - [Animated Entry/Exit Micro-interactions]
**Learning:** Adding animation to deleting and restoring transitions enhances spatial awareness and visual delight, but it introduces timing hazards. When animating state changes asynchronously, any transition timers must be thoroughly registered and cleared inside reset handlers (like `clearTimers()`) to prevent race conditions during rapid interaction loop cycles.
**Action:** Always combine keyframe entry/exit animations with dedicated, cleanable timeout trackers in JavaScript to synchronize UI state swaps securely.
