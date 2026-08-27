# Curriculum Changelog

## Repository consistency — Post-P0 / Pre-P1 state clarification

- Archived the completed P0 baseline state and clarified that P1 has not started.
- Defined current-versus-historical evidence precedence so completed assessment runs explain, but cannot override, a newer Ability Matrix.

## Assessment Spec v1.0.1 — Evidence Fidelity Refinement

- Preserve verified and unverified capability boundaries.
- Distinguish recognition from independent generation and conceptual evidence from practical evidence.
- Preserve Initial / Assisted / Ownership evidence semantics, tool/environment-failure semantics, scenario abstraction, and final evidence-audit requirements.
- Give supported learner corrections priority over mistaken inference.
- Record that Phase 0 completed under `ASSESSMENT_RUN_001` without reconstructing unavailable run metadata.

## Assessment Spec v1.0 — Phase 0 operating specification

- Added adaptive four-stage Phase 0 specification with AI, search, and Codex as normal tools
- Added qualitative evidence dimensions, Minimum Evidence Rule, and no numeric total score
- Defined Confirmed / Provisional / L3 Candidate semantics, blocking gaps, and curriculum routing
- Added fresh-task, metadata, and public-repository privacy rules
- Corrected State Protocol for assessment-before-P1 and conditional ASSESSMENT_SPEC loading
- Distinguish Initial / Assisted / Ownership evidence
- Add Assessor Intervention Policy
- Separate Evidence Sufficiency from Confidence
- Formal assessment has not started; curriculum remains v1.1.1


## v1.1.1 — Curriculum consistency correction

- 删除 CURRICULUM.md 中并存的旧 v1.0 Phase 结构
- 正式建立唯一有效的 P0-P8 v1.1 课程结构
- 恢复 Ability Matrix 的 Target Level 与 Priority
- 修正 Phase 0 Next Action
- 明确长期训练产品在 Phase 0 后选择
- 补充 Phase Exit Gate、Non-goals、Ability-controlled Teaching Depth、Hard Rules / Default Practices、Early User Validation
- Formal Learning / Assessment 仍未开始
- 收窄 Phase 0 主测范围，并区分 `Not Assessed` / `Not Yet Assessed`

## v1.1 — Curriculum operating specification upgrade

- 明确 AI Product Engineer 职业定位与 CORE / CORE-SUPPORT / SUPPORT / AWARENESS 能力分层
- 新增教学协议
- 新增跨对话状态协议
- 新增每 6 周一次的路线审计政策
- 将能力管理改为基于证据，而非课程完成或 Codex 产出
- 固定当前状态为 `Phase 0 — PLANNING`
- 明确 `Formal Learning Started: NO`
- 明确 `Formal Assessment Started: NO`
- 明确本次不开始正式测评

## v1.0.1 — Ability target calibration

- 为 Ability Matrix 增加 `Priority`
- 区分目标深度与职业重心
- 将 TypeScript 调整为 `L3-L4`
- 将 Reliability 调整为 `L3-L4`
- 将 Python 调整为 `L2-L3`
- 将 Deployment 调整为 `L2`
- 明确 AI Infrastructure 为 `L1 / AWARENESS`
- 保持 Product / AI UX / Workflow / Context / Tool Design / Skill / Harness / Eval 等为核心深区
- 未开始 Phase 0 测评

## v1.0

Initial AI Product Engineer curriculum and learning-state architecture.

核心设计：

- AI Product Engineer 职业定位
- AI-native UX / Frontend + Agent Capability / Workflow 为主深度
- 螺旋式能力增长
- GitHub 作为课程唯一精确状态源
- Eval 从早期开始
- Agent Harness 进入核心能力
- Multi-Agent 后置
- Software Engineering Foundation 贯穿
- Phase 0 能力测评作为正式学习第一步

以后只有课程体系发生实质修改才增加版本。
