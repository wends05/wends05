# Agent instructions

<!-- FILL: one line on what this project is and who it is for. -->

## Read first

Start with [docs/README.md](docs/README.md), then read the documents relevant to the task before editing. Check [docs/intent.md](docs/intent.md) before choosing what to build or how it should behave. Use the words defined in [docs/glossary.md](docs/glossary.md) in code, docs, and conversation.

The docs describe direction, conventions, and decisions, not what is implemented today. Read the code for current behavior. Update the docs when a convention, plan, or decision changes; do not add implementation status or check results to them.

## Commands

<!-- FILL: the package manager and the real scripts. Keep this list identical to docs/development.md. -->

```bash
# install
# dev
# check      (format, lint)
# typecheck
# test
# build
# verify     (all of the above; nonzero if any fail)
```

`verify` is the done gate. A change is not done while it fails, even when the cause predates the change.

## Task recipes

<!-- FILL: one numbered runbook per repeatable task (add a page, add content, add a migration). Delete this section if there are none. -->

## Rules

- Do not edit generated files by hand: <!-- FILL: paths, and the command that regenerates them -->
- Keep these boundaries: <!-- FILL: server/client, layer, or feature-folder rules, and where they are documented -->
- Never print or commit the contents of `.env`.
- Don't push to the default branch; all changes go through pull requests. Branches are `<type>/<short-name>` and PR titles are conventional commits. See [docs/workflow.md](docs/workflow.md#git-workflow).

## Skills

<!-- FILL: skill name -> when to use it. Skills that must be present for this repo to work are vendored under .claude/skills/. -->

## Workflow

- Read [docs/workflow.md](docs/workflow.md) before planning substantial work. Plan in chat; record significant architectural decisions in [docs/decisions/](docs/decisions/README.md) and product decisions in [docs/intent.md](docs/intent.md).
- Record actual owner acceptance and implementation authorization; never infer acceptance from an agent-written status. Once authorized, continue routine work within scope without repeatedly asking permission.
- Define observable acceptance criteria, inspect relevant source, and update the plan and affected docs when the approach changes.
- Report actual verification results, existing failures, regressions, and checks not run before reporting completion.
