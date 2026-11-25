---
id: diataxis
version: "1.0.0"
---

# Diátaxis standard

## Purpose

Apply Diátaxis to generated technical documentation. Classify the reader's immediate need independently of their persona, project, expertise in other domains, or the subject being documented.

Use one primary documentation purpose per document or independently navigable section. Do not require all four types for every topic.

## Classification

| Reader need | Activity | Mode | Documentation type |
| --- | --- | --- | --- |
| Acquire practical ability | Action | Learning | Tutorial |
| Achieve a specific outcome | Action | Working | How-to guide |
| Consult facts while working | Cognition | Working | Reference |
| Develop conceptual understanding | Cognition | Learning | Explanation |

Ask whether the reader needs to act or understand, and whether they are acquiring or applying knowledge and skill. A reader may move between modes at any time.

Honor an explicitly requested type when compatible with the stated purpose. If the request has multiple independent purposes, separate them into linked outputs or ask which is primary when necessary. Do not silently reclassify solely because the reader has a particular role.

## Requirements by type

### Tutorial

- Define a feasible learning objective and a concrete activity.
- Provide a controlled, reproducible learning path with visible milestones.
- Explain just enough to orient the learner; link to deeper material.
- Prefer a single supported route over a survey of alternatives.
- Distinguish learning success from simply completing the example.

### How-to guide

- Define one practical outcome and its applicability.
- Address a reader with the necessary prerequisites.
- Provide actionable steps and decision points where real situations differ.
- Include a way to confirm the outcome; describe essential recovery or limitations when relevant.
- Do not turn the guide into a lesson or comprehensive product description.

### Reference

- Describe a bounded subject accurately and systematically.
- Reflect the structure of the described system or authoritative contract.
- Use consistent names, entries, types, units and conditions.
- Include applicable defaults, limits, availability and behavior only when supported.
- Keep explanatory digressions and extended procedures separate.

### Explanation

- Define a bounded topic and organize discussion around the concepts and relationships needed to understand it.
- Discuss relevant context, mechanisms, rationale, trade-offs and alternatives.
- Distinguish documented rationale from inference.
- Use examples or diagrams to illuminate concepts, not to create an implicit procedure.
- Do not become an exhaustive reference.

## Cross-cutting rules

- Use the resolved persona for terminology, assumed knowledge, depth and relevance; use the documentation type for purpose and structure.
- Keep references to adjacent material meaningful and accurate; do not invent links.
- Apply [evidence](evidence.md) and [accuracy](accuracy.md) independently of documentation type.
- Follow project formatting and publishing conventions without changing the selected type's purpose.
- Output headings are adaptable to the topic and project; the four types are not mandatory fixed page templates.

## Acceptance criteria

- The primary reader need is identifiable.
- The structure supports that need throughout.
- Irrelevant material is omitted or linked separately.
- The output does not assume the role dictates the type of content.
- The appropriate type-specific requirements are satisfied.

## Canonical references

- [Diátaxis](https://diataxis.fr/)
- [The compass](https://diataxis.fr/compass/)
- [Tutorials](https://diataxis.fr/tutorials/)
- [How-to guides](https://diataxis.fr/how-to-guides/)
- [Reference](https://diataxis.fr/reference/)
- [Explanation](https://diataxis.fr/explanation/)
