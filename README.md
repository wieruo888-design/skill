# codex-agent-rules

由 [system_prompts_leaks / gpt-6-astra](https://github.com/asgeirtj/system_prompts_leaks/blob/main/OpenAI/Codex/gpt-6-astra.md) 提供。此 skill 为 GPT-6 泄露提示词所做成的 skill 工作流程。

Provided by [system_prompts_leaks / gpt-6-astra](https://github.com/asgeirtj/system_prompts_leaks/blob/main/OpenAI/Codex/gpt-6-astra.md). This skill is a skill workflow created from leaked GPT-6 prompt disclosures.

## 描述

一个可移植的通用型人工智能代理行为层：权限判断、自主性和持久性、工程执行、写作风格和 PR 描述撰写、用户协作以及技能/应用/插件机制。它控制着工作的完成方式，而不会覆盖宿主代理的身份或角色。

## Description

A portable, general-purpose behavioral layer for AI agents: permission judgment, autonomy and persistence, engineering execution, writing style and PR drafting, user collaboration, and skills/apps/plugins mechanics. Governs how work gets done without overriding the host agent's identity or persona.

## 安装 / Install

将 `codex-agent-rules/` 目录放入目标环境的 skills 目录，确保目录内包含 `SKILL.md`。Operit 环境对应路径为 `/sdcard/Download/Operit/skills/`。

## 用法 / Usage

- 启用：`use skill codex-agent-rules`
- 停用：`stop skill codex-agent-rules`

本 skill 为附加行为层，只规范工作的完成方式，不改变加载方的身份、语气与人格。冲突优先级：用户当前指令 > 宿主人格设定 > 本 skill。

## 结构 / Structure

```
codex-agent-rules/
└── SKILL.md
```
