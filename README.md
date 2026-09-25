# codex-agent-rules

由 [system_prompts_leaks / gpt-6-astra](https://github.com/asgeirtj/system_prompts_leaks/blob/main/OpenAI/Codex/gpt-6-astra.md) 提供。此 skill 为 GPT-6 泄露提示词所做成的 skill 工作流程。

Provided by [system_prompts_leaks / gpt-6-astra](https://github.com/asgeirtj/system_prompts_leaks/blob/main/OpenAI/Codex/gpt-6-astra.md). This skill is a skill workflow created from leaked GPT-6 prompt disclosures.

## 描述 / Description

一个可移植的通用型人工智能代理行为层：权限判断、自主性和持久性、工程执行、写作风格和 PR 描述撰写、用户协作以及技能/应用/插件机制。它控制着工作的完成方式，而不会覆盖宿主代理的身份或角色。

A portable, general-purpose behavioral layer for AI agents: permission judgment, autonomy and persistence, engineering execution, writing style and PR drafting, user collaboration, and skills/apps/plugins mechanics. Governs how work gets done without overriding the host agent's identity or persona.

## 说明 / About

本 skill 是一层附加的行为规范，只管「怎么干活」，不改变加载它的 AI 的身份、称呼、语气与人格。写作风格规则仅作用于工程任务与正式产出（过程更新、最终答复、PR、报告），日常闲聊不受约束。

冲突优先级：**用户当前指令 > 宿主人格设定 > 本 skill**。

内容分为 12 个模块：角色与工作方式、权限与自主决定、自主性与持久性、沟通基调与写作风格、技术沟通与 PR、与用户协作、过程更新与最终答复、最终答复与格式、工程执行、Skills 机制、Apps 与 Plugins、环境适配。

## 安装 / Install

将 `codex-agent-rules/` 目录放入目标环境的 skills 目录，确保目录内包含 `SKILL.md`。

- Operit 环境：`/sdcard/Download/Operit/skills/`
- 其他支持 SKILL.md 的环境：放入对应的 skills / agents 目录即可

## 使用方法 / Usage

### 启用

- 在对话中发送 `use skill codex-agent-rules`
- 或在技能列表中打开对应开关

### 触发场景

- 用户要求长流程工程任务、Codex 风格协作
- PR 描述撰写
- skill / plugin / 上下文管理

首次在对话中应用时，AI 会向用户提示一次。

### 停用

- 发送 `stop skill codex-agent-rules`
- 或关闭技能列表中的开关

## 结构 / Structure

```
codex-agent-rules/
└── SKILL.md
```