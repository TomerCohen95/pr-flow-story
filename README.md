# pr-flow-story

Agent skill for reviewing large (often AI-generated) PRs: **story → top-down before/after flow → where to focus**.

Built for the same workflow described in TomerCode’s “Code review in the AI era” series (part 3): understand the picture first, prioritize design and dependency boundaries, skim leaf details, and ask for a stack of smaller PRs when one mental model is not enough.

## What it produces

1. **PR story** — intent, trigger, happy path, risks  
2. **Mermaid flowcharts** — before and after, top-down  
3. **Focus guide** — what to read line-by-line vs skim  
4. **Split check** — when to use stacked PRs (`stacked-pr-split` / `gh stack`)

## Install

Copy this folder into your agent’s skills directory, for example:

- Claude Code: `~/.claude/skills/pr-flow-story/`
- Cursor / agents: `.agents/skills/pr-flow-story/` or your project’s skills path
- Copilot / others: wherever that product loads `SKILL.md`

The skill file is [`SKILL.md`](./SKILL.md).

## Companion

- [stacked-pr-split](https://github.com/TomerCohen95/stacked-pr-split) — split a mega-change into stacked PRs when this skill says the story does not fit in one review.

## License

MIT — use and adapt freely.
