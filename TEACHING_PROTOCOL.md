# Teaching Protocol

本协议规定 AI-native Product Builder 课程的教学与恢复方式。它约束教学过程，不代表任何课程已经开始。

## New Conversation Startup Order

每次开始教学或恢复学习前，必须按以下顺序读取并判断：

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
## Conditional Phase 0 Assessment Loading

When P0 assessment is being planned, started, or resumed, read:

```text
CURRENT_STATE.md
↓
ABILITY_MATRIX.md
↓
REVIEW_QUEUE.md
↓
Relevant P0 section of CURRICULUM.md
↓
TEACHING_PROTOCOL.md
↓
ASSESSMENT_SPEC.md
↓
Active assessment run state, if one exists
```

Do not create an assessment run file until formal assessment explicitly starts.


禁止只根据聊天记忆、上一段对话印象或模型推测决定教学内容。若聊天记忆与仓库状态冲突，仓库中的状态文件优先。

## Baseline Evidence Loading

In the first P1 startup after P0 completion, when `ABILITY_MATRIX.md` evidence is too terse to determine the teaching delta, when Initial / Assisted / Ownership history matters, or when conceptual-versus-practical scope is ambiguous, read the most recent completed assessment run.

A completed run is historical evidence: it may explain the current Matrix but cannot override an updated Matrix. Do not mechanically reread the entire run report for every lesson; load only when the detailed evidence boundary is needed.

## Project Selection Preference

When multiple projects can provide equivalent curriculum evidence, prefer AI-native products with meaningful visual design, interaction design, state transitions, and frontend craft over pure data-processing or admin-style projects.

Visual Design / Interaction Design / AI-native UX / Design Engineering literacy is a formal long-term secondary learning axis alongside the primary Product / Capability / Workflow / Context / Tool / Eval axis. Confirmed learning priority does not equal confirmed learner capability: no visual or interaction `ABILITY_MATRIX.md` Current Status may change without new evidence.

## Default Lesson Structure

教学应优先遵循：

```text
现实场景
↓
用户先做判断 / First-pass
↓
暴露当前认知与关键缺口
↓
补充最少必要理论
↓
方案设计
↓
AI / 搜索 / 文档 / Codex 辅助实践
↓
主动制造或识别失败
↓
Debug
↓
Eval / Verify
↓
复盘与状态归档
```

禁止长期采用“定义 → 定义 → 术语堆砌 → 很久以后才实践”的教材式教学。

### Section Granularity and Diagnostic Prompts

保持 `Chapter → Lesson → Section` 结构，避免切成大量孤立术语小节；一个 Section 应尽量解决一个完整问题。新内容可先用不预设答案的机制题探测当前任务相关的认知模型。若学习者已能正确解释核心机制，只补必要的专业术语和边界后直接推进；不得重复测试 P0 已有充分证据的能力。学习目标是能判断、能审查 Codex、能验证真实行为，而非为手写代码而手写。

## Mental-model-first, Experiment-verified Learning

For conceptually dense engineering topics, especially when the learner does not yet have strong implementation foundations, teaching should normally build a coherent mental model before relying on large project implementation.

The preferred learning loop is:

```text
System / Mental Model
↓
Adversarial Reasoning
↓
Micro Lab
↓
Foundation Consolidation
↓
Integration
```

### 1. System / Mental Model

First establish why the mechanism exists, where it sits in the system, what responsibility it owns, what problem it solves, and how it connects to surrounding layers.

The learner should first understand questions such as:

- Why does this mechanism or layer exist?
- What responsibility belongs here?
- What responsibility does not belong here?
- What would happen if this layer disappeared?
- What can this mechanism guarantee?
- What can it not guarantee?
- How does information or control flow through the surrounding system?

Prefer system relationships, scenarios, architecture diagrams, request flows, state flows, and concrete examples over beginning from isolated syntax or framework vocabulary.

Do not begin primarily from API syntax when the underlying responsibility or system problem has not yet been understood.

For example:

- Do not introduce React state primarily as `useState` syntax. First establish why ordinary variables are insufficient for representing UI state and why some state changes must participate in rendering.
- Do not introduce TypeScript primarily as interface/type syntax. First establish what compile-time checking can guarantee, what it cannot guarantee, and why runtime data can still violate a TypeScript type.
- Do not introduce HTTP primarily as a list of methods and status codes. First establish the Browser / Client / Server communication boundary and the lifecycle of a real request.

### 2. Adversarial Reasoning

Once an initial mental model exists, deliberately vary scenario conditions to expose hidden assumptions, missing boundaries, and incorrect generalizations.

Examples include:

- What if the request times out?
- What if the user triggers the same action twice?
- What if the Model succeeds but the Server fails afterward?
- What if the Server succeeds but the Browser disappears?
- What if the response arrives out of order?
- What if returned JSON is syntactically valid but violates the expected structure?
- What if TypeScript accepts the code but runtime data is wrong?
- What if the user closes the page while server-side work continues?
- What if retry creates duplicated work?
- What if one layer reports success while the overall user-visible operation still fails?

The purpose of these questions is not quiz scoring or reassessment. The purpose is to refine the learner's mental model.

Prefer:

```text
initial judgment
→ changed condition
→ contradiction or gap
→ explanation
→ revised model
```

over repeated definition questions.

### 3. Micro Lab

Use compact real-code experiments to verify important mental models. Micro Labs should normally be much smaller than full project implementation.

Prefer high-information-density experiments such as:

- trace one request through a small codebase;
- identify which code runs in Browser versus Server;
- predict runtime behavior before execution;
- change several meaningful lines;
- deliberately return HTTP 500;
- delay a response;
- remove or rename a returned field;
- create malformed runtime data;
- trigger an action twice;
- inspect loading / success / error state transitions;
- compare expected behavior with observed behavior;
- inspect a small diff produced by Codex; and
- identify which layer should be modified for a changed requirement.

The learner does not need to manually write large amounts of boilerplate code to make the experiment valuable. Codex and other coding agents may normally assist implementation.

However, the learner should retain responsibility for:

- predicting important behavior;
- understanding the relevant responsibility layers;
- explaining why the experiment behaves as observed;
- identifying meaningful changes;
- reviewing important diffs;
- changing key behavior when requirements change; and
- verifying the final result.

Code should function as an experimental instrument for validating understanding, not merely as a volume-of-implementation target.

### 4. Foundation Consolidation

Project-triggered and system-triggered learning must not leave programming fundamentals permanently fragmented. After several related concepts have appeared naturally, perform a short Foundation Consolidation step. The purpose is to reconnect previously encountered fragments into an organized structure.

Examples:

- After JavaScript concepts have naturally appeared, consolidate relationships among variables, functions, objects, arrays, events, async / await, Promise, and errors.
- After React concepts have appeared, consolidate state, events, rendering, props, components, and client interaction.
- After TypeScript concepts have appeared, consolidate type constraints, object shapes, union types, optional fields, compile-time checking, and runtime validation.
- After API work has appeared, consolidate request, response, HTTP status, serialization, client/server boundary, and error categories.

Foundation Consolidation should not become a traditional full programming course inserted before project progress. Do not front-load an entire language or framework curriculum when the current Phase does not require it.

Instead:

```text
encounter concepts naturally
→ understand their role
→ use them
→ periodically organize them into a coherent foundation
```

### 5. Integration

After several mental models have become connected, use a real feature or training project to integrate them. At this stage, the learner should increasingly map an existing conceptual system onto real implementation.

The project should test whether the learner can connect:

```text
concept
→ architecture
→ code
→ runtime behavior
→ failure
→ debugging
→ verification
```

Projects are important integration environments and evidence environments. However, they do not need to be the first entry point for every concept. The learner should ideally enter an integration project with a partial but coherent understanding of how the system is supposed to work, rather than discovering every layer only through local bugs.

## Balance Rules

Maintain the following balance:

- Avoid long theory-only stretches with no contact with real systems.
- Avoid continuous implementation where the learner only fixes local problems without understanding the larger system.
- Prefer fewer, higher-information-density experiments over repetitive coding exercises.
- Real implementation evidence remains required where the Curriculum and Phase Exit Gate require it.
- Conceptual understanding alone does not establish implementation mastery.
- Codex implementation alone does not establish learner mastery.
- Framework/API syntax should normally be introduced after its underlying responsibility or problem is understood.
- Task-local First-pass remains allowed, but it should diagnose the mental model immediately relevant to the current task.
- First-pass must not become repeated broad reassessment.
- Scenario reasoning should be used to expose understanding gaps, not to create unnecessary exam-style questioning.
- When the learner already demonstrates a reliable mental model, do not repeat introductory explanation merely to preserve a fixed lesson format.
- When real runtime behavior contradicts the learner's mental model, prefer investigating the contradiction rather than immediately supplying the answer.

## Cognitive Feedback

Teaching should recognize cognitive feedback as a legitimate form of learning feedback.

Meaningful learning progress may occur when:

- a previously vague system boundary becomes clear;
- multiple isolated concepts become connected;
- a prior assumption is shown to be incomplete;
- the learner can predict a new scenario using the revised model; or
- the learner understands why a mechanism exists instead of only remembering how to invoke it.

Cognitive feedback does not replace implementation evidence. It helps build the model that later implementation and debugging will verify.

## P1 Application

For P1 — AI Product Technical Literacy / Engineering Literacy Foundation, this learning method should normally favor a progression similar to:

```text
Browser / Client / Server / Request lifecycle
↓
JavaScript / Async / error model
↓
React state / rendering / interaction
↓
TypeScript / data contracts / runtime validation
↓
Model API / Structured Output / Streaming
↓
AI UI state / failure / retry / cancellation / concurrency
↓
Tool boundary / deterministic computation
↓
Integrated AI-native Web Feature
```

This is an execution preference, not a replacement for the official P1 Curriculum. The exact P1 Execution Plan must still be produced through the existing Phase-start Research and Planning process using current Curriculum, current Ability Matrix, completed P0 evidence, current external research, and current project needs. Phase-start Research & Planning may refine the order when justified.

P1 should therefore not become either a traditional JS → TS → React → Next.js textbook sequence or a purely reactive project workflow where every concept is learned only because a local implementation broke.

The intended pattern is:

```text
understand the system
→ challenge the model
→ verify with a small real experiment
→ consolidate foundations
→ integrate into the training product
```

## AI and Tool Use

AI、搜索、官方文档、Codex、代码生成与调试工具均属于默认允许的真实工程环境。

如需了解用户的已有判断，可在使用工具前进行简短 First-pass，例如：“你目前会如何判断、设计或排查？”First-pass 仅用于诊断教学起点，不作为闭卷考试，也不得替代真实工程能力证据。

## Codex Completion Is Not Mastery

即使 Codex 完成了代码、设计或完整系统，用户能力等级也不得自动升级。能力升级至少应基于一种或多种真实证据：

- 能解释关键设计选择及其取舍；
- 新需求出现时知道应修改哪一层；
- 能审查关键 diff，识别明显风险或不合理建议；
- 出错时知道从何处开始排查；
- 能判断 Codex 的建议是否合理；
- 能进行测试、验证或 Eval；
- 能在相似但不完全相同的任务中迁移使用。

项目交付状态与用户能力状态必须分开记录。

## Terminology Teaching

- 新术语首次出现且上下文不明显时，使用“英文术语 + 简短中文含义”。
- 不在每节课开头堆砌 glossary；术语在即将频繁使用时引入。
- 已学概念再次出现时，用 1–2 句话回顾；只有明显遗忘或理解错误时才重讲。
- 提问应服务于判断、设计、解释、调试或验证，避免为制造课堂感而连续提问基础定义。

## Phase-start Research and Planning

Before beginning each major curriculum Phase after P0, perform a dedicated Phase-start research and planning step before formal instruction begins. A major Phase means P1, P2, P3, and later Phases; this rule does not apply to every lesson, submodule, or ordinary project iteration.

The Phase-start process must:

1. Read the current repository state, including `CURRENT_STATE.md`, `ABILITY_MATRIX.md`, `REVIEW_QUEUE.md` when relevant, the relevant `CURRICULUM.md` section, and prior-phase evidence when needed.
2. Research current external information relevant to the Phase. Prefer authoritative and up-to-date sources: official documentation, primary technical sources, current engineering practices, high-quality recent open-source implementations, and recent product or job-market evidence when it materially helps planning.
3. Compare Curriculum targets, current learner evidence, current technology/practice, and current project needs.
4. Produce a Phase Execution Plan before formal teaching begins.

The Phase Execution Plan should cover, when relevant:

- Phase objective;
- Learning Delta;
- training product / project;
- capability sequence and major milestones;
- implementation practice, debugging / failure scenarios, and verification / testing / Eval;
- required evidence;
- tools / frameworks;
- cost / latency / reliability considerations;
- triggered topics; and
- explicit non-goals.

Present the Phase Execution Plan to the learner for confirmation before formal Phase instruction begins.

Phase-start research may update execution details, examples, tools, frameworks, and teaching sequence based on current information. It must not silently redesign the long-term Curriculum; structural route changes require explicit justification and learner agreement.

Phase-start Research & Planning is not reassessment. Reuse existing `ABILITY_MATRIX.md` and completed assessment evidence; do not rebuild the learner baseline merely because a new Phase begins. Task-local First-pass diagnosis may still be used during learning when needed.

For every future major Phase, the process is: Phase research → Phase Execution Plan → learner confirmation → formal Phase learning. Apply this as a generic Phase-start rule; determine current progress only from `CURRENT_STATE.md`, and do not use it to infer or restore a Pre-P1 state.

## No Phase-entry Reassessment After P0

This is a Hard Rule.

Once Phase 0 has been completed, later phases must inherit the existing `ABILITY_MATRIX.md` and completed assessment evidence.

Do not start a new broad capability assessment merely because a new Phase, project, lesson, or conversation begins.

A First-pass after P0 is task-local teaching diagnosis only:

- it should concern the capability immediately needed by the current task;
- it should normally take only a few minutes or less;
- it must not re-test multiple previously assessed domains;
- it must not rebuild the learner baseline or block Phase entry;
- existing verified evidence should be reused instead of re-tested.

A new formal reassessment is allowed only when:

1. the learner explicitly requests reassessment; or
2. repository state explicitly marks an assessment as active.

P1 startup therefore means: select/confirm the P1 training product → begin formal P1 learning. It does not mean “start a P1 capability assessment”.

## Hard Rules

### Phase Exit Gate

不能因为学习时间、课程数量或项目完成进入下一 Phase。必须根据该 Phase 的 `Evidence Required` 与 `Exit Gate` 判断。

### Non-goals Protection

进入每个 Phase 前必须检查对应 `Non-goals`。如果教学内容开始深入 Non-goal，必须明确说明为什么当前项目触发了它。禁止因为某技术有趣、热门或模型建议就自动深入。

### Ability-controlled Teaching Depth

教学深度必须由下列三项共同决定：

```text
Curriculum Target
+
ABILITY_MATRIX Current Evidence
+
Current Project Need
```

已经达到较高能力的内容不能从定义重新讲起。存在 Blocking Gap 时，只补当前任务需要的最小完整基础。

### Hard Rules vs Default Practices

Hard Rules 不可改变：

- GitHub 状态优先；
- AI / 搜索 / Codex 属于默认真实工程环境；
- Codex 完成不等于掌握；
- 能力升级必须有证据；
- Spiral Deepening；
- Phase Exit Gate；
- Framework 不是课程目标；
- 项目状态与能力状态分离。

Default Practices 可适应：课时长度、例子数量、使用模型、项目具体主题、类比方式、练习数量与复习形式。教学可以适应，但不能改变课程哲学。

### Early User Validation

真实用户与产品验证不得只出现在后期。早期阶段在条件允许时可以进行少量目标用户观察、Workflow Feedback 或 Usability Feedback；后期再升级到 Metrics、Repeated Usage、Rollout 与 Adoption。

### Meaningful Deviation Logging

如果正式教学明显偏离计划顺序、跳过某模块、提前引入 Triggered Topic 或改变某 Phase 内容，必须记录原因。正常课堂适应不等于课程改版；只有结构性变化才允许修改 `CURRICULUM.md`。

## Phase 0 Evidence Fidelity

Long-term records must preserve verified and unverified boundaries, evidence origin, and important instability. Teaching starts from `Curriculum Target - Verified Evidence = Learning Delta`, not a label alone. Conceptual understanding does not replace practical operation; recognition or scaffolded answers do not equal independent design, diagnosis, or debugging. Codex/IDE/tool failure is neither learner failure nor verified implementation. Final assessment archive must audit Initial, Assisted, Ownership and transfer evidence, contradictions, corrections, scaffold leakage, missing practice, scenario leakage, tool failure, and historical-project inference. Store transferable capability, not scenario-specific detail.

## Realistic AI-native Coding

Codex and coding agents may normally support diagnosis and implementation. Do not require the learner to generate a complete debug path closed-book like a traditional no-AI programmer. Observe whether the learner can frame the goal, provide relevant context, question agent diagnosis, request evidence, understand key responsibility layers, identify irrelevant changes, review key diffs, run and verify real behavior, and retain ownership after requirement changes.

