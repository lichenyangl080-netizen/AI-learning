# Teaching Protocol

本协议规定 AI-native Product Builder 课程如何恢复、教学和形成证据。当前进度只由状态文件决定。

## New Conversation Startup Order

`CURRENT_STATE.md → relevant ABILITY_MATRIX rows → REVIEW_QUEUE.md → relevant current Phase of CURRICULUM.md → PHASE_EXECUTION_PLAN.md → TEACHING_PROTOCOL.md → begin learning / planning`

优先只读取当前任务相关行和段落。需要历史证据边界时再读取 `LEARNING_LOG.md` 或 assessment archive。聊天记忆和模型推断不得覆盖仓库状态。

P0 assessment planning, start, or resume additionally reads `ASSESSMENT_SPEC.md`, then an active run file if one exists. Do not create an assessment run file before formal P0 explicitly starts.

## State and Evidence Semantics

Teaching coverage, capability certification and open verification are different facts:

- 已覆盖且核心机制理解充分：不重复基础理论。
- `ABILITY_MATRIX.md`：只记录可支持的能力结论、置信度与证据边界。
- `REVIEW_QUEUE.md`：保留尚未完成的实践或自然再验证。

因此，“conceptual instruction covered + practical evidence missing”应进入应用或验证，不得仅因 `Not Assessed`、`Not Yet Assessed`、Low confidence 或缺少实践证据而从定义重讲。概念理解也不能自动升级能力等级。

## Default Learning Loop

优先使用：

`现实问题 → 必要时的 task-local diagnosis → 最小完整 mental model → 方案 / Specification → AI-assisted practice → failure / edge case → Debug / Eval / Verify → ownership review → state archive`

保持 `Chapter → Lesson → Section`；一个 Section 尽量解决一个完整问题。避免术语碎片、长时间纯理论和只做局部实现却不理解系统。

### Conditional Diagnosis and Skip Gate

先检查已有仓库证据和当前上下文：

- 足以证明核心机制已理解：直接进入新边界、应用或验证，最多用 1–2 句连接。
- 证据不足且确实需要决定教学深度：使用 1–3 个不泄露答案的简短机制题。
- 暴露局部缺口：只补该缺口；明显错误或新场景迁移失败时才重讲相关基础。

禁止为了课堂感、固定流程或出题本身提问；禁止提问后立即自行回答；禁止新 Phase、项目、Lesson 或对话触发 broad reassessment。诊断只决定教学深度，不替代 runtime、diff、debug 或 Eval 证据。

长期去重包括：局部成功不等于整体成功；build/typecheck/lint pass 不等于 runtime verified；stale result；Schema-valid 不等于 semantically correct；external input is untrusted；retry/idempotency；loading/progress/failure/recovery 基础 UX；deterministic logic 优先使用 code。

## Mental-model-first, Experiment-verified Learning

新机制先建立：为什么存在、责任属于哪层、能保证什么、不能保证什么、信息与控制如何流动。再改变条件暴露假设，例如 timeout、重复触发、乱序、部分成功、runtime data invalid、retry duplicate 或层间成功冲突。

实践优先选择小而高信息密度的真实实验：追踪链路、预测行为、修改关键行、制造失败、检查状态迁移、审查关键 diff、比较预期与实际。Code 是验证理解的实验工具，不是实现量目标。

若多个基础概念自然出现，可做短 Foundation Consolidation，把碎片连接成系统；不得在当前项目不需要时插入完整语言、框架或基础设施课程。最终应能连接：

`concept → product / architecture → code or agent action → runtime behavior → failure → diagnosis → verification`

## AI-assisted Engineering Ownership

AI、搜索、官方文档、Codex 与 coding agents 是默认真实工程环境。学习者不必像无 AI 程序员一样闭卷生成完整 debug path，但必须在关键处承担：

- problem framing、scope、Specification 与 acceptance criteria；
- context gathering、delegation、steering 和对 Agent diagnosis 的质疑；
- responsibility-layer judgment、关键 diff review 与无关修改识别；
- test / Eval 设计、真实运行、失败解释与 requirement change 后的 ownership；
- 最终 accept / reject 判断。

Codex 完成代码、设计或产品不等于学习者掌握。能力升级必须来自可归因的解释、修改、调试、验证、评审或迁移证据。项目交付状态与能力状态分开记录。

## Phase-start Research and Planning

每个新的 major mainline Phase 在正式教学前执行：

1. 读取当前状态、相关 Matrix、Review Queue、Curriculum Phase 和必要历史证据。
2. 查询官方文档、primary sources、当前工程实践、高质量近期实现及必要的产品 / 市场证据。
3. 比较 Curriculum target、learner evidence、current practice 与 project need。
4. 在 `PHASE_EXECUTION_PLAN.md` 形成目标、Learning Delta、项目、里程碑、实践、失败场景、验证/Eval、证据、工具、成本/延迟/可靠性、triggered topics 与 non-goals。
5. 交学习者确认后才开始正式 Phase 教学。

Research & Planning 不是 reassessment，不得静默改写长期 Curriculum。

## Mainline and Support Tracks

当前执行主线是 `P6 → P7 → P8`。P3 capability model 持续贯穿；P4/P5 作为 demand-triggered support tracks。

主线推进不要求每个低编号 support Phase 先形式化 `PASSED`。P3/P4/P5 gap 保留在 `REVIEW_QUEUE.md`，并在真实产品自然需要时补齐。Support evidence 仅在实际产品或当前 mainline Exit Gate 需要时成为 blocking。

同一项目可以产生多个 Phase 的证据，但必须分别归因。P6/P7/P8 的 `Evidence Required` 和 `Exit Gate` 仍必须满足，不得因路线压缩而弱化。

## Teaching Depth and Non-goals

教学深度由以下共同决定：

`Curriculum Target + Current Evidence + Current Project Need`

Supporting topics 只补当前风险所需的最小完整基础，不因 Auth、Security、Database、RAG、MCP、Deployment 等重要就自动扩展为专项课程。若要进入某 Phase 的 Non-goal，必须说明真实项目触发原因。不得追逐框架或热点。

项目优先选择有真实 AI capability、产品判断、视觉/交互状态和用户价值空间的方向。Visual / Interaction 是正式第二学习轴，但学习优先级不等于已有能力。

## Verification and Product Feedback

真实 implementation、runtime behavior、failure / edge case、关键 diff、Eval 与最终产品验收是高价值证据。事实与结构优先使用 code/test/runtime checks；语义和质量可使用 LLM Judge；最终审美、产品价值和高价值主观判断由 Human 验收。单次成功不能证明稳定改善。

用户验证应尽早自然出现；P7 再集中深化 user testing、metrics、rollout、adoption 与 iteration。

## Hard Rules

- Repository state priority.
- No broad phase-entry reassessment after P0.
- AI/Codex allowed; Codex completion is not mastery.
- Teaching coverage prevents repetition but does not certify capability.
- P6/P7/P8 Exit Gates remain evidence-based.
- Frameworks and implementation volume are not curriculum goals.
- Project state and capability state remain separate.
- Structural route changes require audit justification and learner agreement.
- Meaningful deviations are recorded; ordinary lesson adaptation does not rewrite Curriculum.

## Phase 0 Evidence Fidelity

P0 permanently follows `ASSESSMENT_SPEC.md`: preserve Initial / Assisted / Ownership evidence, sufficiency versus confidence, corrections, contradictions, transfer, tool failure and verified/unverified boundaries. Historical assessment evidence may explain the Matrix but cannot override a newer Matrix.
