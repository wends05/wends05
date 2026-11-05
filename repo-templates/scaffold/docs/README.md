# Project documentation

These documents help future agents and collaborators understand the project before changing it.

They describe where the project is going and how to build it: direction, conventions, and decisions. They do not track what is implemented today; read the code for that.

## Read by task

| Document | Read when |
| --- | --- |
| [Product intent](intent.md) | Deciding what to build, choosing between options, or checking whether a change fits the project's goals |
| [Development workflow](workflow.md) | Planning a substantial change, recording acceptance, selecting verification, or reporting completion |
| [Glossary](glossary.md) | The words the project and its code use |
| [Architecture](architecture.md) | Routes or modules, data flow, and where code goes |
| [Development](development.md) | Setup, commands, checks, CI, generated files, and deployment |
| [Decisions](decisions/README.md) | Recording a significant implementation choice and its rationale |

Read [../AGENTS.md](../AGENTS.md) first. For general orientation, continue through product intent and architecture; read the rest as needed.

## Documentation maintenance

- Update the relevant document in the same change as its code or configuration.
- Reference actual source files and commands. Keep secrets and connection strings out of documentation.
- Write direction, conventions, and rules. Do not record implementation status, placeholders, or check results; those belong in chat or the pull request.
- Keep the product target in `intent.md`, conventions in the topic docs, and rationale in `decisions/`; avoid duplicating source files.
- Change `intent.md` only with the owner's agreement; agents should not invent goals.
- Add new topics to the table above so future agents can discover them.

If the code and a convention here disagree, ask whether to change the code or the doc.
