# AI Agent Instructions

## Mandatory First Step

At the start of **every conversation**, before answering any question or performing any task, read the following context files:

1. `docs/context/productContext.md` — What the product is and its key features.
2. `docs/context/techContext.md` — Technology stack and development setup.
3. `docs/context/systemPatterns.md` — Architecture, codebase structure, and data flow.
4. `docs/context/activeContext.md` — Current focus, recent changes, and next steps.

If any additional context files exist in `docs/context/`, read those as well.

## Project Overview

OWASP Threat Dragon is an open-source threat modeling tool. It is a split-stack application:

- **`td.vue/`** — Vue 2 SPA frontend (diagramming with AntV X6, BootstrapVue UI).
- **`td.server/`** — Express backend (OAuth proxy for GitHub/GitLab/Bitbucket).
- **Desktop** — Electron wrapper around `td.vue` with direct filesystem access.

## Rules

- Always check `docs/context/activeContext.md` to understand what is currently being worked on before suggesting changes.
- When making significant changes, update `docs/context/activeContext.md` with what was done.
- Prefer reading existing code and patterns before proposing new ones.
- Every task must follow Behavior Driven Development (BDD) and Test Driven Development (TDD) methodologies.
