# ECOFALL — Next.js

Converted from the supplied standalone HTML into a Next.js App Router project. The UI is rendered by React, styles live in `app/globals.css`, and the original Canvas game engine is preserved in `public/game-engine.js`.

## Run

```bash
npm install
npm run dev
```

Open http://localhost:3000. For production: `npm run build` and `npm start`.

## Files
- `app/page.jsx`: homepage
- `components/EcofallGame.jsx`: React game UI and engine loader
- `app/globals.css`: original styling
- `public/game-engine.js`: original game logic, kept intact

## Notes
The existing game engine is DOM-based, not rewritten into React state. This minimizes behavioral changes during conversion. For a future React-native refactor, migrate game state/event bindings into hooks and clean up animation frames on unmount.
