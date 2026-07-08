# idea-to-app

[English](README.md) | [中文](README.zh.md)

Guide a non-technical person from a raw idea to a working, shippable product — in seven steps, with an AI coding agent.

It ships two ways so almost any agent can use it: a **`SKILL.md`** for Claude Code, and an **`AGENTS.md`** for every tool that reads it (Codex, Cursor, Windsurf, Copilot, Aider, Zed, and 20+ more). Same flow, one source.

Built for founders, PMs, and beginners who want to **drive** the build — make every decision — while the agent does the typing, and walk away with a real thing plus a full paper trail of docs.

## The seven steps

| Step | Produces |
|---|---|
| 1. Requirements | `docs/01-user-research.md` |
| 2. Product design | `docs/02-product-design.md` |
| 3. UI/UX wireframe | `docs/03-wireframe.html` |
| 4. Visual style | `docs/04-style.md` |
| 5. Tech stack | `docs/05-tech-spec.md` |
| 6. Build & preview | the app itself |
| 7. Deploy | `docs/06-deploy.md` |

Every step produces a document, pauses for your sign-off, and can be revisited anytime. Plain language throughout — no jargon.

## Install

### Claude Code (as a skill)
```bash
git clone https://github.com/jobsteven/idea-to-app ~/.claude/skills/idea-to-app
```
Then just say "I want to build an app" / "walk me through building X", or run `/idea-to-app`.
(For one project only, clone into that repo's `.claude/skills/` instead.)

### Codex / Cursor / Windsurf / Copilot / Aider / Zed … (via AGENTS.md)
These tools natively read `AGENTS.md`. Drop this repo's `AGENTS.md` into your project root (or a global config like `~/.codex/AGENTS.md`):
```bash
curl -o AGENTS.md https://raw.githubusercontent.com/jobsteven/idea-to-app/main/AGENTS.md
```
Then tell the agent "build me X from scratch" and it will follow the flow.

### Any other agent
Copy the contents of `AGENTS.md` into that tool's custom-instructions / rules, or paste it as a prompt when you start a build.

## See it in action

`examples/expense-tracker/` is a real product built by walking this flow end to end:
- `index.html` — a piggy-bank expense tracker (double-click to run; data persists in the browser).
- `docs/01`–`06` — the exact documents the seven steps produced along the way.

Read the docs top to bottom to see precisely what each step yields.

## License

MIT © 2026 Eric Wong
