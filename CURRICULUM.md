# AI Product Engineer Curriculum v1.1

## 职业定位

目标角色：**AI Product Engineer**。

培养目标不是传统后端专家、ML 研究工程师、AI 基础设施工程师或单一框架专家，而是能够独立完成 AI 原生产品的识别、设计、构建、评估、调试与交付的产品型工程师。路线强调可迁移的长期能力，不随短期框架热点漂移。

## 能力分层

### CORE

这些是长期职业身份的核心能力，应逐步达到跨场景判断与独立交付水平：

- Product Judgment
- AI UX / Human-AI Interaction
- Frontend Engineering
- Workflow Design
- Context Engineering
- Tool / Capability Design
- Eval
- AI-assisted Engineering

### CORE-SUPPORT

这些能力需要有实质工程深度，但不以基础设施专家深度为目标：

- TypeScript
- React
- Skill Design
- Agent Design
- Testing / Code Review
- Integration Engineering
- Reliability Engineering
- Harness 的应用层理解

### SUPPORT

这些能力达到可靠独立交付深度即可：

- JavaScript
- Next.js
- HTTP / API
- Async Programming
- Git
- Backend
- Database / Data Modeling
- Authentication / Authorization
- RAG
- MCP
- Security
- Model Literacy
- Python
- Deployment

### AWARENESS / TRIGGERED

以下不是主线长期专项；仅在产品需求、项目瓶颈或工作场景触发时学习：

- Multi-Agent Systems
- AI Infrastructure
- Kubernetes
- Kafka
- Advanced Distributed Systems
- vLLM Internals
- Model Training
- RLHF
- CUDA / GPU Kernels

## 教学路线原则

课程不得采用机械串行模式：

```text
Skill 学完 → Workflow 学完 → RAG 学完
```

应采用**完整能力闭环 + 多能力螺旋加深**。每个阶段都可以自然涉及产品、前端、工作流、工具、上下文、评估、后端和可靠性，但不同阶段的深度不同。

每个阶段应围绕真实产品问题组织，并明确：

- 当前场景与用户价值；
- 本阶段主能力与辅助能力；
- 最小可交付成果；
- 可观察的能力证据；
- 常见失败模式；
- 进入下一阶段的条件。

AI Product Engineer 必须具备足够工程深度，能解释、修改、诊断和承担系统结果，只是不与传统后端或基础设施专家在底层深度上正面竞争。

## 当前阶段保护

Phase 0 保持为 `PLANNING`。本课程规范升级不开始正式学习、正式测评、能力评级或考试，也不产生学习能力证据。当前权威状态以 [CURRENT_STATE.md](CURRENT_STATE.md) 为准。

## Retained v1.0 phase reference

以下 v1.0 阶段说明作为历史课程骨架保留；其能力分层与定位如与本页 v1.1 内容冲突，均以 v1.1 为准。

## 职业定位

**AI Product Engineer**

### 主攻方向

- AI-native Product / AI UX
- React / Next.js / TypeScript
- Workflow / Agent
- Context Engineering
- Tool Design
- Skill Design
- Agent Harness
- Eval
- Reliability

### 辅助达到独立交付水平

- Application Backend
- Database / Auth
- RAG
- MCP
- Security
- Python

### 暂不作为主攻

- 模型训练
- RLHF
- CUDA / GPU Kernel
- 深入 AI Infrastructure
- 深入分布式系统
- Kubernetes
- vLLM 内部实现

## 学习方法

课程采用“能力闭环 + 螺旋式加深”，禁止采用 `Skill 学完 → Workflow 学完 → RAG 学完` 这种串行知识点路线。各能力从早期就可能出现，只是在不同阶段不断加深。

统一能力等级：

- L0：认识——知道是什么、解决什么问题
- L1：会用——有示例或 AI 协助时能正确使用
- L2：会设计——面对新问题能自主选择和设计方案
- L3：会诊断——遇到失败能定位原因、比较方案并修复
- L4：工程判断——能跨场景迁移，知道什么时候应该使用以及什么时候不应该使用，并可形成可靠、可复用、可评测方案

能力等级不能因为“上过课”自动提升，必须有证据。

## Phase 0 — 能力测评与课程定标

目标：建立真实起点，不从课程假设推断能力。

测评范围：

- Web / 前后端边界
- JavaScript / TypeScript
- React / Next.js
- HTTP / API / JSON
- Promise / async/await
- Git
- Backend 基础
- AI 基本概念
- Structured Output
- Tool Calling
- Workflow
- Agent
- Skill
- RAG
- Product Judgment
- AI UX

输出：

- Ability Matrix v1
- Foundation gaps
- 第一阶段个性化课程密度

## Phase 1 — AI Feature Engineering

目标：理解并实现 `User → Frontend → Server → Model → Structured Result / Streaming → UI`。

核心：

- Model API、Server / Client boundary、Structured Output、Schema / Validation
- Streaming、AI UI state、Context 基础、单 Tool 调用、基础错误处理
- Token / Cost / Latency、早期人工 Eval

Eval 从这一阶段开始，不等到后期。

## Phase 2 — Workflow + AI-native Interaction

目标：从“调用模型”升级为“设计 AI 任务流程”。

核心：

- Deterministic code vs LLM decision
- Sequential Workflow、Prompt chaining、Routing、Parallelization
- Evaluator → Optimizer、Agent Loop 基础、Human-in-the-loop 基础
- Tool execution UI、Progress / Failure / Retry / Approval UX、Tracing 基础

重点能力：判断哪一步应该普通代码、哪一步应该 LLM、哪些步骤固定 Workflow，以及哪些步骤允许 Agent 自主决策。

## Phase 3 — Context & Capability Engineering

这是核心专业阶段之一。

核心：

- Capability decomposition、Context Engineering、Tool Design、Skill Design
- Session、Memory 基础、Harness 基础、Capability Eval

需要能够区分 Prompt、Context、Tool、Skill、Workflow、Agent、RAG、Memory 和普通代码。

Tool 重点：boundary、name、description、input/output schema、error semantics、side effect、permission、token-efficient return。

Skill 重点：Skill vs Prompt、Skill vs Tool、instructions、scripts、resources、examples、progressive disclosure、versioning、evaluation-driven improvement。

Context 核心原则：不是越多越好，而是给模型最少且最高价值的信息。

## Phase 4 — Knowledge / RAG / MCP / Memory

目标：把外部知识、实时能力和长期状态正确接入 AI 系统。

RAG：ingestion、cleaning、chunking、embedding / index、metadata、sparse retrieval、dense retrieval、hybrid retrieval、reranking、permissions、context construction、retrieval eval、failure attribution。

重点不是学习大量 Vector DB 产品，而是能够诊断 index、chunk、query、recall、rerank、metadata 与 generation 问题。

MCP：Host、Client、Server、Tools、Resources、Prompts、Authorization / trust boundary；只要求掌握稳定概念与应用，不背快速变化的协议细节。

Memory 要区分 current context、conversation history、session、long-term memory、application database 与 artifact。

## Phase 5 — Reliable & Secure Agent Product

目标：从“能跑的 Demo”升级成“能够合理失败的产品”。

核心：

- Application backend、API contract、SQL / PostgreSQL 基础、Data model
- Authentication、Authorization、Timeout、Retry / Backoff、Rate limit
- Partial failure、Fallback、Idempotency、Human Approval、Least privilege
- Validation、Guardrails、Prompt Injection、Tool misuse、Observability、Tracing

重点：不能只设计 Happy Path。

## Phase 6 — Long-running Agent & Harness

目标：处理长时间运行、暂停、恢复和跨 Context 任务。

核心：

- short-lived vs long-running task、durable execution、checkpoint、resume、interruption
- long-running state、context compaction、artifact handoff、filesystem / sandbox
- execution environment、Agent Harness 深化、Multi-Agent 基础

Multi-Agent 只在 `单 Agent + Tool / Workflow 已经证明不足` 之后学习；禁止为了复杂而复杂。

## Phase 7 — Eval-driven Engineering & Optimization

Eval 升级为核心专业能力。

核心：

- Dataset design：easy / normal / edge / adversarial / regression cases
- Human grading、Rule / code grader、LLM-as-Judge、Trace-based Eval
- Failure taxonomy、Failure attribution、Regression Eval
- Latency、Cost、Model routing、Context reduction、Cache、Model selection

要求：系统变好必须尽量有证据，而不是“感觉更聪明”。

## Phase 8 — AI Product / Human-AI Interaction 深化

Product 和 AI UX 从 Phase 1 就存在，本阶段提升到高深度。

核心：

- Problem discovery、User workflow、AI opportunity identification、Product scope
- Human-AI interaction、Trust、Uncertainty、Transparency、Controllability
- Override、Undo、Approval、Provenance、User testing、Product metrics
- Staged rollout、Adoption、Iteration

核心判断：先问“是否值得 AI 化”，再问“用什么 Agent 技术”。

## Phase 9 — 独立毕业项目

必须使用一个新的、真实的问题验证迁移能力。

要求：

- 真实用户、真实问题、AI 存在明确价值
- 至少一个外部能力、存在失败风险、可以定义成功指标

完整过程：

`Problem Discovery → User Research → Scope → Architecture → Prototype → V1 → Real Users → Trace/Eval → Failure Attribution → Redesign → V2 → Rollout → Portfolio`

Portfolio 重点展示为什么这么设计、为什么某处不用 AI、Workflow 如何演化、遇到哪些失败、Eval 发现了什么，以及第二版为什么改变，而不是罗列框架名称。

## 贯穿线

### Software Engineering Foundation

逐步补：JavaScript / TypeScript、React / Next.js、HTTP、Async、Node.js、API Design、SQL / PostgreSQL、Auth / OAuth、Git、Testing、Linux 基础、Web Security、基础数据结构。

约占长期学习精力 20%～30%，根据 Phase 0 测评动态调整。

### AI Model Literacy

只达到应用层决策需要：Token、Context Window、Embedding、Sampling、Reasoning、Multimodal、Latency、Cache、Model Selection、Hallucination；不走模型训练主线。

### AI-assisted Software Engineering

允许并鼓励使用 Codex。掌握证据不是“全部手写代码”，而是：

1. 能解释
2. 能修改
3. 能诊断

随着阶段提高，逐渐要求 specification、implementation delegation、review、diff、testing、debugging 与 long-running coding agent management。

### Security

从第一阶段渐进出现：API key、Tool side effects、capability boundaries、RAG/MCP trust boundary、prompt injection、authorization、excessive agency、sandbox、adversarial eval。

## 触发式学习

以下技术禁止因为“热门”提前系统学习：Redis、Queue、Docker、WebSocket、Temporal、LangGraph、专门 Vector DB、Kafka、Kubernetes、vLLM、Fine-tuning、Multi-Agent framework。

只有项目出现真实需求时再加入。原则：**技术必须证明自己值得增加系统复杂度。**

## 项目结构

整个培养过程主要有三类实践：

1. Micro Labs：验证单个能力
2. 一个长期训练产品：Phase 1～8 持续升级
3. 一个独立毕业项目：Phase 9 验证迁移能力

Phase 0 完成前不要自行确定长期项目主题。

## 学习单元基本循环

每个正式学习单元优先采用：

`真实问题 → 学习者先判断 → 暴露认知 → 最少必要理论 → 设计 → 实践 → 制造失败 → 分析 → 修改 → Eval → 复盘`

不采用长时间纯理论堆积后才实践的模式。
