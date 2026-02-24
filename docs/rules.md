# Project Rules

## Coding Standards
1.  **Vue Version**: Use **Vue 2** syntax (Options API) as the codebase is on Vue 2.7. Avoid Vue 3 Composition API unless specifically refactoring to it.
2.  **Linter**: Follow `standard` JS style. Run `npm run lint` before committing.
3.  **Async/Await**: Prefer `async/await` over raw Promises.

## Naming Conventions
-   **Components**: PascalCase (e.g., `ThreatDiagram.vue`).
-   **Files**: kebab-case (e.g., `threat-diagram.js`).
-   **Variables**: camelCase.

## Documentation
-   Update `docs/context/activeContext.md` at the start of every significant session.
-   Keep `techContext.md` updated if dependencies change.

## Testing
-   **Unit Tests**: Required for logic changes (`td.vue/tests/unit`).
-   **E2E**: Required for critical user flows.
