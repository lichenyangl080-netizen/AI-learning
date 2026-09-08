# Ability Matrix

本矩阵同时记录当前可归档证据与计划目标深度。`Current Status` 不得由历史聊天、项目经历、阅读资料或 Codex 产出自动赋值；项目完成与工具产出均不能单独证明掌握。

## Phase 0 Scope

Phase 0 只主测以下范围：Web / Frontend boundary、JavaScript / TypeScript、React / Next.js 基础、HTTP / API、Async、Git、Model Literacy 基础、Structured Output、Tool Calling、Workflow 基本判断、RAG 基本判断、Product Judgment、AI UX、AI-assisted Engineering 与 Testing / Code Review baseline。其余能力延期，保持 `Not Yet Assessed`，直至其首次实际需要的 Phase 或 triggered 情况。

## PRIMARY CORE

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Product Judgment | Confirmed L2 | L4 | CORE | Product-semantic, deterministic-vs-LLM, risk/permission judgment, and basic cost / latency trade-offs are established. Problem framing, user value, AI opportunity, scope, success criteria, quality bar, ROI, adoption, rollout, and real discovery / metrics evidence remain unverified. | High | P3 capability-scope decisions; P7 product discovery and outcome evidence | 2026-09-04 |
| AI UX / Human-AI Interaction | Provisional L2 | L4 | CORE | Can reason about user-visible state and basic human control for AI or workflow interactions, including progress, error, approval, revalidation, retry / recovery, invalidation, and side-effect boundaries. Broader uncertainty, trust calibration, provenance, override, undo, conversational quality, and user validation remain unverified. | Medium | P3 capability UX; P7 user-validation evidence | 2026-09-07 |
| Workflow Design | Provisional L2 | L4 | CORE | Can decompose a bounded task and allocate deterministic code, Tool actions, fixed workflow steps, human approvals and constrained Agent autonomy; can explain and verify routing, sequencing, state transitions, gates, revalidation, failure and recovery in a controlled local runtime. Sustained observability, broader failure ownership and judgment about when workflow is the wrong abstraction remain unverified. | Medium | P3 capability-boundary practice | 2026-09-07 |
| Context Engineering | Not Yet Assessed | L4 | CORE | P3 conceptual exposure: distinguishes system-held information from inference context, signal density from noise, context rot, progressive disclosure, compaction / eviction / rehydration, repository navigation, and source / scope / recency conflict handling. This is exposure only; no assessed capability conclusion or advanced practical evidence. | Baseline Unknown | P3 practical context-selection validation when required | 2026-09-08 |
| Tool / Capability Design | Not Yet Assessed | L4 | CORE | P3 conceptual exposure distinguishes Capability Design (purpose, inputs, outputs, boundary, reuse and verification) from Tool Design (executable surface, schema, permissions, errors and returns). Allowlist and enforceable-constraint reasoning was introduced; practical design evidence is not yet established. | Baseline Unknown | P3 practical capability / tool design validation | 2026-09-08 |
| Eval | Not Assessed | L4 | CORE | Can reason about representative Eval Sets, one-variable comparisons, guardrails, fresh cases, trace-based attribution, and the different roles of Code checks, LLM Judges, and Human evaluation. This remains conceptual exposure with no independently demonstrated improvement loop or formal capability level. | Low | P3 practical capability Eval validation, then P6 deepening | 2026-09-08 |
| AI-assisted Engineering | Provisional L2 | L4 | CORE | P1 Micro Labs include code tracing, meaningful modifications, failure injection, and runtime verification; this round added Codex-assisted mutation demonstration and runtime-Oracle verification. Chapter 11 added learner-defined acceptance criteria plus personal Delay / HTTP 500 / Race runtime verification and final acceptance of a Codex-scoped change. P2 added learner runtime verification of normal approval, reject, stale invalidation, Tool failure, successful retry / recovery, and retry invalidation after external state change for a Codex-assisted local runtime; systematic critical diff review, broader debugging ownership, and independent verification design remain limited. | Medium | P3 key diff review and capability-boundary practice | 2026-09-07 |

## SECONDARY DESIGN AXIS

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Visual / Interaction Design | Not Yet Assessed | L3-L4 | CORE-SUPPORT | Formal secondary learning axis; no current capability evidence. | Baseline Unknown | Natural P2 workflow / approval UX practice, then P7 studio verification | — |

## CORE-SUPPORT

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Structured Output | Provisional L2 | L3 | CORE-SUPPORT | Can distinguish prompt constraints from schema or constrained output, recognize schema drift and semantic-validity limits, and understand validation, retry, repair and fallback roles. Real Provider Structured Output, independent schema authoring and Provider response handling remain unverified. | Medium | P3 schema / validation transfer; Deferred Provider Lab A when Provider API access is available | 2026-09-02 |
| Tool Calling | Confirmed L1 | L3 | CORE-SUPPORT | Can distinguish tool capability from permission and approval, reason about schemas, result matching, dependencies, revalidation and side-effect boundaries, and verify that a controlled local runtime does not execute rejected, invalidated or failed actions prematurely. Real Provider Tool Calling remains unverified. | Medium | Natural P3 capability-boundary practice; Deferred real Provider Tool Calling when Provider API access is available | 2026-09-07 |
| Skill Design | Not Yet Assessed | L3-L4 | CORE-SUPPORT | P3 conceptual exposure: a Skill packages repeatable principles, workflow, judgment criteria, stop conditions, failure behavior, resources and examples; progressive disclosure and stable-versus-volatile rule separation matter. Current Skill / Capability optimization practice is ongoing and is not completion evidence. | Baseline Unknown | P3 practical Skill design validation | 2026-09-08 |
| Agent Design | Not Assessed | L3-L4 | CORE-SUPPORT | Can discuss conceptually how Agent runtime decision rights, observations, action selection, tool / capability use, stopping conditions and control boundaries differ from a fixed Workflow. No real Agent Runtime implementation evidence or assessed design capability. | Low | Natural P3 capability-boundary practice; real Agent Runtime only when needed | 2026-09-08 |
| Integration Engineering | Not Yet Assessed | L2-L3 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P4 first required practice | — |
| Reliability Engineering | Not Yet Assessed | L2-L3 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P5 first required practice | — |
| Memory / State | Not Yet Assessed | L2-L3 | CORE-SUPPORT | P3 conceptual exposure distinguishes current Context, runtime State, durable Memory and historical record; understands selective writing, conflict updates, retrieval failure modes and why stored information does not guarantee correct retrieval. No assessed implementation or capability conclusion. | Baseline Unknown | P3 practical memory / state boundary validation, then P4 persistent state | 2026-09-08 |
| Model Literacy | Confirmed L1 | L2-L3 | CORE-SUPPORT | P1 concepts include Model API / SDK roles, instructions/input, Token and Context Window basics, schema validity versus semantic correctness, and product-level Token / cost / latency trade-offs. Real Provider API use remains unverified. | Medium | Deferred real Provider Model API lab | 2026-09-04 |

## SUPPORTING ENGINEERING LITERACY

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Frontend Engineering (including Web / Frontend boundary) | Confirmed L1 | L2-L3 | SUPPORT | Can trace a basic Browser / Client / Server request-to-state-to-render path and verify a targeted stale-response repair. Broader frontend implementation and interaction design remain unverified. | Medium | Natural P3 feature code mapping and modification | 2026-09-02 |
| TypeScript | Confirmed L1 | L2-L3 | SUPPORT | Can explain why compile-time types do not validate external runtime data and verify a schema-invalid payload failure path. Broader type design and independent implementation remain unverified. | Medium | P3 data-contract modification when needed | 2026-09-02 |
| React | Confirmed L1 | L2-L3 | SUPPORT | Can trace request, state and render responsibilities and verify a targeted stale-response repair. Broader component and state design remain unverified. | Medium | P3 capability interaction work when needed | 2026-09-02 |
| Testing / Code Review | Not Assessed | L2-L3 | SUPPORT | Can perform targeted runtime verification of expected, failed, stale and recovery behavior, and distinguish build or type success from verified behavior. Systematic test design, regression coverage, critical diff review, independent debugging and verification strategy design remain unverified. | Low | P3 testing / diff-review practice | 2026-09-07 |
| Harness | Not Yet Assessed | L1-L2 | SUPPORT | P3 conceptual exposure identifies Harness as the external environment and feedback loop that lets an Agent read, act, run, observe and be corrected; Tool and Skill are components with different responsibilities. No active harness design or modification evidence is established. | Baseline Unknown | P3 project-level Harness practice | 2026-09-08 |
| JavaScript | Confirmed L1 | L2-L3 | SUPPORT | Can read and run basic request-lifecycle and asynchronous code to trace behavior. Broader language foundations and independent implementation remain unverified. | Medium | P3 practical code modification when needed | 2026-09-02 |
| Next.js | Confirmed L1 | L2-L3 | SUPPORT | Can use a small application to trace Browser and Server responsibilities. Broader Next.js implementation and routing remain unverified. | Medium | Natural P3 UI feature implementation when needed | 2026-09-02 |
| HTTP / API | Confirmed L1 | L2-L3 | SUPPORT | Can trace basic request and response behavior and distinguish transport success from invalid runtime data or failure states. API design, authentication and external integration remain unverified. | Medium | Natural P3 capability integration; P4 external API use | 2026-09-02 |
| Async Programming | Provisional L2 | L2-L3 | SUPPORT | Can reason about delay, failure, race, cancellation, stale results and targeted repair in a small UI flow. Broader production async design remains unverified. | Medium | P3 asynchronous capability behavior when needed | 2026-09-02 |
| Git | Confirmed L0 | L2 | SUPPORT | Understands version-control purpose, change scope, checkpoints and how Git records can ground Agent reports. Direct Git operations and independent Git review remain unverified. | High | Natural P3 Git operations and diff review | 2026-09-04 |
| Backend | Not Yet Assessed | L2 | SUPPORT | No assessed capability conclusion. | Baseline Unknown | P3 server / capability boundary when needed, then P5 depth | — |
| Database / Data Modeling | Not Yet Assessed | L2 | SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P4 first required practice | — |
| Authentication / Authorization | Not Yet Assessed | L2 | SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P4 first required practice | — |
| RAG | Confirmed L1 | L2-L3 | SUPPORT | Distinguishes knowledge retrieval from authoritative real-time state; implementation/eval unverified. | Medium | Natural project review | 2026-08-27 |
| MCP | Not Yet Assessed | L2 | SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P4 first required practice | — |
| Security | Not Yet Assessed | L2 | SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P5 first required practice | — |

## AWARENESS / TRIGGERED

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Python | Not Yet Assessed | L1-L2 | AWARENESS | Deferred outside Phase 0 scope | Baseline Unknown | First real project need | — |
| Deployment | Not Yet Assessed | L1-L2 | AWARENESS | Deferred outside Phase 0 scope | Baseline Unknown | P5 deployment practice | — |
| Multi-Agent | Not Yet Assessed | L1 initially | TRIGGERED | Deferred outside Phase 0 scope | Baseline Unknown | Only after a real need is demonstrated | — |
| AI Infrastructure | Not Yet Assessed | L1 | AWARENESS | Deferred outside Phase 0 scope | Baseline Unknown | Only if a real need is demonstrated | — |
## Evidence and Confirmation Rules

- `Not Assessed` 表示当前证据不足以赋予可靠能力等级；该能力可能已经在 P0 中被检查，但证据仍为 `Missing`、`Partial` 或 `Conflicting`。它不表示测评从未触及该能力。
- `Not Yet Assessed` 表示能力被有意延期到其相关 Phase 或真实触发需求之前；在此之前不得推断或评级。
- `Low` Confidence 表示因证据薄弱或缺失而对能力推断的置信度低，不表示学习者能力低。
- 能力升级必须关联解释、修改、调试、验证、迁移或评审中的具体证据。
- Phase 0 原则上最高正式确认到 `Confirmed L2`。更强表现可记录为 `L3 Candidate`，但不能仅凭 Phase 0 正式认证 L3。
- L4 必须依赖长期跨项目证据。
- Phase 0 status and evidence semantics are defined by `ASSESSMENT_SPEC.md`.


