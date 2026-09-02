# AI-native Product Builder Curriculum v1.2

## 职业定位

目标角色：**AI-native Product Builder**。目标是发现值得解决的问题，设计产品与体验，组织 LLM / Tool / Workflow / Agent / Context / Data 等 AI 能力，定义质量与 Eval 标准，并借助 Codex、coding agents 与其他 AI agents 将产品真正交付。

主轴是 Product Judgment、AI UX、Workflow、Context、Tool / Capability Design、Eval 与 AI-assisted Engineering。**Visual Design / Interaction Design / AI-native UX / Design Engineering literacy** 是正式长期第二学习轴。Engineering 是必要的 Supporting Literacy：能够理解系统边界、阅读关键实现、判断责任层、审查关键 diff、验证 Agent 交付，并在需求变化时知道修改哪一层；不以脱离 AI 手写大量代码或传统框架熟练度作为长期身份目标。

## 能力分层

### PRIMARY CORE

Product Judgment；AI UX / Human-AI Interaction；Workflow Design；Context Engineering；Tool / Capability Design；Eval；AI-assisted Engineering。

### SECONDARY DESIGN AXIS

Visual Design；Interaction Design；AI-native UX；Design Engineering literacy。

### SUPPORTING ENGINEERING LITERACY

Frontend Engineering；JavaScript；TypeScript；React；Next.js；HTTP / API；Async Programming；Git；Backend；Database / Data Modeling；Authentication / Authorization；Testing / Code Review；Integration；Reliability；Model Literacy；Structured Output；Tool Calling；RAG；MCP；Memory / State；Security；Python；Deployment。

### AWARENESS / TRIGGERED

Multi-Agent Systems、AI Infrastructure、Kubernetes、Kafka、Advanced Distributed Systems、vLLM Internals、Model Training、RLHF、CUDA / GPU Kernels 仅在产品需求、项目瓶颈或工作场景触发时学习。

## 全局推进规则

课程保留 P0–P8 的完整能力闭环与多能力螺旋加深，不采用机械串行学习。每个 Phase 都必须包含 Objective、Core Capabilities、Supporting Capabilities、Required Practice、Evidence Required、Exit Gate、Non-goals 与 Triggered Topics。

禁止仅按学习时间、课程数量或项目完成推进。真实 implementation、runtime verification、关键 diff 审查、系统边界判断与最终产品行为验证仍是必要证据；但工程深度服务于产品与 AI capability ownership，不与传统后端或基础设施专家在底层深度上正面竞争。Product、AI UX、Visual / Interaction Judgment 从早期 Phase 贯穿，并在 P7 集中深化。
## P0 — Evidence-based AI-native Capability Baseline

### Objective

建立真实能力基线，并确定后续课程密度；P0 仅评估明确范围，延期能力保持 `Not Yet Assessed`。

### Core Capabilities

在 AI-native 工程环境中进行观察、研究、设计、构建、解释、修改、调试与验证。

### Supporting Capabilities

问题表达、信息检索、基础 Web / 软件边界与工具协作。

### Required Practice

正式开始后采用 `Observe → Research → Design → Build → Explain → Modify → Debug → Verify` 形成基线；AI、搜索、文档、ChatGPT 与 Codex 均是正常工程环境，不以传统闭卷考试作为主要判断方式。

### Evidence Required

可归档的 First-pass、解释、修改、调试与验证证据；不得由历史聊天、项目经历或 Codex 产出替代。

### Exit Gate

能力矩阵已具备真实的初始证据、置信度与明确缺口，并已确定 P1 的最小学习密度。

### Non-goals

不在本阶段认证 L3 或 L4；不选择长期训练产品；不将工具产出视为用户掌握；不评估整张 Ability Matrix，延期能力保持 `Not Yet Assessed`。

### Triggered Topics

仅按发现的 blocking gap 引入最小必要基础。

## P1 — AI Product Technical Literacy / Engineering Literacy Foundation

### Objective

以一个可信的 AI-native Web 功能建立产品型工程 literacy：理解用户界面、浏览器、服务器、模型结果与 UI 之间的关键路径，并能与 coding agents 一起阅读、修改、运行和验证关键行为。

### Core Capabilities

Browser / Client / Server Boundary、HTTP / API、Async、AI UI State、Streaming、Model API、Structured Output、Validation、基础 Tool Calling、基础 Testing / Eval、Token / Cost / Latency，以及关键实现的 Agent-assisted review 与 verification。

### Supporting Capabilities

JavaScript、TypeScript、React、Next.js、Git、基础 Backend、错误呈现与可观察 UI 状态，作为理解、诊断、修改和验证产品关键路径的 supporting literacy。

### Required Practice

在小型 AI Web 功能或 Micro Lab 中追踪关键请求、状态与失败路径；完成 AI UI state / Streaming、Tool vs deterministic logic、基础 Testing / Eval / Verification，并在 API access 可用时完成一次真实 Model integration。

### Evidence Required

能解释关键系统边界与 schema 选择，能指出需求变化应修改的责任层，能审查 Agent/Codex 的关键改动，并通过运行、失败注入或最小测试 / Eval 验证真实行为。

### Exit Gate

能与 AI agents 一起独立诊断一个小型 AI Web 功能的关键路径与常见失败，并以真实 Provider integration、runtime verification 和产品行为证据说明结果可信。框架熟练度、手写代码量或传统 Web 工程纵深不是单独的 Exit Gate。

### Non-goals

不将 P1 扩展为完整 JavaScript / TypeScript / React / Next.js 课程；不因框架熟练度不足长期阻塞 P1；不引入复杂 Agent、RAG、持久队列或基础设施专项。

### Triggered Topics

认证、部署或额外后端能力仅在真实功能需要时引入，深度以 supporting literacy 和产品风险为界。
## P2 — Workflow + Tool + AI-native Interaction

### Objective

把产品意图拆解为可理解、可控制的 Deterministic Code、LLM、Tool、Workflow、Agent 与 Human Approval 能力结构。

### Core Capabilities

Deterministic Code vs LLM、Prompt Chaining、Routing、Parallelization、Workflow、Tool Calling、Basic Agent Loop、Human-in-the-loop、Tracing，以及 Progress / Failure / Retry / Approval UX。

### Supporting Capabilities

状态语义、错误边界、可测试接口、用户反馈设计与必要的实现 literacy。

### Required Practice

围绕一个真实产品任务设计并验证能力分配、工具边界和人工确认；展示正常、失败、重试与审批体验。

### Evidence Required

能说明每一层为何存在、何处应使用普通代码或模型、何处需要 Tool / Workflow / Agent / 人类控制，并能验证关键体验与失败路径。

### Exit Gate

能交付一个不依赖黑箱自主性的可控 AI workflow，并以产品结果、交互状态与运行证据解释其取舍。

### Non-goals

不把实现 workflow 的代码量当作主要目标；不因复杂而引入多 Agent；不把所有步骤交给 LLM。

### Triggered Topics

只有单 Agent + Tool / Workflow 已被真实证明不足时，才评估 Multi-Agent。
## P3 — Context & Capability Engineering

### Objective

把模型能力设计为边界清晰、上下文高价值、可复用且可评估的产品能力；这是长期主轴之一。

### Core Capabilities

Capability Engineering、Context Engineering、Tool Design、Skill Design、Agent capability boundary、Memory / State Basics 与 application-level Harness understanding。

### Supporting Capabilities

Schema、权限边界、错误语义、context selection / compaction、token-efficient return、capability Eval 与必要实现 literacy。

### Required Practice

拆分一项 AI capability，设计其 context、tool、skill 或 agent 边界，比较替代方案，并对失败案例与上下文质量进行诊断。

### Evidence Required

能区分 Prompt、Context、Tool、Skill、Workflow、Agent、RAG、Memory 与普通代码；能说明能力边界、上下文取舍、失败影响和验证方式。

### Exit Gate

能交付一个可复用、可验证且边界明确的 AI capability design，并用最小实现或 Agent-assisted prototype 验证关键假设。

### Non-goals

不把 Skill 视为最高层抽象；Harness 只要求应用层理解与诊断；不培养 Agent Runtime / Infra 专家。

### Triggered Topics

脚本、资源、版本化或额外 harness 机制仅在能力复用与产品风险需要时引入。
## P4 — Data / Integration / RAG / MCP / State

### Objective

把外部知识、数据、权限与持久状态可靠地接入 AI 产品，并能作出明确的 integration trade-off。

### Core Capabilities

External APIs、API Contracts、Authentication / Authorization、Permissions、Database / Data Modeling、Persistent State、RAG、MCP、Memory 与 Integration Engineering。

### Supporting Capabilities

Source of Truth、Data Ownership、Capability Boundary、Retrieval vs Authoritative Source、Persistent State vs Memory、数据质量、错误处理与安全边界。

### Required Practice

接入一项外部能力或数据源，明确合同、权限、来源、状态、失败路径与用户影响；必要实现可由 agents 辅助，但取舍与验证由学习者承担。

### Evidence Required

能定位 integration、retrieval、权限、来源或状态问题，解释数据和能力边界，并提出可验证的修复或降级方案。

### Exit Gate

能在真实产品边界内可靠使用外部数据或工具能力，并说明为何该方案优于替代方案。

### Non-goals

不以亲自熟练实现所有基础设施组件为目标；MCP 不以协议版本细节为主线；不因学习 RAG 而深挖所有 Vector DB。

### Triggered Topics

MCP 以应用层接入、边界、简单 Server 与安全 / 权限理解为目标，深度由真实需求决定。
## P5 — Trust / Control / Safety / Reliability

### Objective

将 AI 功能提升为可控、可信、可恢复且能向用户解释失败影响的产品系统，而非基础设施专项。

### Core Capabilities

Permissions、Approval、Undo / Rollback、Side Effects、Failure Impact、Recovery、product-level Observability、Tracing、Least Privilege、Capability vs Permission、Identity / Privilege、Human Control、Prompt Injection、Tool Misuse、Memory Poisoning、Validation、Timeout、Retry / Backoff、Rate Limit、Partial Failure、Fallback、Idempotency、Duplicate Execution、Checkpoint / Resume、Durability、Sandbox、Deployment 与 Latency / Cost。

### Supporting Capabilities

必要的 Backend、Database、Auth、Security、Reliability 与 Deployment literacy。

### Required Practice

为有副作用或长任务风险的功能设计权限、审批、失败、恢复与回滚路径，并验证至少一个真实失败或降级场景。

### Evidence Required

能说明谁可执行什么、失败会影响谁、何处需要控制或恢复，并能验证修复、降级或恢复机制在产品层真实有效。

### Exit Gate

能交付一个具有明确控制边界、失败处理、可观察行为与用户可理解反馈的 AI 功能。

### Non-goals

不进入大规模基础设施、分布式 runtime 或 Kubernetes 深度；不将可靠性简化为仅配置重试。

### Triggered Topics

专门 durable execution 技术仅在真实长任务、并发或恢复需求出现时引入。
## P6 — Eval-driven Improvement & AI-assisted Engineering

### Objective

把 Eval 建立为长期核心能力：用产品、AI UX、视觉 / 交互质量、用户证据、回归与失败归因持续改进 AI 产品，并验证 AI-agent 生成的工作。

### Core Capabilities

Dataset、Edge / Adversarial / Regression、Human Eval、Rule / Code Grader、LLM-as-Judge、Trace-based Eval、Failure Taxonomy、Failure Attribution、Product Judgment、UX / Visual Quality Evaluation、Comparison 与 AI-assisted Engineering。

### Supporting Capabilities

Unit / Integration / Regression Test、Code Review、Problem Framing、Specification、Context Gathering、Plan、Delegation、Diff Review、Testing、Correction、Debug 与 Iteration。

### Required Practice

为一个产品系统创建最小 Eval 集，覆盖行为、体验或质量边界；定位失败归因，并完成一次有证据的产品或实现改进循环。

### Evidence Required

能审查 AI 生成的关键 diff、验证改动，说明案例、用户反馈、质量标准或指标为何支持该改进。

### Exit Gate

能用 Eval、软件测试与产品 / UX 证据共同证明一次改进优于原方案。

### Non-goals

不把 Eval 等同于单一模型分数；Codex 写出代码不等于用户掌握；不以感觉替代验证。

### Triggered Topics

复杂 judge、模型路由或缓存仅在数据、产品收益与成本信号支持时引入。
## P7 — AI-native Product & Design Studio

### Objective

把 AI capability、产品判断、AI UX、Visual / Interaction Design 与渐进交付放入真实用户场景中集中深化。

### Core Capabilities

Problem Discovery、User Workflow、AI Opportunity、AI vs Deterministic Automation、Product Scope、Trust、Uncertainty、Controllability、Override、Undo、Approval、Provenance、Visual Design、Interaction Design、Design System Awareness、Taste / Quality Judgment、User Testing、Metrics、Rollout、Adoption 与 Iteration。

### Supporting Capabilities

前端交互、可靠性、Eval、分析、用户研究与 agent-assisted build / verification。

### Required Practice

围绕真实场景设计并迭代一个 AI-native 产品功能，记录用户反馈、视觉 / 交互取舍、风险与产品指标。

### Evidence Required

能说明为何值得 AI 化、何处不用 AI、体验与视觉选择如何服务用户控制，以及用户反馈如何改变设计。

### Exit Gate

能完成一次从问题到可验证交付的 AI-native 产品迭代，并以用户、质量、体验与运行证据调整方案。

### Non-goals

不把 Visual / Interaction 第二轴误解为纯 UI 产出；不以漂亮 demo、框架清单或 Agent 输出替代产品证据。

### Triggered Topics

早期阶段可进行轻量用户观察、Workflow Feedback 或 Usability Feedback；本阶段再深化 Metrics、Repeated Usage、Rollout 与 Adoption。
## P8 — Independent AI-native Product Capstone

### Objective

使用新的陌生问题验证 AI-native Product Builder 的跨场景迁移与独立交付能力。

### Core Capabilities

Problem Discovery、Product Definition、AI Capability Design、Workflow / Context / Tool / Eval、AI UX、Visual / Interaction Design、Agent-assisted Build、Trust / Control、Real Users、Iteration 与 Delivery。

### Supporting Capabilities

研究、架构、外部集成、必要实现 literacy、测试、发布、作品集表达与复盘。

### Required Practice

完成 `Problem Discovery → Research → Scope → Product Definition → AI Capability / UX / Visual Design → Agent-assisted Build → Real Use → Testing / Eval → Failure Attribution → Redesign → Delivery → Portfolio`。

### Evidence Required

项目须有 Real User / Stakeholder、Real Problem、Meaningful AI Value、明确的质量 / Eval 标准、External Capability / Data（如适用）、Failure Risk 与 Measurable Success Criteria。

### Exit Gate

能以真实产品、用户、体验、运行与 Eval 证据说明设计选择、失败归因、迭代效果与可迁移学习；不以手写代码量作为掌握证据。

### Non-goals

不以框架清单、单次 demo 或 Codex 产出替代迁移能力证明。

### Triggered Topics

仅由 capstone 的真实技术、产品、设计或交付约束决定。
