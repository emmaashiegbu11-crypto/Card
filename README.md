# 📇 Card Component

Welcome to the **Card** project! This repository is dedicated to building delightful, accessible, and reusable card components.

## ✨ Getting Started

To begin developing or using these components, follow these steps:

1. **Clone the repository**
2. **Install dependencies** (once a package manager is initialized)
   ```bash
   pnpm install
   ```
3. **Start the development server**
   ```bash
   pnpm dev
   ```

## ♿ Accessibility First

We believe accessibility is not optional. Here is a foundational example of an accessible card interaction:

```html
<div class="card">
  <h3>Card Title</h3>
  <p>Some interesting content goes here.</p>
  <!-- ✅ Accessible icon-only button with ARIA label -->
  <button
    aria-label="Delete card"
    class="icon-button"
    onclick="handleDelete()"
  >
    🗑️
  </button>
</div>
```

## 🎨 UX Standards

- **Intuitive Interactions:** Every button should have a clear purpose.
- **Keyboard Friendly:** All interactive elements must be reachable via `Tab`.
- **Visual Feedback:** Use hover and focus states to guide the user.
