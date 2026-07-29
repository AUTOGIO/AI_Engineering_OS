# Engineering Kernel

Contracts and rules for the AI Engineering OS knowledge layer.

## Current scope

This folder holds **v0.1 schema contracts** (custom YAML DSL) and `KERNEL_MANIFEST.md`.
There is no validator or automation consumer yet — schemas are editorial contracts until tooling is added.

## Schema format (decision)

- **Keep** the custom DSL used by `PROJECT_SCHEMA.yaml` (`schema` / `required` / `type` / `values`).
- **Do not** introduce a second dialect in this repo.
- Migration to JSON Schema (and a `scripts/` validator) is **deferred** until there is at least one real instance document to validate.

## Schemas (v0.1)

| File | Object | Status |
|------|--------|--------|
| `PROJECT_SCHEMA.yaml` | Project | Defined |
| `KNOWLEDGE_SCHEMA.yaml` | Knowledge Unit | Defined |
| `PATTERN_SCHEMA.yaml` | Pattern | Defined |
| `AGENT_SCHEMA.yaml` | Agent | Defined |
| `WORKFLOW_SCHEMA.yaml` | Workflow | Defined |
| `CONTEXT_SCHEMA.yaml` | Context (shared runtime/session bag) | Defined |

## Deferred canonical objects

Listed in `KERNEL_MANIFEST.md` but **not** given schema files yet:

Reasoning Session, Architecture, Decision, Trace, Report, Prompt, Memory.

Do not invent empty schema files for these. Add a real v0.1 schema when the object is needed.
