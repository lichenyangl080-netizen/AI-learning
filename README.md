# AI Product Engineer Learning System

跨对话的 AI Product Engineer 课程、能力证据、项目状态与审计事实源。

## Current Baseline

- Curriculum Version: v1.1.1
- Assessment Spec Version: v1.0.1
- Lifecycle Position: `P0 complete / P1 not started`
- Formal Learning Started: `NO`
- Formal Assessment Active: `NO`
- Phase 0 Assessment Completed: `YES`
- Completed Assessment Run: `ASSESSMENT_RUN_001`

This is an entry summary only. [CURRENT_STATE.md](CURRENT_STATE.md) remains the single source of truth for the current learning lifecycle and next action.

## Core Files

- [CURRICULUM.md](CURRICULUM.md)：学什么、达到多深。
- [TEACHING_PROTOCOL.md](TEACHING_PROTOCOL.md)：教学如何运行。
- [ASSESSMENT_SPEC.md](ASSESSMENT_SPEC.md)：P0 证据如何收集。
- [STATE_PROTOCOL.md](STATE_PROTOCOL.md)：跨对话状态如何维护。
- [AUDIT_POLICY.md](AUDIT_POLICY.md)：何时允许课程路线变化。
- [CURRENT_STATE.md](CURRENT_STATE.md)：唯一当前状态与下一步。
- [ABILITY_MATRIX.md](ABILITY_MATRIX.md)：证据、目标深度、优先级与待验证缺口。
- [REVIEW_QUEUE.md](REVIEW_QUEUE.md)、[PROJECT_STATE.md](PROJECT_STATE.md)、[LEARNING_LOG.md](LEARNING_LOG.md)、[CHANGELOG.md](CHANGELOG.md)：复习、项目、历史与版本记录。

## Startup Order

日常恢复：`CURRENT_STATE.md → ABILITY_MATRIX.md → REVIEW_QUEUE.md → relevant CURRICULUM.md → TEACHING_PROTOCOL.md`。

P0 assessment planning, start, or resume additionally requires `ASSESSMENT_SPEC.md` after `TEACHING_PROTOCOL.md`; an active run state is read afterward only if it exists. Repository state takes precedence over committed history, conversation memory, and model inference.

This public repository stores no private conversations, credentials, API keys, passwords, or full assessment answers.
