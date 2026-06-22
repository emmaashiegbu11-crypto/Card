# 📇 Card Component

Delightful, accessible, and reusable card components.

## ✨ Getting Started
Open `index.html` in your browser to see the accessible card demo.

## ♿ Accessibility First
Every interactive element includes proper ARIA labels and visual focus indicators.

```html
<button aria-label="Delete card" title="Delete card" class="btn">
  <span aria-hidden="true">🗑️</span>
</button>
```

```css
.btn:focus-visible { outline: 2px solid #2563eb; outline-offset: 2px; }
```
