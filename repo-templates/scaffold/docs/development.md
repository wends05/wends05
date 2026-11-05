# Development

Setup, commands, checks, and deployment.

## Local setup

<!-- FILL: package manager, required services, env files. Keep secrets out; point to .env.example. -->

```bash
# install
# dev
```

The dev server runs on port `<port: number>`.

## Available scripts

This is the canonical command list. [../AGENTS.md](../AGENTS.md) repeats it; keep the two identical.

| Command | Configured action |
| --- | --- |
| `<!-- FILL: dev -->` | Development server |
| `<!-- FILL: build -->` | Production build |
| `<!-- FILL: check -->` | Format, lint, import order |
| `<!-- FILL: typecheck -->` | Type check without emitting files |
| `<!-- FILL: test -->` | Test runner, once |
| `<!-- FILL: verify -->` | check, typecheck, test, and build in sequence; nonzero if any fail |

Scripts do not pass `--write`; add it only when you intend to change files.

## Validation

Pick checks that fit the change ([workflow.md](workflow.md#verification-by-change-type)):

```bash
# verify   # everything
# test     # tests only
```

Tests live in `<location: folder and file naming rule>`. Every pull request that changes behavior includes tests.

### CI

<!-- FILL: workflow file, what it runs, runtime versions. -->

`verify` must pass before a change is done. Report results in chat or the PR, not in these docs.

## Generated files

<!-- FILL: each generated file or folder, what produces it, and the command to regenerate. Never edit these by hand. -->

- Keep the lockfile aligned with intentional dependency changes.
- <!-- FILL: import alias rules, e.g. `#/` maps to `src/` -->

## Dependencies

<!-- FILL: update policy (Dependabot or manual), overrides and why, audit command. -->

## Build output and deployment

<!-- FILL: host, which branches deploy, how to reproduce the build locally, and what a push to the default branch does. -->

| Variable | Needed for |
| --- | --- |
| `<name: environment variable name>` | `<purpose: what needs it, and in which environment>` |

Never commit variable values.

After a deploy, confirm the deployment succeeded and the entry page responds.
