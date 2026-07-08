# idea-to-app

[English](README.md) | [中文](README.zh.md)

带一个不懂技术的人,用 AI 把脑子里的想法,七步做成一个能用、能上线的产品。

一套流程、两种壳,几乎所有 AI 编程工具都能装:给 Claude Code 的 **`SKILL.md`**,和给其余工具(Codex、Cursor、Windsurf、Copilot、Aider、Zed 等 20 多种)的 **`AGENTS.md`**。同一套内容,一个源头。

为想**自己做主**的创业者、产品经理、新手准备:每个决定你拍板,打字交给 AI,走完手里有一个真东西,外加一整套过程文档。

## 七步

| 步骤 | 产出 |
|---|---|
| 1. 需求调研 | `docs/01-user-research.md` |
| 2. 产品设计 | `docs/02-product-design.md` |
| 3. UI/UX 结构(线框) | `docs/03-wireframe.html` |
| 4. 风格设计 | `docs/04-style.md` |
| 5. 技术选型 | `docs/05-tech-spec.md` |
| 6. 开发预览 | 产品本身 |
| 7. 部署上线 | `docs/06-deploy.md` |

每一步都产出一份文档、停下来等你确认、随时能回头改。全程大白话,不甩术语。

## 安装

### Claude Code(作为 skill)
```bash
git clone https://github.com/jobsteven/idea-to-app ~/.claude/skills/idea-to-app
```
然后说一句"我想做个 XX""带我做个产品",或直接 `/idea-to-app` 就能触发。
(只想用在某一个项目里,就克隆到那个项目的 `.claude/skills/` 下。)

### Codex / Cursor / Windsurf / Copilot / Aider / Zed ……(用 AGENTS.md)
这些工具都认 `AGENTS.md`。把本仓库的 `AGENTS.md` 丢到你项目根目录(或全局配置,如 `~/.codex/AGENTS.md`):
```bash
curl -o AGENTS.md https://raw.githubusercontent.com/jobsteven/idea-to-app/main/AGENTS.md
```
然后跟它说"从头帮我做个 XX",它就会照着流程走。

### 其他任何 agent
把 `AGENTS.md` 的内容贴进那个工具的自定义指令/规则里,或开工时当 prompt 发给它。

## 看看效果

`examples/expense-tracker/` 是照着这套流程真跑一遍做出来的:
- `index.html` —— 一个小猪存钱罐记账 App(双击就能用,数据存在浏览器里,刷新不丢)。
- `docs/01`–`06` —— 七步一路产出的那几份文档,原样都在。

从头翻一遍那些文档,就能看清每一步到底产出什么。

## 许可

MIT © 2026 Eric Wong
