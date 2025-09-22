# Weazel News Kit V4 — Fix for Vercel
- Перенёс `vite` и `@vitejs/plugin-react` в `dependencies` (чтобы Vercel точно их установил даже при прод-сборке).
- Добавил `vercel.json` с `installCommand: npm install`, `buildCommand: npm run build`, `functions.runtime: nodejs18.x`.
- В `index.html` путь к точке входа `./src/main.jsx`, а в `vite.config.js` — `base: ''` и `outDir: dist`.
