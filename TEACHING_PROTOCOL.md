# Teaching Protocol

本协议规定 AI Product Engineer 课程的教学与恢复方式。它约束教学过程，不代表任何课程已经开始。

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
