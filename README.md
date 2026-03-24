<div align="center">

# 🎱 Bingo Mixer

**The social icebreaker game that gets people talking!**

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Node.js 22+](https://img.shields.io/badge/node-%3E%3D22-brightgreen.svg)](https://nodejs.org/)
[![Built with React](https://img.shields.io/badge/React-19-61dafb.svg)](https://react.dev/)
[![Powered by Vite](https://img.shields.io/badge/Vite-8-646cff.svg)](https://vite.dev/)

[🚀 Play Now](#quick-start) · [📚 Workshop Guide](workshop/GUIDE.md) · [🤝 Contributing](CONTRIBUTING.md)

</div>

---

## ✨ What is Bingo Mixer?

**Bingo Mixer** is a fast, fun, phone-friendly bingo game built for in-person events, meetups, and conferences. Players roam the room finding real people who match the clues on their card — first to get **5 in a row** wins!

No accounts. No installs. Just open the link and play. 🎉

---

## 🕹️ How to Play

| Step | Action |
|------|--------|
| 1️⃣ | Open the game on your phone |
| 2️⃣ | Walk around and find people who match each square |
| 3️⃣ | Tap a square when you've found a match |
| 4️⃣ | Get **5 in a row** — horizontally, vertically, or diagonally |
| 5️⃣ | Shout **BINGO!** 🎊 |

> **Free Space** is always in the center — it's yours for free!

---

## 🌟 Features

- 📱 **Mobile-first** — designed for phones at events
- 🔀 **Randomized boards** — every player gets a unique card
- ⚡ **Instant play** — no sign-up, no download needed
- 💾 **Saves your progress** — leave and come back anytime
- 🎊 **Win celebration** — satisfying bingo animation when you win
- 🚀 **Deploys to GitHub Pages** — share a single URL with your whole event

---

## 🚀 Quick Start

### Option 1 — GitHub Codespaces (zero setup)

Click **Code → Codespaces → Create codespace** on your fork and you're ready to code in seconds.

### Option 2 — Dev Container (VS Code)

Clone the repo, then run **Dev Containers: Reopen in Container** in VS Code.

### Option 3 — Local

```bash
# Prerequisites: Node.js 22+
npm install
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) and start mixing! 🎲

### Deploy

```bash
npm run build
```

Push to `main` — it automatically deploys to **GitHub Pages** at  
`https://<your-username>.github.io/<your-repo-name>/game/`

> The `/game/` sub-path is set by the `VITE_REPO_NAME` environment variable in the deploy workflow. See [`vite.config.ts`](vite.config.ts) to customize.

---

## 🛠️ Tech Stack

| Technology | Role |
|-----------|------|
| [React 19](https://react.dev/) | UI components |
| [TypeScript](https://www.typescriptlang.org/) | Type-safe logic |
| [Vite](https://vite.dev/) | Build & dev server |
| [Tailwind CSS v4](https://tailwindcss.com/) | Styling |
| [Vitest](https://vitest.dev/) | Unit testing |

---

## 🔬 Workshop Lab Guide

This project is also a **hands-on workshop** for learning GitHub Copilot Agent Mode!

| Part | Title | What You'll Do |
|------|-------|----------------|
| [**00**](workshop/00-overview.md) | Overview & Checklist | Get oriented and set up |
| [**01**](workshop/01-setup.md) | Setup & Context Engineering | Onboard AI to your codebase |
| [**02**](workshop/02-design.md) | Design-First Frontend | Redesign the UI with creative themes |
| [**03**](workshop/03-quiz-master.md) | Custom Quiz Master | Build a custom agent for quiz themes |
| [**04**](workshop/04-multi-agent.md) | Multi-Agent Development | Build features with TDD + design agents |

> 📝 Full guide: [`workshop/GUIDE.md`](workshop/GUIDE.md)

---

## 🤝 Contributing

Contributions are welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

<div align="center">

Made with ❤️ for better icebreakers · [MIT License](LICENSE)

</div>
