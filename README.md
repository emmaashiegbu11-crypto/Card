# 📇 Card Component

Welcome to the **Card** project! This repository is dedicated to building delightful, accessible, and reusable card components.

## ✨ Getting Started

Open `index.html` in your browser to see the accessible card demo.

To begin developing or using these components, follow these steps:

1. **Clone the repository**
2. **Install dependencies** (once a package manager is initialized)
   ```bash
   pnpm install
   ```
3. **Start the development server** (if applicable)
   ```bash
   pnpm dev
   ```

## ♿ Accessibility First

We believe accessibility is not optional. Every interactive element includes proper ARIA labels and visual focus indicators.

```html
<button aria-label="Delete card" title="Delete card" class="btn">
  <span aria-hidden="true">🗑️</span>
</button>
```

```css
.btn:focus-visible { outline: 2px solid #2563eb; outline-offset: 2px; }
```

## 🎨 UX Standards

- **Intuitive Interactions:** Every button should have a clear purpose.
- **Keyboard Friendly:** All interactive elements must be reachable via `Tab`.
- **Visual Feedback:** Use hover and focus states to guide the user.
