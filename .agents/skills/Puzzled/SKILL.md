```markdown
# Puzzled Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill outlines the core development patterns and conventions used in the Puzzled TypeScript codebase. It covers file organization, import/export styles, commit message habits, and testing approaches. By following these guidelines, contributors can maintain consistency and quality across the project.

## Coding Conventions

### File Naming
- Use **PascalCase** for all file names.
  - Example: `PuzzleBoard.ts`, `GameLogic.ts`

### Import Style
- Use **relative imports** for referencing modules within the codebase.
  - Example:
    ```typescript
    import { PuzzlePiece } from './PuzzlePiece';
    ```

### Export Style
- Use **named exports** rather than default exports.
  - Example:
    ```typescript
    // In PuzzlePiece.ts
    export function PuzzlePiece() { ... }
    ```
    ```typescript
    // In another file
    import { PuzzlePiece } from './PuzzlePiece';
    ```

### Commit Patterns
- Commit messages are **freeform** and do not follow a strict prefix.
- Average commit message length is about 34 characters.
  - Example: `Fix edge case in puzzle solver`

## Workflows

_No automated workflows detected in the repository._

## Testing Patterns

- **Testing Framework:** Not explicitly detected.
- **Test File Pattern:** All test files follow the `*.test.*` naming convention.
  - Example: `PuzzleBoard.test.ts`
- **Test Placement:** Tests are placed alongside or near the files they test.

## Commands

| Command | Purpose |
|---------|---------|
| /test   | Run all test files matching `*.test.*` |
| /lint   | (Suggested) Lint the codebase for style consistency |
| /format | (Suggested) Format code according to conventions |

```