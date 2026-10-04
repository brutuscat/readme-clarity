---
name: readme-clarity
description: "Create, restructure, or review repository READMEs as human-first information design. Use when a README is missing, dense, generic, template-driven, keyword-heavy, hard to navigate, or difficult to act on. Keep it simple, focused, outcome-based, and verified. Select only the sections readers need, prefer concrete examples, and use diagrams when they reduce cognitive load. Do not invent project facts."
---

# README Clarity

Use this skill to make repository READMEs understandable and useful to humans.

A README is not a keyword index, marketing landing page, or dump of all project documentation. It should help a person quickly understand what the project is, whether it matters to them, and what to do next.

## Human-First Rule

Write for humans first.

Do not optimize prose for keyword density, search, AI retrieval, completeness, or documentation conventions at the expense of readability. Use technical terms when they improve precision, not merely for discoverability.

The final question is:

> Would a human understand this?

## Goals

- Give the reader the shortest verified path from arrival to a useful outcome.
- Explain what the project is in plain language before going deep.
- Prefer concrete examples and observable behavior over feature claims.
- Make the first useful workflow runnable as written when practical.
- Keep only sections that serve a reader need.
- Move deep reference material out of the README when appropriate.
- State material limitations or non-goals when they affect expectations.
- Preserve useful project terminology, voice, commands, paths, and technical detail.
- Prefer the smallest README that sufficiently explains the project.
- Leave clear writing alone.

## Establish the README Contract

Before drafting, determine:

1. Who is the primary reader?
2. Why did they open this repository?
3. What are the first three to five questions they need answered?
4. What is the primary successful action they should be able to take?

Infer these from repository evidence when possible. Do not ask for information that the repository already makes clear.

Do not impose one structure. A library, CLI, internal service, monorepo, infrastructure repository, PoC, data project, or skill can need very different READMEs.

## Inspect and Verify

When repository context is available, inspect enough evidence to understand the project before changing the README. Useful sources include the existing README, manifests, entry points, scripts, examples, configuration, deeper docs, and tests when they clarify behavior.

Distinguish:

- facts verified from the repository;
- facts supplied by the user;
- reasonable structural inferences;
- unknowns.

Do not turn unknowns into plausible claims.

Never invent commands, configuration keys, supported platforms, API behavior, dependencies, benchmarks, compatibility, deployment behavior, security properties, or project status.

## Select Only Useful Sections

Start from reader needs, not from a template.

Add a section because it helps the reader understand, evaluate, use, contribute to, or operate the project. Delete sections that are empty, redundant, ceremonial, or low-value.

Do not require conventional sections such as `Features`, `Roadmap`, `FAQ`, `Contributing`, `License`, `Acknowledgments`, screenshots, or badges unless they serve the intended reader.

Use progressive disclosure. Keep the first path useful and move deeper reference material to dedicated docs when that improves the README.

## Choose the Clearest Form

Choose the form that explains each piece of information fastest:

- prose for concepts and context;
- runnable examples for behavior;
- steps for actions;
- tables for compact comparison or reference;
- links for deep material;
- Mermaid for relationships, architecture, state, ownership, or non-trivial workflows.

Prefer demonstration before exhaustive explanation.

Do not add a diagram merely to make the README visual. Use Mermaid when it makes relationships or flow materially easier to understand than prose, and keep the diagram small enough to scan.

## Simplification Pass

For every section, ask:

- What outcome does this give the reader?
- Can it be deleted or condensed?
- Should it move to deeper documentation?
- Would an example explain it faster?
- Would a Mermaid diagram explain it better?

For every paragraph, ask:

- Would a human understand this on the first read?
- Is it more abstract than necessary?
- Is it repeating terminology for keyword density rather than meaning?
- Is it carrying more than one idea?

If a paragraph is dense, abstract, repetitive, keyword-heavy, or awkward, silently consider at least three simpler formulations that preserve meaning and technical accuracy. Use the clearest one.

Do not mechanically rewrite prose that is already clear. Do not remove useful technical terms, nuance, or human voice just to make text shorter.

## Writing Rules

- Open with a plain description of what the project is.
- Explain why it exists when that context changes how it is understood or used.
- Prefer direct, normal language over promotional language.
- Prefer evidence over adjectives.
- Do not make claims such as `fast`, `secure`, `production-ready`, or `scalable` without evidence when the distinction matters.
- Avoid generic feature lists when an example demonstrates the value better.
- Keep commands, identifiers, paths, option names, and syntax exact.
- Keep one stable term for one concept.
- Put prerequisites before the action that requires them.
- Make the first useful example self-contained when practical.
- State significant limitations honestly.
- Avoid repetition.
- Do not add sections merely for completeness.
- Do not impose a fixed word count or section count.

## Optional Agent Clarity Pass

If Agent Clarity is available in the host, use it selectively on operational instructions such as setup, prerequisites, configuration, deployment, validation, rollback, and recovery.

Use Agent Clarity to reduce execution ambiguity, not to rewrite the README's explanatory voice.

README Clarity remains responsible for human readability, information architecture, section selection, narrative explanation, examples, diagrams, and progressive disclosure.

Do not depend on Agent Clarity. If it is unavailable, complete the README normally.

## Process

1. Inspect the repository or supplied material and identify verified facts.
2. Determine the primary reader, their first questions, and the primary successful action.
3. Select the minimum section set needed for that reader journey.
4. Order information from understanding to first useful action, then deeper detail.
5. Draft or restructure while preserving useful project-specific content and voice.
6. Run the section and paragraph simplification pass.
7. Apply Agent Clarity selectively to operational instructions when available.
8. Validate examples, commands, paths, links, prerequisites, claims, and limitations.
9. Read the result as someone who did not build the project.

## Human Read

Ask:

- Do I understand what this is?
- Do I understand why I might care?
- Do I know what to do next?
- Can I reach the first useful outcome without guessing?
- Are unfamiliar concepts explained before they are relied upon?
- Is any important limitation hidden?
- Is anything repeated?
- Is any paragraph written like metadata rather than communication?
- Would I actually read every section that remains?
- Would a human understand this?

If not, simplify again.

## Output

When asked to create or rewrite a README, update the applicable `README.md` when a writable repository is available. Return the full Markdown if no writable repository is available or the user explicitly requests it; otherwise, summarize the change.

When asked to review one, show the problem, why it matters to the reader, and the smallest useful correction. Do not produce a mechanical style audit unless requested.

When important facts are missing, omit unsupported claims or identify the missing information.

## Boundaries

Use this skill for repository READMEs and closely related top-level repository documentation.

Do not use it as a fixed template, marketing-copy generator, SEO optimizer, replacement for full product documentation, or general prose polisher.

Do not change project behavior to make the README easier to explain.

If the existing README already serves its readers well, make only changes that materially improve comprehension or successful use.

## Examples

See `examples/before-after.md` for different repository types and structures.
