# AI Agent Instructions for Vite Vue Template

This file provides guidance for AI coding agents customizing this Vite + Vue template.

## Quick Start

1. **App Entry**: Edit `src/App.vue` for main application
2. **Styling**: Edit `src/style.css` for global styles
3. **Components**: Add components to `src/components/`

---

## Files to MODIFY (Customize These)

### Core Application
| File | Purpose |
|------|---------|
| `src/App.vue` | Main application component |
| `src/style.css` | Global styles |
| `index.html` | HTML template, page title, meta tags |

### Assets
| Location | Purpose |
|----------|---------|
| `src/assets/` | Images, fonts, static files |
| `public/` | Public static files (favicon, etc.) |

### Configuration
| File | Purpose |
|------|---------|
| `vite.config.ts` | Vite build configuration |

---

## Project Structure

```
src/
├── App.vue          # Main app component
├── main.ts          # Entry point
├── style.css        # Global styles
├── components/      # Vue components
└── assets/          # Static assets
```

---

## Vue Component Structure

```vue
<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
  <button @click="count++">
    Count: {{ count }}
  </button>
</template>

<style scoped>
button {
  padding: 0.5rem 1rem;
}
</style>
```

---

## Build and Test

```bash
# Install dependencies
npm install

# Start dev server (hot reload)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

---

## Deployment Notes

**Build output**: `dist/` folder

For static hosting:
1. Run `npm run build`
2. Deploy the `dist/` folder

For Netlify, add `netlify.toml`:
```toml
[build]
  command = "npm run build"
  publish = "dist"
```
