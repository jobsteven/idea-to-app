# idea-to-app

[English](README.md) | [中文](README.zh.md)

You've got an idea for an app. You can't code. Until recently, that was the end of the story.

**idea-to-app** is a skill that walks you from that idea to a working, shippable app in seven steps, with an AI agent doing the typing. You make the calls at every step; it does the work. You finish with something real in your hands, plus a folder of docs showing how you got there.

It runs in Claude Code as a `SKILL.md`, and in every agent that reads `AGENTS.md` — Codex, Cursor, Windsurf, Copilot, Aider, Zed, and 20-odd more. One flow, one source.

## Made by walking the flow

Five small apps, each built start to finish with idea-to-app. All single-file, double-click to run, data kept in the browser.

<table>
<tr>
<td align="center" width="25%"><img src="examples/expense-tracker/screenshot.png" width="190"><br><b>记账 · Expense</b><br><sub>A piggy-bank budget app. The pig frowns when you overspend.</sub></td>
<td align="center" width="25%"><img src="examples/mood-journal/screenshot.png" width="190"><br><b>心情 · Mood</b><br><sub>One face and one line a day; read your month at a glance.</sub></td>
<td align="center" width="25%"><img src="examples/bullethell/bullethell.png" width="190"><br><b>弹幕游戏</b><br><sub>像素风 Bullethell 小游戏</sub></td>
</tr>
</table>

The expense tracker also ships its full paper trail in [`examples/expense-tracker/docs/`](examples/expense-tracker/docs) — the six documents the seven steps produced. Read them top to bottom to see what each step actually yields.

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

Each step writes a document, stops for your OK, and can be reopened later. No jargon anywhere.

## Install

**Claude Code** — clone it into your skills folder, then say "I want to build an app" or run `/idea-to-app`:
```bash
git clone https://github.com/jobsteven/idea-to-app ~/.claude/skills/idea-to-app
```

**Codex, Cursor, Windsurf, and other AGENTS.md tools** — drop the flow into your project root:
```bash
curl -o AGENTS.md https://raw.githubusercontent.com/jobsteven/idea-to-app/main/AGENTS.md
```

**Anything else** — paste `AGENTS.md` into that tool's custom instructions, or hand it over as a prompt when you start.

## License

MIT © 2026 Eric Wong
