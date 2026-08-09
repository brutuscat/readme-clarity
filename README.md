# oss-readme-template

A battle-tested README structure for open source projects. Skip the AI cliches and the empty "Features" section. Use the structure that actually answers what visitors want to know.

This repo IS the template. Fork or copy `TEMPLATE.md` into your own project's `README.md` and fill in the sections.

## What's in the template

A 12-section structure that handles 95% of OSS repos:

1. **Project name** + one-line description (what it is, in plain words)
2. **The problem** (1-2 sentences, why this exists)
3. **Quick example** (code or output showing it working)
4. **Install** (one command if possible)
5. **Use it** (minimal, runnable usage)
6. **API / CLI reference** (link to dedicated docs if longer than a screen)
7. **What it doesn't do** (set expectations honestly)
8. **Contributing** (link to CONTRIBUTING.md or short note)
9. **Tech / dependencies** (one line)
10. **License**
11. **Related** (companion projects)
12. **Acknowledgments** (optional)

## What's NOT in the template

Sections to delete or keep minimal because they almost always become slop:

- **"Features"** as a bullet list. Show the example instead, it's more convincing.
- **"Why X?"** marketing comparisons. Say what your tool does well, don't trash competitors.
- **Animated GIF showing every feature.** One static screenshot is better.
- **Roadmap** in the README. Use a project board or pinned issue.
- **Sponsor banner above the title.** Put it at the bottom or in the sidebar.
- **"Built with love"** badges. Use them sparingly; they're noise.
- **Long FAQ.** If users keep asking the same thing, fix the docs.

## Files

- [`TEMPLATE.md`](TEMPLATE.md), the README skeleton, ready to copy
- [`example-filled.md`](example-filled.md), the same template filled out for a fictional project
- [`CONTRIBUTING.md`](CONTRIBUTING.md), a minimal contributing template

## Why this exists

Most OSS READMEs fall into two failure modes:

1. **The marketing landing page.** Logo, badges, animated GIF, "Why X is the best Y," buy-now button. Makes you suspicious instead of curious.
2. **The empty stub.** Project name, one sentence, install command, no usage example, no idea what it does.

The middle path is shorter than people think. This template aims for that middle.

## Use it

```bash
curl -O https://raw.githubusercontent.com/0xelitesystem/oss-readme-template/main/TEMPLATE.md
mv TEMPLATE.md README.md
```

Then edit. The sections you don't need, delete. The placeholders, fill in. Don't add sections "for completeness", empty sections are noise.

## More

Part of a catalog of single-file browser tools and plain-language references, all MIT licensed and dependency-free: [0xelitesystem.github.io](https://0xelitesystem.github.io/). Built by [elitesystem.ai](https://elitesystem.ai).

## License

MIT for the template files. Apply whatever license fits your project to the README you generate.

## Related

- [readme-slop-checker](https://github.com/0xelitesystem/readme-slop-checker), audit any README for AI cliches
- [oss-license-picker](https://github.com/0xelitesystem/oss-license-picker), decide which license to use
- [solo-saas-launch-checklist](https://github.com/0xelitesystem/solo-saas-launch-checklist), pre-launch checklist
