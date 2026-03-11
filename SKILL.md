---
name: typescript
description: Guidelines for how to work with TypeScript
---

# TypeScript

## Do not

- Don't combine type imports with non-type imports in the same import statement. Separate them into two statements.

  ```typescript
  // Bad
  import { type MyType, myFunction } from "./myModule";

  // Good
  import type { MyType } from "./myModule";
  import { myFunction } from "./myModule";
  ```
