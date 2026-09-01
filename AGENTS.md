# aislop documentation

Source for [docs.scanaislop.com](https://docs.scanaislop.com). Mintlify MDX plus `docs.json`.

## Product

- **aislop** is the open-source CLI quality gate for AI generated code (`npx aislop@latest scan`).
- **scanaislop** is the hosted product at [scanaislop.com](https://scanaislop.com): badges, public scans, team gates.
- Do not call the CLI "Scanaislop". Site name is `aislop`.

## Source of truth

Check behavior against `scanaislop/aislop` (CLI) before changing commands, flags, scoring, engines, languages, or CI examples.

Current product facts:

- CLI version: 0.16.0
- 10 language targets: TypeScript, JavaScript, Expo / React Native, Python, Go, Rust, Ruby, PHP, C#, C/C++
- Six engines: format, lint, code-quality, ai-slop, security, architecture (opt-in)
- Deterministic: no LLM in the runtime path
- Default scoring `smoothing` is `5` (changed in 0.15.0)
- Optional Ruff / golangci-lint binaries: run `aislop-tools` after install; package install does not run lifecycle scripts

## Style

- Active voice, second person
- Sentence case headings
- No decorative or generated illustrations. Use commands, tables, and real terminal output.
- No em dashes in page copy. Use a period, colon, or parentheses.
- Code formatting for commands, paths, flags, and rule IDs
- Brand color is emerald `#10b981`, matching scanaislop.com

## Agent surfaces to keep in docs

- `/agents` is the copy-paste page: prompt, skill URL, hooks, AGENTS.md template
- Skill install: `npx skills add scanaislop/skills`
- Skill file: `https://scanaislop.com/.well-known/agent-skills/aislop/SKILL.md`
- Hooks: `npx aislop@latest hook install`
- Handoff: `npx aislop@latest fix --prompt`

## What not to document here

Internal admin, unreleased enterprise-only flows, and cultural "AI slop" jokes that are not about generated code.
