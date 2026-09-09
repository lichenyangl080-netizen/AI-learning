# AI-native Product Builder Learning System

跨对话的 AI-native Product Builder 课程、能力证据、项目状态与审计事实源。

## Current State

Curriculum Version: v1.3
Execution Mainline: P6 → P7 → P8
Current Position: P6 Phase-start Research & Planning / Not Yet Confirmed

`CURRENT_STATE.md` is the lifecycle source of truth. `PHASE_EXECUTION_PLAN.md` holds the current Phase route.

## Core Files

- `CURRENT_STATE.md`：当前阶段、阻塞与下一步。
- `PHASE_EXECUTION_PLAN.md`：当前 Phase 的具体执行计划。
- `ABILITY_MATRIX.md`：能力结论、证据边界与待验证缺口。
- `REVIEW_QUEUE.md`：尚未关闭的验证需求。
- `CURRICULUM.md`：长期结构、主线与支撑能力。
- `TEACHING_PROTOCOL.md`：教学和恢复规则。
- `STATE_PROTOCOL.md`、`ASSESSMENT_SPEC.md`、`AUDIT_POLICY.md`：状态、P0 测评与路线审计规则。
- `PROJECT_STATE.md`、`LEARNING_LOG.md`、`CHANGELOG.md`：项目、历史与版本记录。

## Startup Order

日常恢复：`CURRENT_STATE.md → relevant ABILITY_MATRIX rows → REVIEW_QUEUE.md → CURRICULUM global route + relevant current Phase → PHASE_EXECUTION_PLAN.md → TEACHING_PROTOCOL.md → begin current learning / planning`。

只读取当前任务所需的 Matrix 行和 Curriculum 段；需要历史证据边界时再读取 `LEARNING_LOG.md` 或 assessment archive。P0 assessment planning, start, or resume additionally requires `ASSESSMENT_SPEC.md`. Repository state takes precedence over conversation memory and model inference.

This public repository stores no private conversations, credentials, API keys, passwords, or full assessment answers.
