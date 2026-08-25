# AI Product Engineer Learning System

这是培养 **AI Product Engineer** 的跨对话课程规范与状态仓库，而不是“只学框架”的资料库。它共同维护课程、能力证据、项目状态和路线审计规则。

## 当前基线

- Curriculum Version: v1.1
- Current Phase: `Phase 0 — PLANNING`
- Formal Learning Started: `NO`
- Formal Assessment Started: `NO`

本次规范升级不代表 Phase 0 已完成，也不代表正式学习或测评已经开始。

## 核心文件

- [CURRENT_STATE.md](CURRENT_STATE.md)：唯一当前学习进度与下一步。
- [ABILITY_MATRIX.md](ABILITY_MATRIX.md)：能力证据矩阵、置信度与待验证缺口。
- [CURRICULUM.md](CURRICULUM.md)：v1.1 职业定位、能力分层与课程骨架。
- [TEACHING_PROTOCOL.md](TEACHING_PROTOCOL.md)：教学流程、First-pass 与工具使用规则。
- [STATE_PROTOCOL.md](STATE_PROTOCOL.md)：跨对话状态职责、冲突优先级与归档规则。
- [AUDIT_POLICY.md](AUDIT_POLICY.md)：每 6 周的路线审计政策。
- [REVIEW_QUEUE.md](REVIEW_QUEUE.md)：需要复习或再次验证的内容。
- [PROJECT_STATE.md](PROJECT_STATE.md)：项目实施状态，不等同于学习能力。
- [LEARNING_LOG.md](LEARNING_LOG.md)：正式学习历史。
- [CHANGELOG.md](CHANGELOG.md)：课程规范与状态结构的版本记录。

## 新对话或恢复学习的读取顺序

```text
CURRENT_STATE.md
↓
ABILITY_MATRIX.md
↓
REVIEW_QUEUE.md（如存在）
↓
CURRICULUM.md 的当前相关部分
↓
TEACHING_PROTOCOL.md
↓
开始本次学习
```

状态冲突时，当前仓库状态文件优先于已提交历史、对话记忆和模型推测。仓库中不得保存敏感个人信息、私人聊天内容、账号信息、API Key、密码或真实私人资料。

## Legacy overview (retained)

这是一个公开的 AI Product Engineer 长期学习状态仓库，也是 ChatGPT 与 Codex 跨对话共享的唯一课程状态源（Source of Truth）。

- ChatGPT 负责教学、讨论、测评和课程决策。
- Codex 负责实践开发，以及必要时维护课程状态文件。
- GitHub 是唯一精确状态源。
- 每个新对话都应优先读取 [CURRENT_STATE.md](CURRENT_STATE.md)。
- 禁止保存敏感个人信息、私人聊天内容、账号信息、API Key、密码或真实私人资料。

## 状态优先级

`GitHub explicit state > long-term memory > conversational inference`

本仓库只保存学习路线、课程状态、能力等级、复习记录和项目学习进度；实际项目代码可位于其他仓库。
