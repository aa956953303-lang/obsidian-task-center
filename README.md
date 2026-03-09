# obsidian-task-center

## 中文说明

这是一个面向 OpenClaw 的可复用 skill，用来把 Obsidian 笔记库整理成一套可长期维护的三段式结构：

- **任务中心**：管理任务状态、详情页、归档
- **经验**：沉淀做完后的复盘、踩坑与结论
- **技能**：沉淀以后可重复使用的 SOP、方法和工作流

这套 skill 的重点不是只把目录摆整齐，而是让任务在完成之后，能继续反哺经验和技能，形成长期可复用的知识闭环。

## 中文导航

- [这个 skill 能做什么](#这个-skill-能做什么)
- [包含哪些文件](#包含哪些文件)
- [核心设计思路](#核心设计思路)
- [适用场景](#适用场景)
- [截图导览（中文）](#截图导览中文)
- [English Navigation](#english-navigation)
- [What this skill helps with](#what-this-skill-helps-with)
- [Included files](#included-files)
- [Core design ideas](#core-design-ideas)
- [Suggested usage](#suggested-usage)
- [Screenshots walkthrough](#screenshots-walkthrough)
- [Share / reuse](#share--reuse)
- [License](#license)

## 这个 skill 能做什么

- 搭建或优化 Obsidian 的**任务中心**
- 新增 **经验 / 技能** 目录，让任务与知识沉淀接起来
- 为复杂任务补**详情页**
- 让总览页更适合 Obsidian 的**悬停预览**
- 保守清理无关内容、空目录、旧模板

## 包含哪些文件

- `SKILL.md`：主技能说明
- `references/example-templates.md`：总览页 / 列表页 / 经验页 / 技能页示例
- `references/sample-vault-structure.md`：最小可复制 vault 结构
- `references/sample-task-pack.md`：完整样例任务包
- `references/cleanup-guidelines.md`：清理与归档规则
- `references/README.md`：参考资料索引

## 核心设计思路

1. **三段式结构**
   - 任务中心
   - 经验
   - 技能

2. **优先适配悬停预览**
   - 总览页前面先放紧凑表格
   - 用户不点进去也能先看懂内容概览

3. **任务闭环**
   - 任务不是做完就结束
   - 完成后要检查是否需要沉淀经验 / 技能

4. **保守清理**
   - 空目录和已被替代文件可清
   - 用途不明的页面不要乱删

## 适用场景

当用户要：
- 优化 Obsidian 任务系统
- 新增模板
- 把任务和经验 / 技能连接起来
- 让总览页更适合快速预览

就适合使用这个 skill。

## 截图导览（中文）

### 1. 使用说明

这页定义了整个任务中心的使用规则。
它说明任务应该放在哪里、什么时候需要详情页、任务完成后如何回写到经验和技能文档里。

![使用说明](assets/usage-guide.png)

### 2. 任务总览

这是整个系统的总入口。
顶部概览表格用于快速查看有哪些区域、当前状态如何、最近一次更新时间是什么时候。

![任务总览](assets/task-overview.png)

### 3. 任务总览悬停预览

这张图展示了为什么总览页前面要放紧凑表格。
在 Obsidian 里悬停预览时，前几行会直接影响浏览效率，所以这里优先展示状态信息，而不是写说明文字。

![任务总览悬停预览](assets/task-overview-hover-preview.png)

### 4. 进行中任务

这里记录当前还在推进中的一次性或阶段性任务。
每个任务上面先给一个紧凑总览，下面再放详细字段，并连接到详情页、经验文档和技能文档。

![进行中任务](assets/ongoing-tasks.png)

### 5. 任务详情页

复杂任务不应该永远只停留在列表里。
详情页用来记录背景、步骤、风险、产出、验收标准和复盘，这样后续维护会清楚很多。

![任务详情页 1](assets/task-detail-page-1.png)
![任务详情页 2](assets/task-detail-page-2.png)

### 6. 经验总览

经验区用来沉淀“这次做完学到了什么”。
重点是记录踩坑、问题、做法和结论，方便以后少重复踩坑。

![经验总览](assets/experience-overview.png)

### 7. 技能总览

技能区用来沉淀“以后怎么稳定复用”。
经验更偏复盘，技能更偏 SOP 和标准做法，两者配合起来才完整。

![技能总览](assets/skills-overview.png)

### 8. 技能实际使用

这张图展示了技能文档的实际落地方式。
一个好的技能文档应该能帮助后续任务执行得更快、更稳，而不是只写概念说明。

![技能实际使用](assets/skill-in-practice.png)

### 9. 已完成任务

已完成任务不会直接消失，而是移动到已完成区。
这样一方面可以保留任务轨迹，另一方面也能持续连接到对应产出的经验和技能文档。

![已完成任务](assets/completed-tasks.png)

---

## English Navigation

- [What this skill helps with](#what-this-skill-helps-with)
- [Included files](#included-files)
- [Core design ideas](#core-design-ideas)
- [Suggested usage](#suggested-usage)
- [Screenshots walkthrough](#screenshots-walkthrough)
- [Share / reuse](#share--reuse)
- [License](#license)

A reusable OpenClaw skill for organizing an Obsidian vault into a maintainable three-part workflow:

- **Task Center** — task status, details, archive
- **Experience** — lessons learned, pitfalls, post-task reflections
- **Skills** — reusable SOPs, stable workflows, repeatable methods

This skill is designed for people who want their Obsidian task system to be easy to preview, easy to maintain, and easy to extend over time.

## What this skill helps with

- Build or optimize an Obsidian **task center**
- Add **experience** and **skills** folders to create a knowledge loop
- Link tasks to related experience / skill notes
- Add **detail pages** for complex tasks
- Improve top-of-file summaries for better **hover preview readability** in Obsidian
- Clean up unused or empty parts of a vault carefully

## Included files

- `SKILL.md` — main skill instructions
- `references/example-templates.md` — examples for overview pages and summary tables
- `references/sample-vault-structure.md` — minimal vault structure you can copy
- `references/sample-task-pack.md` — complete sample task pack
- `references/cleanup-guidelines.md` — safe cleanup guidance
- `references/README.md` — reference index

## Core design ideas

1. **Three-part structure**
   - Task Center
   - Experience
   - Skills

2. **Hover-preview-first summaries**
   - Put compact summary tables at the top of overview pages
   - Let users understand a note before opening it

3. **Closed-loop maintenance**
   - A task should not just be marked done
   - After completion, check whether the task should create or improve:
     - an experience note
     - a skill note

4. **Conservative cleanup**
   - Safe to remove empty directories and truly replaced files
   - Do not blindly delete unclear notes or potentially linked pages

## Suggested usage

Use this skill when a user asks to:
- optimize their Obsidian task system
- add reusable templates
- connect tasks with learnings and reusable workflows
- make overview pages easier to scan in hover previews

## Screenshots walkthrough

Below is a visual walkthrough of the structure used in this skill.
The goal is not just to show a folder layout, but to demonstrate how tasks, experience notes, and reusable skills connect into one maintainable workflow.

### 1. Usage guide

This page defines the operating rules of the whole task center.
It explains where ongoing tasks should go, how long-term tasks are separated, when to create detail pages, and how completed tasks should feed back into experience and skill notes.

![Usage Guide](assets/usage-guide.png)

### 2. Task overview

This is the main entry point of the whole system.
Its top summary table is designed for quick scanning: users can immediately see which sections exist, what state they are in, and when they were last updated.

![Task Overview](assets/task-overview.png)

### 3. Task overview hover preview

This screenshot shows the hover-preview effect of the overview page.
Because Obsidian previews the first lines of a note, the top summary table becomes part of the navigation experience, not just decoration.

![Task Overview Hover Preview](assets/task-overview-hover-preview.png)

### 4. Ongoing tasks

This page is used for one-off or phase-based work that is still active.
Each task has a compact overview row at the top, followed by a more detailed record below, including links to detail pages, experience notes, and skill notes.

![Ongoing Tasks](assets/ongoing-tasks.png)

### 5. Task detail pages

Complex work should not stay only in list pages.
Detail pages are used to record background, execution steps, risks, outputs, acceptance criteria, and post-task reflections.
That makes ongoing work much easier to maintain over time.

![Task Detail Page 1](assets/task-detail-page-1.png)
![Task Detail Page 2](assets/task-detail-page-2.png)

### 6. Experience overview

The experience section collects lessons learned from finished work.
These notes focus on practical takeaways: what happened, what failed, what should be remembered, and what should be done differently next time.

![Experience Overview](assets/experience-overview.png)

### 7. Skills overview

The skills section stores reusable workflows, SOPs, and stable methods.
If experience notes are about reflection, skill notes are about repeatability.
This is where one-off work becomes reusable operational knowledge.

![Skills Overview](assets/skills-overview.png)

### 8. Skill in practice

This screenshot shows what a concrete skill note can look like in practice.
A skill note should help future work run faster and more reliably by documenting standard steps, common issues, and execution patterns.

![Skill in Practice](assets/skill-in-practice.png)

### 9. Completed tasks

Completed tasks are moved into an archive-style finished section instead of being deleted.
That keeps the whole workflow traceable, and makes it easy to connect each finished task back to the experience and skill notes it produced.

![Completed Tasks](assets/completed-tasks.png)

## Share / reuse

If you want to share this skill with another OpenClaw setup, the minimum recommended package is:

- `SKILL.md`
- `references/example-templates.md`
- `references/sample-vault-structure.md`
- `references/sample-task-pack.md`
- `references/cleanup-guidelines.md`

## License

MIT
