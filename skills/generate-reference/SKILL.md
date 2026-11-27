---
name: generate-reference
description: Generate structured factual reference documentation. Use for descriptions of interfaces, components, settings, terms, supported behavior, policies, or other bounded entities that readers consult while working.
---

# Generate reference

## Objective

Provide authoritative, systematically organized facts for consultation.

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

1. Define the entity or collection and establish what counts as in scope.
2. Identify the relevant contracts, definitions, configuration, policies and implementation evidence.
3. Extract facts systematically; prefer deterministic extraction if appropriate tooling exists.
4. Choose an organization reflecting the subject and consistent entry schema; do not assume every subject has API fields.
5. Compare descriptions with normative contracts and relevant implementation; label discrepancies.
6. Check completeness within the bounded scope and verify each entry against evidence. Validate included code examples, configuration fragments and commands according to the applicable selected standards.

## Output

Use the project format and adapt headings to the topic. The following is a suggested structure, not a required fixed page template:

- Subject title and brief scope.
- Version and applicability where relevant.
- Systematic entries or tables using consistent applicable fields.
- Conditions, supported values, defaults, constraints and availability where relevant.
- Concise examples only when useful for consultation.
- Related material.

Return the document and the verification summary required by the applicable standards. Record what code validation was performed, its results and any unverified examples or procedures; distinguish static review from execution. Keep provenance traceable and separate from publishable prose where appropriate. Do not publish or modify project files unless requested.

## Type-specific acceptance criteria

- Entries are accurate, consistent and discoverable.
- The documented scope and completeness are explicit.
- Facts, version conditions and limitations are traceable.
- Extended procedures and conceptual digressions are kept separate.

Apply the acceptance criteria of all selected standards before delivery. If any critical requirement cannot be met, identify what is missing rather than presenting an unverified result as complete.
