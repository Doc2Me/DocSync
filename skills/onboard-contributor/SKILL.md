---
name: onboard-contributor
description: Guide new or returning open-source contributors from their interests and experience to a first meaningful contribution. Use when someone wants to join a project, find a contribution path, choose a suitable first task, learn the contribution workflow, or resume contributing after an absence.
---

# Onboard contributor

## Objective

Help the contributor become an independent, confident participant in the project through an achievable, project-specific contribution. Support code and non-code contributions equally.

## Required dependencies

Read the project configuration before discovering resources. Honor configured locations and selections. For each collection independently, use explicitly selected files when declared; otherwise use all available files in the corresponding folder.

- Read and apply the selected standards in `standards/`.
- Read and use the selected context in `context/`.
- Discover eligible personas, skills and templates in `personas/`, `skills/` and `templates/` respectively. Load relevant definitions, workflows and templates as needed.

Do not rely on fixed filenames or an index file. Do not broaden an explicit selection with default files. Report missing or inaccessible configured resources. Keep project-specific selection in the configuration only.

## Inputs and context

Resolve the target project, contribution scope, current project state and contributor's immediate need. Establish, where relevant:

- Existing skills, project familiarity, experience and interests.
- Preferred contribution type, available time and practical constraints.
- Whether the contributor is new to open source, new to this project, or returning after an absence.
- Current prerequisites, participation rules, access requirements and available contribution opportunities.

Select the most suitable allowed contributor persona. Read each declared ancestor recursively and combine corresponding sections additively, without overrides. Do not assume technical knowledge, administrative authority or prior contribution experience. Ask only questions that materially affect the proposed path; do not repeat information already provided.

## Workflow

1. **Orient.** Explain the project's purpose, relevant teams or components and how contributions are organized. Distinguish project-wide onboarding from the selected team's workflow.
2. **Find a path.** Discover supported contribution types from current project sources. Match the contributor's interests, existing skills, learning goals and constraints to relevant opportunities. If the contributor has not chosen a path, offer a small set of evidence-backed options and explain their differences. Do not assume contribution means writing code.
3. **Establish prerequisites.** Identify official onboarding material, applicable contribution and conduct policies, necessary accounts, permissions, tools, environments, communication channels and guidance. Distinguish required steps from optional recommendations, and explain the purpose of unfamiliar requirements. Never request credentials; use authorized connections and report access gaps.
4. **Find a suitable first contribution.** Consult available project sources such as issue trackers, contribution boards, team channels and documentation. Where an authorized MCP connection is configured, use it as appropriate. Check that a suggested live task is still open, relevant, reasonably bounded and not already claimed or blocked where this can be established. Respect project-specific assignment and participation rules. Do not invent tasks, labels, mentors, response times or guarantees of acceptance. If current opportunities cannot be verified, provide a verified way for the contributor to find or propose one.
5. **Prepare.** Guide the contributor through the minimum necessary setup and any learning required for the chosen task. Use eligible tutorial, explanation, reference or how-to skills for distinct needs when useful; keep the overall onboarding path coherent. Validate procedures, commands and examples according to the applicable standards.
6. **Contribute.** Explain how to coordinate with the relevant team, define the intended change, prepare and check the contribution, and submit it through the actual project workflow. Offer checkpoints and ways to get help when blocked. Provide guidance rather than taking over the contributor's work; do not submit, claim tasks, contact people or modify external state without explicit authorization.
7. **Navigate review.** Explain what happens after submission, how to respond to feedback, how to revise work, and how to recognize completion. Include project-specific credit or recognition practices only when verified. Do not promise review, approval or merging within a particular time.
8. **Continue.** Suggest the next achievable contribution or learning step based on progress. For returning contributors, prioritize verified changes to processes, tooling and expectations since their last participation rather than repeating familiar onboarding.

## Interaction and output

Prefer a progressive, conversational onboarding workflow when the contributor is participating directly. Give a manageable next action and observable checkpoint at each stage, adapt subsequent steps to their progress, and distinguish advice from work actually completed.

When asked to generate onboarding documentation or a plan, return a structured, persona-specific path instead. Include, as applicable:

- Starting point and contribution goal.
- Recommended contribution path and relevant entry points.
- Prerequisites and setup.
- First task or verified method for finding one.
- Preparation, submission, review and completion checkpoints.
- Where and how to ask for help.
- A next step after the first contribution.

Use the configured project format and appropriate allowed templates. Apply relevant documentation-generation skills to individual outputs rather than treating onboarding as an additional Diátaxis documentation type. Return the verification summary required by the applicable standards, including source state, evidence gaps, task freshness and validation results. Do not publish or modify project files unless requested.

## Acceptance criteria

- The path matches the contributor's experience, interests and immediate goal.
- The next action is concrete, achievable and supported by current project evidence.
- Required prerequisites, permissions, coordination and review steps are explicit.
- Code and non-code pathways are supported without assuming a specific platform or contribution process.
- The contributor can recognize progress, find help, and understand how to submit and respond to review.
- Suggested opportunities and claims about project processes are verified or explicitly qualified.
- The contributor retains agency; no unauthorized external action or promise of acceptance is made.

Apply the acceptance criteria of all selected standards before delivery. Identify unresolved critical gaps rather than presenting an unverified path as complete.
