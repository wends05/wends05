# Decision records

Use this folder for implementation choices whose rationale should survive future refactors. Examples include changing the rendering approach, redesigning model relationships, choosing a deployment host, or establishing a visual system.

| Record | Status |
| --- | --- |
| _No records yet._ | |

Do not invent reasons for choices made before these records began; record only the reasons the owner states. Existing architecture is documented in [../architecture.md](../architecture.md). Add each new record to the table above.

Name new records `NNNN-short-topic.md`, starting with `0001`. Use this template:

```markdown
# 0001: Decision title

Date: YYYY-MM-DD
Status: Proposed | Accepted | Superseded

## Context

What concrete problem or requirement led to this choice?

## Decision

What was chosen, and where is it implemented?

## Alternatives

What relevant options were considered, and why were they not chosen?

## Consequences

What benefits, costs, limitations, and follow-up work result?

## Validation

What was checked, and what remains unverified?
```

Add a Mermaid diagram or code example when it clarifies the choice. Mark a record accepted only when the decision has actually been made. Link superseded records to their replacements and update the current topic docs to reflect the implemented behavior.
