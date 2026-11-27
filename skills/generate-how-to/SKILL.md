---
name: generate-how-to
description: Generate task-oriented how-to guides. Use when the reader already has or can meet prerequisites and needs practical directions to solve a specific problem or achieve a concrete outcome.
---

# Generate how-to guide

## Objective

Enable the reader to accomplish a defined real-world task.

## Required dependencies

Read the project configuration before discovering standards or context. Apply the following rules independently to each collection:

- **Standards:** Use the standards files explicitly selected in the configuration. If no selection is declared, read and apply every file in the DocSync `standards/` folder.
- **Context:** Use the context files explicitly selected in the configuration. If no selection is declared, read and use every file in the project's `context/` folder.

Honor configured locations and selection rules. Explicit configuration takes precedence over folder defaults; do not add default files to an explicitly configured selection. Discover files from the resolved folders rather than relying on fixed filenames or an index file. Report missing or inaccessible configured dependencies and do not silently substitute guessed content.

Keep project-specific selection in the configuration only. Do not require changes to any standard, context file, or skill to select different files.

## Inputs and context

Resolve from the request and project configuration:

- Topic and immediate reader need.
- Project, component and target version or revision.
- Selected persona, including every persona named directly or indirectly in its `extends` field.
- Applicable project context and evidence sources.
- Desired destination or output format, if specified.

Read all context files selected by the dependency rules above. Use their contents and relevant evidence references to establish the project scope, terminology, policies and source state.

For audience adaptation, read the selected persona and all of its ancestors recursively. Combine the content of corresponding sections from every ancestor and the selected persona additively. An omitted section inherits all applicable parent content; a supplied section adds to it. Do not override, replace or give precedence to any parent's content. A persona without `extends` is standalone. Report missing parents or cyclic inheritance and clarify any genuine ambiguity that materially affects the output.

If project context is missing or incomplete, discover accessible primary sources and identify the gaps. Do not manufacture missing project facts. If the request does not fit this documentation type, use Diátaxis and any applicable selected standards to propose an appropriate type or separate outputs.

## Workflow

1. Establish the target outcome, prerequisites, environment and any required permissions.
2. Identify the supported procedure and relevant variations using authoritative project sources.
3. Order actions by actual dependencies; include decision points only where they affect the result.
4. Provide a way to confirm success and note relevant failure recovery or limits.
5. Link supporting reference and explanation rather than embedding a lesson.
6. Check each action against evidence and validate included code, configuration, commands and the procedure's expected outcome according to the applicable selected standards.

## Output

Use the project format and adapt headings to the topic. The following is a suggested structure, not a required fixed page template:

- Action-oriented title.
- Applicability and prerequisites.
- Procedure with relevant decisions.
- Verify the result.
- Relevant recovery or troubleshooting, if needed.
- Related references.

Return the document and the verification summary required by the applicable standards. Record what code validation was performed, its results and any unverified examples or procedures; distinguish static review from execution. Keep provenance traceable and separate from publishable prose where appropriate. Do not publish or modify project files unless requested.

## Type-specific acceptance criteria

- The outcome is specific and verifiable.
- All required prerequisites and actions are explicit.
- Variations and limitations are handled where material.
- The guide is not a tutorial, conceptual essay or exhaustive reference.

Apply the acceptance criteria of all selected standards before delivery. If any critical requirement cannot be met, identify what is missing rather than presenting an unverified result as complete.
