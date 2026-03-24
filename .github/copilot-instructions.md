# Copilot instructions for Bingo Mixer

## Stack and scope
- Vite + React 19 + TypeScript + Tailwind CSS v4.
- Client-only app; game state is in React state + `localStorage`.
- Entry points: `src/main.tsx`, `src/App.tsx`.

## Architecture
- `App` routes between `StartScreen` (`gameState === 'start'`) and `GameScreen`, with `BingoModal` overlay.
- Game orchestration: `src/hooks/useBingoGame.ts`.
- Pure domain logic only in `src/utils/bingoLogic.ts` (`generateBoard`, `toggleSquare`, `checkBingo`, `getWinningSquareIds`).
- Shared types: `src/types/index.ts`.
- Static questions: `src/data/questions.ts` (`FREE SPACE` at index 12).

## Persistence and behavior rules
- Persist key: `bingo-game-state`, `version: 1` in `useBingoGame.ts`.
- Keep `validateStoredData` aligned with any persisted-shape changes.
- Guard storage access with `typeof window === 'undefined'` checks.
- Keep bingo transition via `queueMicrotask` in `handleSquareClick`.

## UI and styling conventions
- Keep `src/components/*` presentational with explicit typed `Props`.
- `BingoBoard` maps data to `BingoSquare`; pass click actions via callbacks.
- Center free-space remains disabled + always marked (`isFreeSpace` behavior).
- Tailwind v4 is CSS-first (`@import 'tailwindcss'` + `@theme` tokens in `src/index.css`).
- Reuse existing tokens (`accent`, `accent-light`, `marked`, `marked-border`) before adding colors.

## Quality and config
- Commands: `npm install`, `npm run dev`, `npm run build`, `npm run lint`, `npm run test`.
- Logic tests live in `src/utils/bingoLogic.test.ts`; update when board rules change.
- Vite config: `vite.config.ts` (`@vitejs/plugin-react`, `@tailwindcss/vite`).
- Pages base path: `VITE_REPO_NAME` → `/${repo}/game/`, else `/`.
- TypeScript is strict (`tsconfig.app.json`): avoid `any` and unused vars/params.
