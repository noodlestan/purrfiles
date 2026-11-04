# Guide: Purrfiles

> Own and publish the Purrfiles meta packages: the entity model and extraction tooling.

Monorepo hosting `@noodlestan/purrfiles-entities` (the framework-agnostic entity model and meta service) and `@noodlestan/purrfiles-extract` (the TypeScript extraction tooling), moved from Art MD.

## Recommended Reading

Agents SHOULD scan these files for relevant clarifications when faced with ambiguity or omissions that may result from missing definitions.

- `_guide.md` — this file: system overview, layout, setup, verification.
- `_records/project.art` — the project record.
- `_records/repository.art` — the repository record.

## Repository Layout

```
libs/       — library packages
cli/        — CLI packages
```

## Packages

| Package                          | Path                       |
| -------------------------------- | -------------------------- |
| `@noodlestan/purrfiles-entities` | `libs/purrfiles-entities/` |
| `@noodlestan/purrfiles-extract`  | `cli/purrfiles-extract/`   |

## Conventions

This repository follows strict conventions. Read the convention indexes listed below and follow them when planning and executing work.

- `./node_modules/@noodlestan/conventions-typescript/art/index.md` — TypeScript conventions.
- `./node_modules/@noodlestan/conventions-unit-tests/art/index.md` — Unit Test conventions.

## Operating Instructions

### Operating Instructions: Setting Up

**Instructions:**

Run from the repository root (monorepo):

```bash
npm ci # to install dependencies.
```

### Operating Instructions: Verifying Completion

**Instructions:**

Runs automatically on pre-commit hook (from the repository root):

```bash
npm run ci # lint, then every package's ci
```
