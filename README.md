# 📇 Card Component

Welcome to the **Card** project! This repository is dedicated to building delightful, accessible, and reusable card components.

## ✨ Getting Started

Open `index.html` in your browser to see the accessible card demo featuring a "Copy to Clipboard" micro-interaction.

## ♿ Accessibility First

We believe accessibility is not optional. Every interactive element includes proper ARIA labels, focus states, and screen reader feedback.

### Key Accessibility Features in this Demo:
- **ARIA Labels:** Icon-only buttons include descriptive `aria-label` attributes.
- **Screen Reader Feedback:** We use `aria-live="polite"` regions to announce dynamic updates, like successful clipboard copying.
- **Keyboard Navigation:** All interactive elements are fully reachable via `Tab` and feature clear `:focus-visible` styles.
- **Visual Feedback:** We use tooltips and icon changes to provide immediate visual confirmation of actions.

## 🎨 UX Standards

- **Intuitive Interactions:** Every button should have a clear purpose and immediate feedback.
- **Tactile Feel:** Use of `:active` states to provide physical-like response to clicks.
- **Predictable Behavior:** Actions like "Copy" provide clear visual and auditory (via screen reader) confirmation.
