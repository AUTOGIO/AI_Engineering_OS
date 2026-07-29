# AGENTS.md — repository layout

Personal knowledge / engineering-OS repo. Keep the layout simple and stable.

## Top-level folders

| Folder | Purpose |
|--------|---------|
| `config/` | Non-secret settings and schemas (e.g. `config/engineering_kernel/`) |
| `docs/` | Markdown guides, design notes |
| `docs/prompts/` | AI prompt files |
| `scripts/` | Runnable helpers (`.sh`, `.zsh`, Makefile script targets) |
| `archive/` | Obsolete files kept for reference — do not delete casually |
| Root | Only `README.md`, `AGENTS.md`, `.gitignore`, and toolchain files (e.g. `*.code-workspace`) |

Create these only when needed (ask before adding other top-level names):

- `src/` or `app/` — application code (pick one; never both)
- `data/` — CSV, Excel, exports (`data/raw`, `data/processed` if helpful)
- `assets/` — images, icons, logos
- `tests/` — tests only

## Rules

1. Prefer **move** over copy. Prefer **edit** existing files over creating new ones.
2. Do not invent new top-level folders without asking.
3. No filename versioning (`Foo_v1.0.md` → `docs/foo.md`; old copy → `archive/` if unsure).
4. Merge duplicates into the canonical folders above.
5. Never commit secrets (`.env`, keys, credentials).
6. Folder names stay English as listed; content filenames may stay Portuguese/English as already used.
7. After moves, fix broken paths if anything would break.
8. Do not delete unless clearly a duplicate; otherwise move to `archive/`.
