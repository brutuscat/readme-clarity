# readme-clarity

A human-first skill for creating, restructuring, and reviewing repository READMEs.

The goal is simple: make a repository understandable and usable with the minimum necessary documentation.

## Core idea

A README should give a person the shortest verified path from:

`What is this?`

to:

`I understand whether this matters to me and what to do next.`

That means:

- write for humans, not keyword density;
- keep sections only when they serve a reader outcome;
- prefer concrete examples over abstract feature claims;
- move deep reference material out of the README when appropriate;
- use diagrams when they genuinely reduce cognitive load;
- delete or condense before adding more prose;
- never invent commands, capabilities, requirements, benchmarks, or compatibility claims.

## What the skill does

`readme-clarity` inspects the available project context, identifies the likely reader and primary successful action, then selects only the README structure needed for that project.

It is not tied to open source projects or to one template. It can be used for libraries, CLIs, applications, services, internal repositories, monorepos, infrastructure, prototypes, data or ML projects, plugins, and documentation repositories.

## Install and use in Codex

Clone this repository, then copy the skill into Codex's personal skills directory:

```sh
git clone https://github.com/brutuscat/readme-clarity.git
mkdir -p ~/.agents/skills
cp -R readme-clarity/readme-clarity ~/.agents/skills/
```

Then invoke it in Codex with a README request:

```text
$readme-clarity Rewrite this repository's README for a first-time user.
```

Codex's [skills guide](https://developers.openai.com/codex/skills#where-codex-loads-local-skills) lists `$HOME/.agents/skills` as the user-level discovery directory. Run `/skills` in Codex CLI or the IDE extension to check that `readme-clarity` is listed; if it is missing, restart Codex.

## Human-first checks

For every section:

- What does the reader get from this?
- Can it be deleted or condensed?
- Does it belong in the README or in deeper documentation?
- Would an example explain it faster?
- Would a Mermaid diagram explain the relationship better?

For every paragraph:

- Would a human understand this?
- Is it written as normal prose rather than metadata or keyword stuffing?
- If it is dense, abstract, repetitive, or awkward, can it be expressed more simply?

The skill silently considers multiple simpler formulations when prose needs simplification, while leaving already-clear writing alone.

## Agent Clarity

If [Agent Clarity](https://github.com/brutuscat/agent-clarity) is available, README Clarity can use it selectively as a second pass on operational instructions such as setup, prerequisites, configuration, deployment, validation, and recovery steps.

README Clarity remains responsible for human readability, information architecture, tone, examples, diagrams, and section selection. Agent Clarity is optional; this skill must work fully without it.

## Files

- [`readme-clarity/SKILL.md`](readme-clarity/SKILL.md) — the skill
- [`readme-clarity/examples/before-after.md`](readme-clarity/examples/before-after.md) — examples showing different README structures

## Origin

This project started from [0xelitesystem/oss-readme-template](https://github.com/0xelitesystem/oss-readme-template). Its strongest ideas remain here: plain descriptions, useful examples early, honest limitations, progressive disclosure, and deleting sections that do not earn their place.

README Clarity generalizes those ideas beyond OSS and turns them into a human-first documentation skill rather than a fixed template.

## License

MIT. See [LICENSE](LICENSE).
