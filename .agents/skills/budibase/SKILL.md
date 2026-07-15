```markdown
# budibase Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the core development patterns and conventions used in the `budibase` repository, a TypeScript codebase built with the Svelte framework. You'll learn about file naming, import/export styles, commit message patterns, and how to write and organize tests. This guide will help you contribute code that matches the project's established style and structure.

## Coding Conventions

### File Naming
- Use **camelCase** for file names.
  - Example: `userProfile.ts`, `dataService.ts`

### Import Style
- Use **relative imports** for modules within the codebase.
  - Example:
    ```typescript
    import { fetchData } from './dataService'
    ```

### Export Style
- Use **named exports** for functions, types, and components.
  - Example:
    ```typescript
    // dataService.ts
    export function fetchData() { ... }
    export const DATA_LIMIT = 100
    ```

### Commit Messages
- Commit messages are **freeform** (no enforced type or prefix).
- Average commit message length: **62 characters**.
  - Example:
    ```
    Fix bug in user authentication flow
    ```

## Workflows

_No automated workflows detected in this repository._

## Testing Patterns

- **Test files** follow the pattern: `*.test.*`
  - Example: `userService.test.ts`
- **Testing framework** is unknown, but tests are colocated with source files or in dedicated test files.
- Example test file structure:
  ```typescript
  // userService.test.ts
  import { fetchUser } from './userService'

  test('fetchUser returns correct user data', () => {
    // ...test implementation
  })
  ```

## Commands
| Command | Purpose |
|---------|---------|
| /coding-conventions | Show coding conventions for budibase |
| /testing-patterns   | Show how to write and organize tests |
```