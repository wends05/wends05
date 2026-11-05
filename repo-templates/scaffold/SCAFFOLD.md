# Project scaffold

Run this in a new project's root. It overwrites files with the same name, so use a fresh project.

```bash
bunx degit wends05/wends05/repo-templates/scaffold . --force
```

This copies `AGENTS.md`, `docs/`, and this file. Then fill every `FILL` comment and every `<name: hint>` slot. The hint says what to write; replace the whole tag.

```bash
grep -rnE "FILL|<[a-z ]+: " AGENTS.md docs
```

Delete a section that does not apply instead of leaving it empty. Delete this file when you are done.

This file is named `SCAFFOLD.md`, not `README.md`, so copying it never overwrites a project's own README.

Claude Code may read `CLAUDE.md` rather than `AGENTS.md`. If a fresh session does not load `AGENTS.md`, add a one-line `CLAUDE.md` containing `@AGENTS.md`.
