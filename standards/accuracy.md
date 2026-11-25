---
id: accuracy
version: "1.0.0"
---

# Accuracy standard

## Purpose

Produce information that is correct for the selected software state and honest about what has not been established. Apply [evidence](evidence.md) to every material claim and [Diátaxis](diataxis.md) to the form of output.

## Preconditions

Resolve the project, target version or revision, topic, persona and immediate need. If a choice materially changes correctness and cannot be established from the request or project policy, request clarification. Otherwise state a reasonable, verified assumption.

If the project context is incomplete, discover what is accessible and report gaps; do not manufacture missing project context.

## Validation workflow

1. Establish the scope and freeze the source state where possible.
2. Gather relevant evidence, including project policies and specifications as appropriate.
3. Draft from evidence rather than generating facts from memory and attaching citations afterwards.
4. Verify material claims against their sources; check identifiers, values, defaults, conditions and version applicability.
5. Check for omitted prerequisites, meaningful exceptions, and differences between intended and implemented behavior.
6. Validate code examples and procedures according to the
   requirements in Code and procedure validation.
7. Check persona relevance, terminology, accessibility, project conventions and documentation-type requirements.
8. Report limitations and unresolved gaps separately from the publishable material.

## Code and procedure validation

For every code example, command and procedure:

- Verify syntax, identifiers, signatures, arguments, configuration, dependencies and compatibility against the target version.
- Verify that all necessary prerequisites and setup steps are included.
- Verify that the documented steps are in the correct order.
- Verify that the stated results are supported by evidence.
- Check for unintended side effects and destructive operations.

Prefer static inspection for checks that do not require execution.

When execution is necessary, feasible and authorized:

- Use an isolated test environment and synthetic data.
- Use the target software version and relevant configuration.
- Compare observed results with documented results.
- Do not modify existing software, infrastructure, project data or external state without explicit authorization.

When execution is not possible, perform static validation and report any remaining uncertainty.

Distinguish between static validation and execution validation. Never claim execution that did not occur.

## Requirements

- Preserve exact identifiers, signatures, configuration keys, commands, units and semantics when relevant.
- Distinguish examples from supported interfaces and recommendations from requirements.
- Do not generalize behavior across versions, deployments or platforms without evidence.
- Do not infer design intent, permissions, supported status or compatibility from code alone.
- Avoid promising outcomes that depend on conditions outside verified scope.
- Use clear, accessible language; adapt precision and detail to the persona without distorting facts.
- Never include credentials or sensitive data in examples.

## Freshness

Documentation is current relative to its declared source state, not merely its generation date.

- Resolve the requested target at generation time; record the revision or version actually inspected.
- Prefer current primary sources for that target over stale secondary accounts.
- If the source changes before delivery and the change can affect the output, recheck affected claims or state the newer state was not inspected.
- If freshness cannot be verified, state the inspected version or date and limitation.
- Do not describe unreleased functionality as generally available.

## Validation status

Use one of these outcomes:

| Status | Meaning |
| --- | --- |
| verified | All material claims are supported by appropriate evidence, and all necessary validation checks have passed. |
| qualified | Useful output containing clearly identified uncertainty, unresolved conflicts or necessary validation checks that could not be performed. |
| incomplete | Critical evidence or prerequisites are missing, preventing a trustworthy output. |

These are run-level assessments, not mathematical guarantees.

Execution is not required when static validation provides sufficient evidence. When execution is necessary to establish correctness but cannot be performed, report the limitation and assign the appropriate validation status.

Always distinguish static validation from execution validation.

## Delivery

Return the requested document in the project's format, plus a compact verification summary (separate from the document if needed):

- Documentation type and resolved persona.
- Project and inspected version/revision.
- Evidence references or ledger.
- Validation methods used and their results, including any necessary checks that could not be performed.
- Unresolved gaps or conflicts.
- Validation status.

Do not publish, commit or create a pull request without user authorization. Never label unreviewed generated material as officially approved.

## Acceptance criteria

- Statements are correct within the established scope.
- Sources, revisions, assumptions and uncertainty are traceable.
- Claims of execution and validation reflect work actually performed.
- No material unsupported claim is presented as established fact.
- Output meets the reader's immediate need without sacrificing accuracy.
