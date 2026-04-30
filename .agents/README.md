# React Workspace Notes

## Scope

This repo owns:
- `@deepgram/react` in `packages/react/`
- local examples in `examples/`

Sibling dependency:
- `../agent` → `@deepgram/agents`

## Commands

```bash
bun run build
bun run typecheck
bun run test
bun run dev
```

## Architecture Notes

- `@deepgram/react` depends on `@deepgram/agents`.
- It provides the provider + hooks layer only; no bundled UI.
- `@deepgram/ui` consumes this package for prebuilt components.

## File Layout

```text
packages/
  react/    # @deepgram/react
examples/   # local usage examples
```
