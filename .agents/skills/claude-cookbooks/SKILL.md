```markdown
# claude-cookbooks Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill documents the core development patterns and conventions used in the `claude-cookbooks` repository. The codebase is written in TypeScript and is not tied to any specific framework. It emphasizes consistent file naming, import/export styles, and commit message conventions. This guide will help contributors quickly adapt to the project's standards and workflows.

## Coding Conventions

### File Naming
- Files are named using **camelCase**.
  - Example: `myUtilityFile.ts`

### Import Style
- Use **relative imports** for all modules.
  - Example:
    ```typescript
    import { myFunction } from './utils';
    ```

### Export Style
- Use **named exports** exclusively.
  - Example:
    ```typescript
    export function myFunction() { /* ... */ }
    ```

### Commit Messages
- Follow the **conventional commit** format.
- Use the `chore` prefix for maintenance and non-feature commits.
  - Example:
    ```
    chore: update dependencies for security patch
    ```

## Workflows

### Code Contribution
**Trigger:** When adding new features, utilities, or making improvements  
**Command:** `/contribute`

1. Create a new file using camelCase naming.
2. Write your TypeScript code, using named exports.
3. Use relative imports for any dependencies.
4. Write or update corresponding test files (`*.test.*`).
5. Commit changes using the conventional commit format (e.g., `chore: add new utility function`).
6. Submit a pull request for review.

### Running Tests
**Trigger:** When verifying code changes or before submitting a pull request  
**Command:** `/test`

1. Identify or create test files matching the `*.test.*` pattern.
2. Run the test suite using the project's preferred test runner (framework not specified; check project documentation or package scripts).
3. Ensure all tests pass before pushing changes.

## Testing Patterns

- Test files follow the `*.test.*` naming convention (e.g., `myFunction.test.ts`).
- The specific testing framework is not specified; refer to the project documentation or `package.json` for details.
- Place tests alongside the code or in a dedicated test directory, as per project structure.

## Commands
| Command      | Purpose                                      |
|--------------|----------------------------------------------|
| /contribute  | Start the code contribution workflow         |
| /test        | Run the test suite for the codebase          |
```
