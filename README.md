# linear-skill

[![Skill Lint](https://github.com/effectorHQ/linear-skill/actions/workflows/lint.yml/badge.svg)](https://github.com/effectorHQ/linear-skill/actions/workflows/lint.yml) [![ClawHub Ready](https://img.shields.io/badge/ClawHub-publish%20ready-E03E3E)](https://clawhub.com) [![Reference Implementation](https://img.shields.io/badge/effectorHQ-reference%20impl-1A1A1A)](https://github.com/effectorHQ) [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)

An [OpenClaw](https://github.com/openclaw/openclaw) skill for managing Linear issues, projects, and cycles via the Linear GraphQL API.

---

## Install

```bash
# Copy to your OpenClaw workspace
cp -r . ~/.openclaw/workspace/skills/linear/

# Or install from ClawHub (once published)
clawhub install linear
```

Then add your Linear API key to your OpenClaw config:

```
LINEAR_API_KEY=lin_api_xxxxxxxxxxxxxxxx
```

Get your key at Linear → Settings → API → Personal API keys.

## What it does

- List and search issues by team, assignee, priority, or status
- Create issues from conversation
- Update issue state, priority, or assignee
- Check sprint progress (active cycle)
- Add comments to issues

## Reference

See [SKILL.md](./SKILL.mdd) for the full command reference and examples.

## Contributing

Issues tagged **good first issue** or **help wanted** are a great place to start. See [effectorHQ contributing guide](https://github.com/effectorHQ/.github/blob/main/CONTRIBUTING.md).

---

## About this repo

`linear-skill` is also the **reference implementation** for effectorHQ — a demonstration of what a well-structured, production-ready OpenClaw skill looks like.

What "reference implementation" means here:

- `SKILL.md` passes `skill-lint` with **zero errors, zero warnings**
- CI uses `skill-lint-action` via the org's reusable workflow
- Description is optimized for ClawHub vector search discovery
- All frontmatter fields are properly filled
- Body has Purpose, When to Use, When NOT to Use, Setup, Commands, Examples, and Notes sections

Use this repo as a template when building your own skill. The [plugin-template](https://github.com/effectorHQ/plugin-template) repo has the scaffolding; this repo shows what a finished skill looks like.

---

MIT License — effectorHQ Contributors
