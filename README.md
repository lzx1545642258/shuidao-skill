# 水导Skill

蒸馏自 B站「水论文的程序猿」（水导，[Space](https://space.bilibili.com/383551518)）的《研究生自救指南》（~9万字）。提炼其完整的决策模型、操作流程、价值观和生存法则，让 AI agent 面对研究生常见的困境时，能按水导的思维框架给出建议和行动指导。

## 这是什么？

这是一个 **Agent Skill**，基于开放的 [Agent Skills 协议](https://agentskills.io/home)，可在任何 skills-compatible 的 AI agent runtime 中运行（Claude Code、Codex、Cursor、OpenClaw、Hermes Agent、CodeBuddy、Workbuddy、Gemini CLI、OpenCode 等 50+ runtime）。

### 它蒸馏了什么？

原指南覆盖了一个研究生读研3年可能遇到的几乎所有问题。本 skill 提取了其中 **agent 可直接执行的 6 个核心决策模块**：

| 模块 | 内容 |
|------|------|
| **毕业目标决策树** | 考公/考编/进厂/读博 怎么选 |
| **选导师评估框架** | 5种导师类型 + 避雷法 |
| **与导师相处操作手册** | 示弱→交好→沟通→莫较真→斗争 |
| **水论文流水线** | 基准模型→模块→缝→实验→发表 |
| **期刊选择与投稿** | 水刊判断、EI会议、返修模板 |
| **三年时间规划** | 研一到研三的里程碑 checklist |

### 目录结构

```
shuidao-skill/
├── SKILL.md                          # 核心 skill 文件（~11k chars）
├── references/
│   ├── 导师类型对比.md               # 5种导师类型详细对比
│   ├── 毕业目标选择决策表.md          # 7种目标优劣对比
│   ├── 学术裁缝操作指南.md            # 水论文的完整流程
│   ├── 期刊分级速查.md                # 核心/普刊/SCI/EI/CCF 分级
│   ├── 论文返修模板.md                # 返修回复信模板+话术
│   ├── 三年时间规划表.md              # 详细时间线甘特图
│   ├── 导师相处详细策略.md            # 五层策略的详细展开
├── README.md
└── LICENSE
```

## 安装

```bash
# 推荐（跨运行时，自动检测你的 agent）
npx skills add lzx1545642258/shuidao-skill
```

或手动克隆到对应目录：

```bash
# Claude Code
git clone https://github.com/lzx1545642258/shuidao-skill.git ~/.claude/skills/graduate-survival-guide/
# Codex CLI
git clone https://github.com/lzx1545642258/shuidao-skill.git ~/.codex/skills/graduate-survival-guide/
# Cursor
git clone https://github.com/lzx1545642258/shuidao-skill.git ~/.cursor/skills/graduate-survival-guide/
# OpenClaw
git clone https://github.com/lzx1545642258/shuidao-skill.git ~/.openclaw/workspace/skills/graduate-survival-guide/
# Hermes Agent
git clone https://github.com/lzx1545642258/shuidao-skill.git ~/.hermes/skills/education/graduate-survival-guide/
```

## 工作原理

当你用任何兼容 Agent Skills 的 AI 助手提问时，如果问题涉及研究生生存相关内容（选导师、被push、发论文、毕业规划等），skill 会自动加载，agent 会按照水导的思维框架来回答。

## 许可

本项目基于 MIT 许可开源。原文《研究生自救指南》版权归 B站「水论文的程序猿」所有，本 skill 仅提炼其方法论，不包含原文可识别的实质性内容。如有侵权，请联系我，我将修改。

## 致谢

- **B站「水论文的程序猿」** — 原文作者，[Space](https://space.bilibili.com/383551518)
- **Agent Skills 生态** — 开放的技能协议让知识可以跨平台流动
