---
name: generate-explanation
description: Generate understanding-oriented explanations. Use when the reader wants to understand concepts, architecture, relationships, design decisions, trade-offs or why a system behaves in a particular way.
---

# Generate explanation

## Objective

Develop a coherent mental model of a bounded topic.

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

1. Identify the conceptual question and what the persona already knows.
2. Trace relevant components, relationships, behavior, terminology and design records.
3. Distinguish observed mechanisms from documented design intent and your own inference.
4. Organize the discussion around conceptual relationships, not a sequence of operational steps.
5. Use illustrative examples, comparisons or diagrams only when they clarify the concept.
6. Check each relationship and rationale against evidence; identify alternatives or trade-offs only when justified. Validate code examples, configuration fragments and commands according to the applicable selected standards.

## Output

Use the project format and adapt headings to the topic. The following is a suggested structure, not a required fixed page template:

- Topic title and framing.
- Relevant conceptual background.
- Mechanisms and relationships.
- Rationale, trade-offs or alternatives where supported.
- Illustration or example where useful.
- Implications, limitations and related material.

Return the document and the verification summary required by the applicable standards. Record what code validation was performed, its results and any unverified examples or procedures; distinguish static review from execution. Keep provenance traceable and separate from publishable prose where appropriate. Do not publish or modify project files unless requested.

## Type-specific acceptance criteria

- The reader can explain the topic and its relevant relationships.
- The discussion is coherent and bounded.
- Rationale is not fabricated from implementation alone.
- Examples illuminate concepts without becoming a procedure or exhaustive reference.

Apply the acceptance criteria of all selected standards before delivery. If any critical requirement cannot be met, identify what is missing rather than presenting an unverified result as complete.
