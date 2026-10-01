---
name: readme-clarity
description: "Create, restructure, or review repository READMEs as human-first information design. Use when a README is missing, dense, generic, template-driven, keyword-heavy, hard to navigate, or difficult to act on. Keep it simple, focused, outcome-based, and verified. Select only the sections readers need, prefer concrete examples, and use diagrams when they reduce cognitive load. Do not invent project facts."
---

# README Clarity

Use this skill to make repository READMEs understandable and useful to humans.

A README is not a keyword index, marketing landing page, or dump of all project documentation. It should help a person quickly understand what the project is, whether it matters to them, and what to do next.

## Human-First Rule

Write for humans first.

Do not optimize prose for keyword density, search, AI retrieval, completeness, or documentation conventions at the expense of readability.

Use technical terms when they improve precision. Do not repeat them merely for discoverability.

The final question is always:

> Would a human understand this?

## Goals

- Give the reader the shortest verified path from arrival to a useful outcome.
- Explain what the project is in plain language before going deep.
- Prefer concrete examples and observable behavior over feature claims.
- Make the first useful workflow runnable as written when practical.
- Keep only sections that serve a reader need.
- Move deep reference material out of the README when that makes the README easier to use.
- State material limitations, non-goals, and unsupported cases when they affect expectations.
- Preserve useful project-specific terminology, voice, commands, paths, and technical detail.
- Prefer the smallest README that sufficiently explains the project.
- Leave clear writing alone.

## Determine the README Contract

Before drafting, determine:

1. Who is the primary reader?
2. Why did they open this repository?
3. What are the first three to five questions they need answered?
4. What is the primary successful action they should be able to take?

Infer these from repository evidence when possible. Do not ask the user for information that the repository already makes clear.

Examples:

- Library: what it does, whether it solves the problem, installation, first use, important limits.
- CLI: purpose, example, install, common commands, options, important limits.
- Application: purpose, how to run it, configuration, development workflow.
- Service or API: role in the system, local run, interfaces, configuration, dependencies, operations.
- Internal repository: purpose, ownership or context when relevant, setup, common development and deployment workflows.
- Monorepo: purpose, repository layout, setup, shared workflows, where package-specific documentation lives.
- Infrastructure: purpose, architecture, prerequisites, apply or deploy, rollback, environments.
- Prototype or PoC: question being tested, current state, how to reproduce, findings, limitations.
- Data or ML project: purpose, inputs, data or model provenance, reproduction, outputs, limitations.
- Skill or plugin: purpose, when to use it, behavior, examples, boundaries.

These are section candidates, not templates.

## Inspect Before Writing

When repository context is available, inspect enough evidence to understand the project before changing the README.

Useful sources include:

- the existing README;
- manifests and package metadata;
- entry points;
- scripts and commands;
- examples;
- configuration;
- `docs/`;
- tests when they clarify actual behavior.

Distinguish between:

- facts verified from the repository;
- facts explicitly supplied by the user;
- reasonable structural inferences;
- unknowns.

Do not turn unknowns into plausible-sounding claims.

Never invent:

- commands;
- configuration keys;
- supported platforms;
- API behavior;
- dependencies;
- benchmarks;
- compatibility;
- deployment behavior;
- security properties;
- project status.

## Select Sections From Reader Needs

Start from zero. Add a section because the reader needs it, not because READMEs usually contain it.

Common candidates include:

- project description;
- problem or context;
- quick example;
- install or setup;
- usage;
- architecture;
- configuration;
- API or CLI reference;
- repository layout;
- development workflow;
- deployment or operations;
- limitations or non-goals;
- contributing;
- license;
- related documentation.

Delete empty, redundant, ceremonial, or low-value sections.

Do not require `Features`, `Roadmap`, `FAQ`, `Contributing`, `License`, `Acknowledgments`, screenshots, badges, or any other conventional section unless it helps the intended reader.

## Choose the Clearest Form

For each piece of information, choose the form that helps the reader understand it fastest.

Use:

- prose for concepts and context;
- runnable examples for behavior;
- steps for actions;
- tables for compact comparison or reference;
- links for deep material that does not belong inline;
- Mermaid for relationships, architecture, state, ownership, or non-trivial workflows.

Prefer demonstration before exhaustive explanation.

Do not turn a simple sequence into a diagram merely to make the README visual.

Use Mermaid when a diagram makes relationships or flow materially easier to understand than prose. Keep diagrams small enough to scan.

## Simplification Pass

For every section, ask:

- What outcome does this section give the reader?
- Can it be deleted?
- Can it be condensed?
- Should it move to deeper documentation?
- Would an example explain it faster?
- Would a Mermaid diagram explain it better?

For every paragraph, ask:

- Would a human understand this on the first read?
- Is it more abstract than necessary?
- Is it repeating terminology for keyword density rather than meaning?
- Is it carrying more than one idea that should be separated?

If a paragraph is dense, abstract, repetitive, keyword-heavy, or awkward, silently consider at least three simpler formulations that preserve the same meaning and technical accuracy. Use the clearest one.

Do not mechanically rewrite prose that is already clear.

Do not remove useful technical terms, nuance, or human voice merely to make sentences shorter.

## Writing Rules

- Open with a plain description of what the project is.
- Explain why it exists when that context changes how the reader understands or uses it.
- Prefer direct, normal language over promotional language.
- Prefer evidence over adjectives.
- Do not write `fast`, `secure`, `simple`, `production-ready`, `scalable`, or similar claims without evidence when the distinction matters.
- Avoid generic feature lists when a short example demonstrates the value better.
- Avoid marketing comparisons that exist mainly to diminish alternatives.
- Keep commands, identifiers, paths, option names, and syntax exact.
- Keep one stable term for one concept.
- Put prerequisites before the action that requires them.
- Make the first useful example self-contained when practical.
- Use progressive disclosure: README first, deeper docs second.
- State significant limitations honestly.
- Avoid repetition across overview, features, examples, and usage.
- Do not add sections merely for completeness.
- Do not impose a fixed word count or section count.

## Optional Agent Clarity Pass

If Agent Clarity is available in the host, use it selectively for operational instructions such as:

- setup steps;
- prerequisites;
- commands;
- configuration procedures;
- deployment instructions;
- validation steps;
- rollback or recovery procedures.

Use it to reduce execution ambiguity, not to rewrite the README's explanatory voice.

README Clarity remains responsible for:

- human readability;
- information architecture;
- section selection;
- narrative explanation;
- examples;
- diagrams;
- progressive disclosure.

Do not depend on Agent Clarity. If it is unavailable, complete the README normally.

## Process

1. Inspect the repository or supplied material and identify verified facts.
2. Determine the primary reader, their first questions, and the primary successful action.
3. Select the minimum section set needed to support that reader journey.
4. Order information from understanding to evaluation to first useful action, then deeper detail.
5. Draft or restructure while preserving useful project-specific content and voice.
6. Run the section and paragraph simplification pass.
7. Apply Agent Clarity selectively to operational instructions when available.
8. Validate examples, commands, paths, links, prerequisites, claims, and limitations against available evidence.
9. Perform a final human read.

## Human Read

Read the result as someone who did not build the project.

Ask:

- Do I understand what this is?
- Do I understand why I might care?
- Do I know what to do next?
- Can I reach the first useful outcome without guessing?
- Are unfamiliar concepts explained before they are relied upon?
- Are examples concrete enough to teach behavior?
- Is any important limitation hidden?
- Is anything repeated?
- Is any paragraph written like metadata rather than communication?
- Would I actually read every section that remains?
- Would a human understand this?

If the answer to the last question is no, simplify again.

## Output

When asked to create or rewrite a README, return the finished README by default.

When asked to review a README, report:

- the problem;
- why it matters to the reader;
- the smallest useful correction.

Do not produce a mechanical style audit unless the user asks for one.

When important facts are missing, omit unsupported claims or identify the missing information. Do not hide uncertainty behind confident prose.

## Boundaries

Use this skill for repository READMEs and closely related top-level repository documentation.

Do not use it as:

- a fixed README template;
- a generic marketing-copy generator;
- an SEO or keyword-density optimizer;
- a replacement for complete product documentation;
- a reason to move every design detail into the README;
- a general prose polisher unrelated to repository documentation.

Do not change project behavior to make the README easier to explain.

If the existing README already serves its readers well, make only changes that materially improve comprehension or successful use.

## Examples

See `examples/before-after.md` for examples across different repository types.
