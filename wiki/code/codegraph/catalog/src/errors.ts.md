---
title: 'Module: src/errors.ts'
type: catalog
provenance: extracted
module: src/errors.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/`errors.ts`/
symbols:
  logDebug: logDebug().
  logWarn: logWarn().
  CodeGraphError: CodeGraphError#
  ParseError.-constructor: ParseError#`<constructor>`().
  defaultLogger: defaultLogger.
  silentLogger: silentLogger.
  currentLogger: currentLogger.
  Logger: Logger#
  setLogger: setLogger().
  getLogger: getLogger().
  CodeGraphError.-constructor: CodeGraphError#`<constructor>`().
  logError: logError().
  FileError: FileError#
  ParseError: ParseError#
  DatabaseError: DatabaseError#
  SearchError: SearchError#
  VectorError: VectorError#
  ConfigError: ConfigError#
  ParseError.-constructor-.options-typeLiteral0.cause: ParseError#`<constructor>`().(options)typeLiteral0:cause.
  Logger.debug: Logger#debug().
  Logger.warn: Logger#warn().
  Logger.error: Logger#error().
  FileError.-constructor: FileError#`<constructor>`().
  DatabaseError.-constructor: DatabaseError#`<constructor>`().
  SearchError.-constructor: SearchError#`<constructor>`().
  ParseError.-constructor-.options-typeLiteral0.line: ParseError#`<constructor>`().(options)typeLiteral0:line.
  ParseError.-constructor-.options-typeLiteral0.column: ParseError#`<constructor>`().(options)typeLiteral0:column.
  CodeGraphError.code: CodeGraphError#code.
  CodeGraphError.context: CodeGraphError#context.
  FileError.filePath: FileError#filePath.
  ParseError.filePath: ParseError#filePath.
  ParseError.line: ParseError#line.
  ParseError.column: ParseError#column.
  DatabaseError.operation: DatabaseError#operation.
  SearchError.query: SearchError#query.
  VectorError.-constructor: VectorError#`<constructor>`().
  ConfigError.-constructor: ConfigError#`<constructor>`().
---
# Module: [`src/errors.ts`](../../../../../raw/code/codegraph/src/errors.ts)

## Classes
### `CodeGraphError`  ·  implements/extends Error
- def: [`src/errors.ts:45`](../../../../../raw/code/codegraph/src/errors.ts#L45)
- doc: Base error class for all CodeGraph errors.
- signature: `class CodeGraphError`
- members:
  - `<constructor>(message: string, code: string, context?: Record<string, unknown> | undefined)` — [`L51`](../../../../../raw/code/codegraph/src/errors.ts#L51) — Base error class for all CodeGraph errors.
  - `code` — [`L47`](../../../../../raw/code/codegraph/src/errors.ts#L47) — Error code for categorization (e.g., 'FILE_ERROR', 'PARSE_ERROR')
  - `context` — [`L49`](../../../../../raw/code/codegraph/src/errors.ts#L49) — Additional context about the error
- uses (calls/refs, reference-scoped): [`ConfigError`](errors.ts.md#ConfigError), [`DatabaseError`](errors.ts.md#DatabaseError), [`FileError`](errors.ts.md#FileError), [`ParseError`](errors.ts.md#ParseError), [`SearchError`](errors.ts.md#SearchError), [`VectorError`](errors.ts.md#VectorError)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`ConfigError`](errors.ts.md#ConfigError), [`DatabaseError`](errors.ts.md#DatabaseError), [`FileError`](errors.ts.md#FileError), [`ParseError`](errors.ts.md#ParseError), [`SearchError`](errors.ts.md#SearchError), [`VectorError`](errors.ts.md#VectorError)

### `ConfigError`  ·  implements/extends CodeGraphError, Error
- def: [`src/errors.ts:157`](../../../../../raw/code/codegraph/src/errors.ts#L157)
- doc: Error with configuration
- signature: `class ConfigError`
- members:
  - `<constructor>(message: string, details?: Record<string, unknown> | undefined)` — [`L158`](../../../../../raw/code/codegraph/src/errors.ts#L158) — Error with configuration
- uses (calls/refs, reference-scoped): [`CodeGraphError`](errors.ts.md#CodeGraphError)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`CodeGraphError`](errors.ts.md#CodeGraphError)

### `DatabaseError`  ·  implements/extends CodeGraphError, Error
- def: [`src/errors.ts:112`](../../../../../raw/code/codegraph/src/errors.ts#L112)
- doc: Error with database operations
- signature: `class DatabaseError`
- members:
  - `<constructor>(message: string, operation: string, cause?: Error | undefined)` — [`L115`](../../../../../raw/code/codegraph/src/errors.ts#L115) — Error with database operations
  - `operation` — [`L113`](../../../../../raw/code/codegraph/src/errors.ts#L113)
- uses (calls/refs, reference-scoped): [`CodeGraphError`](errors.ts.md#CodeGraphError)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`CodeGraphError`](errors.ts.md#CodeGraphError)

### `FileError`  ·  implements/extends CodeGraphError, Error
- def: [`src/errors.ts:67`](../../../../../raw/code/codegraph/src/errors.ts#L67)
- doc: Error reading or accessing files
- signature: `class FileError`
- members:
  - `<constructor>(message: string, filePath: string, cause?: Error | undefined)` — [`L70`](../../../../../raw/code/codegraph/src/errors.ts#L70) — Error reading or accessing files
  - `filePath` — [`L68`](../../../../../raw/code/codegraph/src/errors.ts#L68)
- uses (calls/refs, reference-scoped): [`CodeGraphError`](errors.ts.md#CodeGraphError)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`CodeGraphError`](errors.ts.md#CodeGraphError)

### `Logger`
- def: [`src/errors.ts:170`](../../../../../raw/code/codegraph/src/errors.ts#L170)
- doc: Simple logger for CodeGraph operations
- signature: `interface Logger`
- members:
  - `debug(method)` — [`L171`](../../../../../raw/code/codegraph/src/errors.ts#L171)
  - `error(method)` — [`L173`](../../../../../raw/code/codegraph/src/errors.ts#L173)
  - `warn(method)` — [`L172`](../../../../../raw/code/codegraph/src/errors.ts#L172)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`logDebug`](errors.ts.md#logDebug), [`logWarn`](errors.ts.md#logWarn), [`defaultLogger`](errors.ts.md#defaultLogger), [`silentLogger`](errors.ts.md#silentLogger), [`currentLogger`](errors.ts.md#currentLogger), [`getLogger`](errors.ts.md#getLogger), [`setLogger`](errors.ts.md#setLogger), [`logError`](errors.ts.md#logError)

### `ParseError`  ·  implements/extends CodeGraphError, Error
- def: [`src/errors.ts:83`](../../../../../raw/code/codegraph/src/errors.ts#L83)
- doc: Error parsing source code
- signature: `class ParseError`
- members:
  - `<constructor>(message: string, filePath: string, options?: { line?: number | undefined; column?: number | undefined; cause?: Error | undefined; } | undefined)` — [`L88`](../../../../../raw/code/codegraph/src/errors.ts#L88) — Error parsing source code
  - `cause` — [`L91`](../../../../../raw/code/codegraph/src/errors.ts#L91)
  - `column` — [`L86`](../../../../../raw/code/codegraph/src/errors.ts#L86)
  - `column` — [`L91`](../../../../../raw/code/codegraph/src/errors.ts#L91)
  - `filePath` — [`L84`](../../../../../raw/code/codegraph/src/errors.ts#L84)
  - `line` — [`L85`](../../../../../raw/code/codegraph/src/errors.ts#L85)
  - `line` — [`L91`](../../../../../raw/code/codegraph/src/errors.ts#L91)
- uses (calls/refs, reference-scoped): [`CodeGraphError`](errors.ts.md#CodeGraphError)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`CodeGraphError`](errors.ts.md#CodeGraphError)

### `SearchError`  ·  implements/extends CodeGraphError, Error
- def: [`src/errors.ts:128`](../../../../../raw/code/codegraph/src/errors.ts#L128)
- doc: Error with search operations
- signature: `class SearchError`
- members:
  - `<constructor>(message: string, query: string, cause?: Error | undefined)` — [`L131`](../../../../../raw/code/codegraph/src/errors.ts#L131) — Error with search operations
  - `query` — [`L129`](../../../../../raw/code/codegraph/src/errors.ts#L129)
- uses (calls/refs, reference-scoped): [`CodeGraphError`](errors.ts.md#CodeGraphError)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`CodeGraphError`](errors.ts.md#CodeGraphError)

### `VectorError`  ·  implements/extends CodeGraphError, Error
- def: [`src/errors.ts:144`](../../../../../raw/code/codegraph/src/errors.ts#L144)
- doc: Error with vector/embedding operations
- signature: `class VectorError`
- members:
  - `<constructor>(message: string, operation: string, cause?: Error | undefined)` — [`L145`](../../../../../raw/code/codegraph/src/errors.ts#L145) — Error with vector/embedding operations
- uses (calls/refs, reference-scoped): [`CodeGraphError`](errors.ts.md#CodeGraphError)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`CodeGraphError`](errors.ts.md#CodeGraphError)

## Functions
- `getLogger()` — [`L217`](../../../../../raw/code/codegraph/src/errors.ts#L217) — Get the current logger
- `logDebug(message: string, context?: Record<string, unknown> | undefined)` — [`L224`](../../../../../raw/code/codegraph/src/errors.ts#L224) — Log a debug message
- `logError(message: string, context?: Record<string, unknown> | undefined)` — [`L238`](../../../../../raw/code/codegraph/src/errors.ts#L238) — Log an error message
- `logWarn(message: string, context?: Record<string, unknown> | undefined)` — [`L231`](../../../../../raw/code/codegraph/src/errors.ts#L231) — Log a warning message
- `setLogger(logger: Logger)` — [`L210`](../../../../../raw/code/codegraph/src/errors.ts#L210) — Set the global logger

## Module values
- `currentLogger` — [`L205`](../../../../../raw/code/codegraph/src/errors.ts#L205) — Current logger instance (can be replaced)
- `defaultLogger` — [`L179`](../../../../../raw/code/codegraph/src/errors.ts#L179) — Default console-based logger
- `silentLogger` — [`L196`](../../../../../raw/code/codegraph/src/errors.ts#L196) — Silent logger (no output) - useful for tests

