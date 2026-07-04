---
title: 'Module: understand-anything-plugin/packages/core/src/ignore-generator.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/ignore-generator.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/`ignore-generator.ts`/
symbols:
  generateStarterIgnoreFile: generateStarterIgnoreFile().
  TEST_PATTERN_GROUPS.Array.typeLiteral5.patterns: TEST_PATTERN_GROUPS.Array:typeLiteral5:patterns.
  TEST_PATTERN_GROUPS.Array.typeLiteral5.label: TEST_PATTERN_GROUPS.Array:typeLiteral5:label.
  detectDirectories: detectDirectories().
  isCoveredByDefaults: isCoveredByDefaults().
  HEADER: HEADER.
  EXACT_DIR_NAMES: EXACT_DIR_NAMES.
  SUFFIX_DIR_GLOBS: SUFFIX_DIR_GLOBS.
  TEST_PATTERN_GROUPS: TEST_PATTERN_GROUPS.
  parseGitignorePatterns: parseGitignorePatterns().
---
# Module: [`understand-anything-plugin/packages/core/src/ignore-generator.ts`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts)

## Functions
- `detectDirectories(projectRoot: string)` — [`L126`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts#L126) — Detects directories under projectRoot that match either an exact name
- `generateStarterIgnoreFile(projectRoot: string)` — [`L153`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts#L153) — Generates a starter .understandignore file content by scanning the project
- `isCoveredByDefaults(pattern: string)` — [`L115`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts#L115) — Returns true if a gitignore pattern is already covered by the hardcoded defaults.
- `parseGitignorePatterns(gitignorePath: string)` — [`L102`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts#L102) — Parses a .gitignore file and returns active patterns (no comments, no blanks).

## Module values
- `EXACT_DIR_NAMES` — [`L20`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts#L20)
- `HEADER` — [`L5`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts#L5)
- `SUFFIX_DIR_GLOBS` — [`L44`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts#L44)
- `TEST_PATTERN_GROUPS` — [`L52`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts#L52)
- `label` — [`L52`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts#L52)
- `patterns` — [`L52`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/ignore-generator.ts#L52)

