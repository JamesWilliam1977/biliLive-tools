```markdown
# biliLive-tools Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the core development patterns and conventions used in the `biliLive-tools` TypeScript codebase. It covers file naming, import/export styles, commit message practices, and testing patterns, providing practical examples and command suggestions for efficient workflow management.

## Coding Conventions

### File Naming
- **Pattern:** PascalCase
- **Example:**  
  ```plaintext
  LiveRoomManager.ts
  UserSessionHandler.ts
  ```

### Import Style
- **Pattern:** Absolute imports are preferred.
- **Example:**
  ```typescript
  import { LiveRoom } from 'src/LiveRoomManager';
  ```

### Export Style
- **Pattern:** Mixed (both default and named exports are used)
- **Examples:**
  ```typescript
  // Named export
  export function startLiveStream() { ... }

  // Default export
  export default class LiveRoomManager { ... }
  ```

### Commit Messages
- **Pattern:** Freeform, average length ~17 characters.
- **Example:**  
  ```plaintext
  fix login bug
  add new feature
  update config
  ```

## Workflows

_No automated workflows detected in the repository._

## Testing Patterns

- **Framework:** Unknown (not explicitly detected)
- **File Pattern:** Test files are named with the `*.test.*` convention.
- **Example:**
  ```plaintext
  LiveRoomManager.test.ts
  ```
- **Typical Test Structure:**
  ```typescript
  // Example test file
  import { startLiveStream } from 'src/LiveRoomManager';

  test('should start live stream', () => {
    expect(startLiveStream()).toBeTruthy();
  });
  ```

## Commands
| Command | Purpose |
|---------|---------|
| /test   | Run all test files matching `*.test.*` |
| /lint   | Lint the codebase (suggested, if linter is configured) |
| /build  | Build the TypeScript project (suggested) |
```