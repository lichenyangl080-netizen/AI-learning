# AI Product Engineer Curriculum v1.1.1

## 职业定位

目标角色：**AI Product Engineer**。培养目标不是传统后端专家、ML 研究工程师、AI 基础设施工程师或单一框架专家，而是能独立识别、设计、构建、评估、调试与交付 AI 原生产品的产品型工程师。路线强调可迁移的长期能力，不随短期框架热点漂移。

## 能力分层

### CORE

Product Judgment；AI UX / Human-AI Interaction；Frontend Engineering；Workflow Design；Context Engineering；Tool / Capability Design；Eval；AI-assisted Engineering。

### CORE-SUPPORT

TypeScript；React；Skill Design；Agent Design；Testing / Code Review；Integration Engineering；Reliability Engineering；Harness 的应用层理解。

### SUPPORT

JavaScript；Next.js；HTTP / API；Async Programming；Git；Backend；Database / Data Modeling；Authentication / Authorization；RAG；MCP；Security；Model Literacy；Python；Deployment。

### AWARENESS / TRIGGERED

Multi-Agent Systems、AI Infrastructure、Kubernetes、Kafka、Advanced Distributed Systems、vLLM Internals、Model Training、RLHF、CUDA / GPU Kernels 仅在产品需求、项目瓶颈或工作场景触发时学习。

## 全局推进规则

课程采用完整能力闭环与多能力螺旋加深，不采用 `Skill 学完 → Workflow 学完 → RAG 学完` 的机械串行模式。每个 Phase 都必须包含 Objective、Core Capabilities、Supporting Capabilities、Required Practice、Evidence Required、Exit Gate、Non-goals 与 Triggered Topics。

禁止仅按学习时间、课程数量或项目完成推进。只有 Exit Gate 达成才允许进入下一阶段。AI Product Engineer 必须具备足够工程深度，能解释、修改、诊断和承担系统结果，但不与传统后端或基础设施专家在底层深度上正面竞争。

## P0 — Evidence-based AI-native Capability Baseline

### Objective

建立真实能力基线，并确定后续课程密度；当前保持 PLANNING，未开始正式学习或正式测评。P0 不会评估整张 Ability Matrix，延期能力保持 `Not Yet Assessed`。

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

## P1 — AI-native Web & Model Feature

### Objective

交付一个可信的 AI-native Web 功能，理解从用户界面到模型结果再回到 UI 的完整路径。

### Core Capabilities

Frontend Engineering、TypeScript / React / Next.js、HTTP / API、Async、Server / Client Boundary、Model API、Structured Output、Validation、Streaming、AI UI State、基础 Tool Calling、基础 Testing、基础 Eval、Token / Cost / Latency。

### Supporting Capabilities

Git、基础 Backend、错误呈现、可观察的 UI 状态。

### Required Practice

构建一个含结构化结果或流式结果的最小功能，并验证错误、延迟与结果状态。

### Evidence Required

能解释前后端边界与 schema 选择，能修改关键层，并能用最小测试或 Eval 验证结果。

### Exit Gate

可独立完成并诊断一个小型 AI Web 功能的关键路径与常见失败。

### Non-goals

不引入复杂 Agent、RAG、持久队列或基础设施专项。

### Triggered Topics

仅在真实功能需要时引入认证、部署或额外后端能力。

## P2 — Workflow + Tool + AI-native Interaction

### Objective

从单次模型调用升级为可理解、可控制的 AI 任务流程。

### Core Capabilities

Deterministic Code vs LLM、Prompt Chaining、Routing、Parallelization、Workflow、Tool Calling、Basic Agent Loop、Human-in-the-loop、Tracing、Progress / Failure / Retry / Approval UX。

### Supporting Capabilities

状态管理、错误语义、可测试接口与用户反馈设计。

### Required Practice

设计一个含工作流、工具或人工确认的任务流程，并展示正常、失败与重试体验。

### Evidence Required

能判断普通代码、LLM、Tool、Workflow、Agent 与人类确认分别应承担什么。

### Exit Gate

能设计并验证一个不依赖黑箱自主性的可控工作流。

### Non-goals

不因复杂而引入多 Agent；不把所有步骤交给 LLM。

### Triggered Topics

当单 Agent 加 Tool / Workflow 已被证明不足时，才评估 Multi-Agent。

## P3 — Context & Capability Engineering

### Objective

将模型能力设计为边界清晰、上下文高价值且可评估的应用能力。

### Core Capabilities

Capability Engineering、Context Engineering、Tool Design、Skill Design、State / Memory Basics、Application-level Harness Understanding。

### Supporting Capabilities

Schema、权限边界、错误语义、token-efficient return 与 capability Eval。

### Required Practice

拆分一项能力，设计其 context、tool 或 skill 边界，并对失败案例进行诊断。

### Evidence Required

能区分 Prompt、Context、Tool、Skill、Workflow、Agent、RAG、Memory 与普通代码，并解释取舍。

### Exit Gate

能交付一个可复用、可验证且边界明确的应用能力设计。

### Non-goals

Skill 不是最高层抽象；Harness 仅要求应用层理解与诊断，不培养 Agent Runtime / Infra 专家。

### Triggered Topics

脚本、资源、版本化或额外 harness 机制仅在能力复用需求出现时引入。

## P4 — Data / Integration / RAG / MCP / State

### Objective

把外部知识、数据、权限与持久状态可靠地接入 AI 产品。

### Core Capabilities

Integration Engineering、External APIs、API Contracts、Authentication / Authorization、Permissions、Database / Data Modeling、Persistent State、RAG、MCP、Memory。

### Supporting Capabilities

数据清理、检索质量、metadata、错误处理与安全边界。

### Required Practice

接入一项外部能力或数据源，明确合同、权限、失败路径和状态边界。

### Evidence Required

能定位 integration、retrieval、权限或状态问题，并提出可验证的修复。

### Exit Gate

能在真实应用边界内可靠接入外部数据或工具能力。

### Non-goals

MCP 不以协议版本细节为主线；不因学习 RAG 而枚举或深挖所有 Vector DB。

### Triggered Topics

MCP 目标为应用层 L2-L3：会接入、设计边界、实现简单 Server，并理解安全与权限。

## P5 — Production AI Systems

### Objective

将 AI 功能提升为能合理失败、恢复、观测与交付的产品系统。

### Core Capabilities

Validation、Timeout、Retry / Backoff、Rate Limit、Partial Failure、Fallback、Idempotency、Duplicate Execution、Observability、Tracing、Prompt Injection、Tool Misuse、Identity / Privilege、Least Privilege、Memory Poisoning、Capability vs Permission、Human Approval、Checkpoint、Resume、Durability、Sandbox、Deployment、Rollback、Latency / Cost。

### Supporting Capabilities

Backend、Database、Auth、Security、可靠性工程与发布运维基础。

### Required Practice

为一个有副作用或长任务风险的功能设计失败、恢复、审批与回滚路径。

### Evidence Required

能解释风险边界，复现至少一种失败，并验证修复、降级或恢复机制。

### Exit Gate

能交付一个具备明确权限、故障处理与可观察性的生产级 AI 功能。

### Non-goals

Harness 继续作为应用运行环境理解；不深入分布式 Runtime。Multi-Agent 不作为固定必修升级路线。

### Triggered Topics

只有真实长任务、并发或恢复需求才引入专门 durable execution 技术。

## P6 — Eval-driven Improvement & AI-assisted Engineering

### Objective

用证据持续改善 AI 行为与软件质量，并能有效管理 AI 辅助开发。

### Core Capabilities

AI Eval：Dataset、Edge / Adversarial / Regression、Human Eval、Rule / Code Grader、LLM-as-Judge、Trace-based Eval、Failure Taxonomy、Failure Attribution。

### Supporting Capabilities

Software Quality：Unit Test、Integration Test、Regression Test、Code Review；AI-assisted Engineering：Problem Framing、Specification、Context Gathering、Plan、Delegation、Diff Review、Testing、Correction、Debug、Iteration。

### Required Practice

为一个系统创建最小 Eval 集，定位失败归因，并完成一次有证据的改进循环。

### Evidence Required

能审查 AI 生成的 diff、验证改动，并说明指标或案例为何支持该改进。

### Exit Gate

能用 Eval 与软件测试共同证明一个改进优于原方案。

### Non-goals

Codex 写出代码不等于用户掌握；不以“感觉更聪明”替代验证。

### Triggered Topics

模型路由、缓存或复杂 judge 仅在数据和成本信号支持时引入。

## P7 — Product Delivery Studio

### Objective

把工程能力放入真实产品决策、用户验证与渐进交付中深化。

### Core Capabilities

Problem Discovery、User Workflow、AI Opportunity、AI vs Deterministic Automation、Product Scope、Trust、Uncertainty、Controllability、Override、Undo、Approval、Provenance、User Testing、Metrics、Rollout、Adoption、Iteration。

### Supporting Capabilities

前端交互、可靠性、Eval、分析与用户研究。

### Required Practice

围绕真实场景设计并迭代一个产品功能，记录用户反馈、风险与产品指标。

### Evidence Required

能说明为何值得 AI 化、何处不用 AI，以及用户反馈如何改变设计。

### Exit Gate

能完成一次从问题到可验证交付的产品迭代，并基于证据调整方案。

### Non-goals

真实用户验证不能第一次只出现在 P7；早期阶段在条件允许时即可进行轻量验证。

### Triggered Topics

早期可进行少量目标用户观察、Workflow Feedback 或 Usability Feedback；本阶段再深化 Metrics、Repeated Usage、Rollout 与 Adoption。

## P8 — Independent Capstone

### Objective

使用新的陌生问题验证跨场景迁移与独立交付能力。

### Core Capabilities

产品判断、AI UX、工程实现、可靠性、Eval、交付与复盘的综合迁移。

### Supporting Capabilities

研究、架构、外部集成、测试、发布与作品集表达。

### Required Practice

完成 `Problem Discovery → Research → Scope → Architecture → Prototype → V1 → Real Use → Testing / Eval → Failure Attribution → Redesign → V2 → Delivery → Portfolio`。

### Evidence Required

项目须有 Real User / Stakeholder、Real Problem、Meaningful AI Value、External Capability / Data、Failure Risk 与 Measurable Success Criteria。

### Exit Gate

能以真实证据说明设计选择、失败归因、迭代效果与可迁移学习。

### Non-goals

不以框架清单、单次 demo 或 Codex 产出替代迁移能力证明。

### Triggered Topics

仅由 capstone 的真实技术、产品或交付约束决定。
