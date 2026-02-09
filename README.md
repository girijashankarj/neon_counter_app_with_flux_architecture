<p align="center">
  <h1 align="center">neon_counter_app_with_flux_architecture</h1>
  <p align="center">
    A neon-themed counter application built with vanilla JavaScript demonstrating the Flux architecture pattern — increment, decrement, and learn unidirectional data flow.
  </p>
</p>

<p align="center">
  <a href="https://github.com/girijashankarj/neon_counter_app_with_flux_architecture"><img src="https://img.shields.io/github/last-commit/girijashankarj/neon_counter_app_with_flux_architecture?style=flat-square&logo=github" alt="last commit" /></a>
  <img src="https://img.shields.io/badge/JavaScript-vanilla-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Architecture-Flux-764ABC?style=flat-square" alt="Flux" />
  <img src="https://img.shields.io/badge/Type-Educational-FF9800?style=flat-square" alt="Educational" />
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square" alt="PRs welcome" />
</p>

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Flux Architecture](#flux-architecture)
- [Quick Start](#quick-start)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

**neon_counter_app_with_flux_architecture** is an educational project that demonstrates the Flux architecture pattern using a simple counter. It uses vanilla JavaScript — no frameworks — to show how Actions, a Dispatcher, a Store, and a View work together to create predictable, unidirectional data flow. The neon cyan/pink theme makes it visually striking.

---

## Features

- **Increment** — add 1 to the counter
- **Decrement** — subtract 1 from the counter
- **Neon theme** — cyan and pink glow effects
- **Pure Flux** — Dispatcher, Store, Actions, View — no frameworks
- **Single file** — entire app in one HTML file for easy learning

---

## Flux Architecture

```mermaid
flowchart LR
    A["User clicks<br/>+1 or -1"] --> B["Actions<br/>incrementCounter<br/>decrementCounter"]
    B --> C["Dispatcher<br/>dispatch()"]
    C --> D["CounterStore<br/>state management"]
    D --> E["CounterView<br/>re-render display"]
    E -->|user interaction| A

    style A fill:#FF9800,color:#fff
    style B fill:#2196F3,color:#fff
    style C fill:#9C27B0,color:#fff
    style D fill:#4CAF50,color:#fff
    style E fill:#F44336,color:#fff
```

**Why Flux?**
- **Predictable data flow** — one-way data movement
- **Centralized state** — single source of truth
- **Separation of concerns** — clear roles for each layer
- **Easier debugging** — traceable state changes

---

## Quick Start

```bash
git clone https://github.com/girijashankarj/neon_counter_app_with_flux_architecture.git
cd neon_counter_app_with_flux_architecture
```

Open `neon_counter_app_with_flux_architecture.html` directly in your browser — no build step required.

---

## Project Structure

```
neon_counter_app_with_flux_architecture/
├── neon_counter_app_with_flux_architecture.html    # Single-file app
└── README.md
```

---

## How It Works

| Layer          | Responsibility                                    |
| -------------- | ------------------------------------------------- |
| **Actions**    | Create action objects (`INCREMENT`, `DECREMENT`)  |
| **Dispatcher** | Central hub — receives actions, notifies store    |
| **Store**      | Holds counter state, processes dispatched actions |
| **View**       | Renders the counter, listens for store changes    |

The entire implementation lives in a single HTML file with embedded JavaScript and CSS — making it easy to read, modify, and learn from.

---

## Contributing

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/my-feature`
3. **Make** your changes
4. **Commit** and open a Pull Request

---

## License

This project is open source. See the [LICENSE](LICENSE) file for details.

---

<p align="center">
  Built with discipline by <a href="https://github.com/girijashankarj">GarryTJ</a>
</p>
