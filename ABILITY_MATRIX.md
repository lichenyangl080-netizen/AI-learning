# Ability Matrix

本矩阵同时记录当前可归档证据与计划目标深度。`Current Status` 不得由历史聊天、项目经历、阅读资料或 Codex 产出自动赋值；项目完成与工具产出均不能单独证明掌握。

## Phase 0 Scope

Phase 0 只主测以下范围：Web / Frontend boundary、JavaScript / TypeScript、React / Next.js 基础、HTTP / API、Async、Git、Model Literacy 基础、Structured Output、Tool Calling、Workflow 基本判断、RAG 基本判断、Product Judgment、AI UX、AI-assisted Engineering 与 Testing / Code Review baseline。其余能力延期，保持 `Not Yet Assessed`，直至其首次实际需要的 Phase 或 triggered 情况。

## PRIMARY CORE

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Product Judgment | Confirmed L2 | L4 | CORE | Can judge product semantics, deterministic-versus-LLM fit, risk/permission boundaries, basic cost/latency trade-offs, and conceptual integration-surface trade-offs. Problem framing, user value, AI opportunity, scope, success criteria, quality bar, ROI, adoption, rollout, and real discovery/metrics evidence remain unverified. | High | P6 product specification and acceptance decisions; P7 discovery, rollout and outcome evidence | 2026-09-09 |
| AI UX / Human-AI Interaction | Provisional L2 | L4 | CORE | Can reason about user-visible state and basic human control, including progress, error, approval, revalidation, retry/recovery, invalidation and side-effect boundaries. Uncertainty, trust calibration, provenance, override/undo, latency perception, conversational quality and real user validation remain unverified. | Medium | P6 product interaction and verification; P7 real-user validation | 2026-09-07 |
| Workflow Design | Provisional L2 | L4 | CORE | Can decompose a bounded task across deterministic code, Tool actions, fixed workflow steps, human approvals and constrained Agent autonomy; a real Product Design optimization also exercised scoped Candidate flow, steering, rejection/restore and acceptance. Sustained observability, broader failure ownership and judgment about when workflow is the wrong abstraction remain unverified. | Medium | P7 cross-product workflow and user-outcome evidence | 2026-09-10 |
| Context Engineering | Not Yet Assessed | L4 | CORE | P3 core instruction covered context selection, signal density, context rot, progressive disclosure, compaction/eviction/rehydration and source/scope/recency conflicts. The Product Design optimization adds practical evidence of scoped context, reference/boundary preservation and checkpoint-based rehydration; cross-project transfer remains unverified. | Baseline Unknown | Future cross-project context packaging and transfer | 2026-09-10 |
| Tool / Capability Design | Not Yet Assessed | L4 | CORE | P3 core instruction covered Capability Design versus Tool Design, allowlists and enforceable constraints. A real Product Design workflow now provides practical evidence of capability boundaries, scoped file permissions, checkpoint/QA/restore gates and failure containment; broader reusable design remains unverified. | Baseline Unknown | Future product capability/tool design with a new domain | 2026-09-10 |
| Eval | Not Assessed | L4 | CORE | Can reason about Eval Sets, guardrails, fresh cases, trace attribution and Code/LLM Judge/Human roles. The real practice completed seven test groups, three-way visual QA, correction, reject/restore and accepted paths; independent cross-product Eval design and outcome metrics remain unverified. | Low | P7 product-quality Eval with new users or a new domain | 2026-09-10 |
| AI-assisted Engineering | Provisional L2 | L4 | CORE | A real Product Design practice completed problem/scope, context/delegation, steering, implementation, verification/Eval, correction and explicit acceptance; an incorrect screenshot-source direction was withdrawn. Broader cross-project delegation, critical diff review and independent verification design remain limited. | Medium | P7 end-to-end product iteration with new user evidence | 2026-09-10 |

## SECONDARY DESIGN AXIS

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Visual / Interaction Design | Not Yet Assessed | L3-L4 | CORE-SUPPORT | Formal secondary learning axis; no current capability evidence. | Baseline Unknown | P6 real product interaction work; P7 design and user-validation evidence | — |

## CORE-SUPPORT

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Structured Output | Provisional L2 | L3 | CORE-SUPPORT | Can distinguish prompt constraints from schema/constrained output, recognize schema drift and semantic-validity limits, and explain validation, retry, repair and fallback roles. Real Provider Structured Output, independent schema authoring and Provider response handling remain unverified. | Medium | P6 product schema/validation use; Provider Lab when API access is available | 2026-09-02 |
| Tool Calling | Confirmed L1 | L3 | CORE-SUPPORT | Can distinguish tool capability from permission and approval, reason about schemas, result matching, dependencies, revalidation and side-effect boundaries, and verify that a controlled local runtime does not execute rejected, invalidated or failed actions prematurely. Real Provider Tool Calling remains unverified. | Medium | P6 practical tool use when the product needs it; real Provider verification when access is available | 2026-09-07 |
| Skill Design | Not Yet Assessed | L3-L4 | CORE-SUPPORT | P3 core instruction covered reusable principles, workflow, judgment criteria, stop conditions, failure behavior, resources and examples. The completed Product Design optimization provides practical evidence of turning repeated failures into bounded Skill/capability rules with checkpoint, QA and restore behavior; cross-project reuse remains unverified. | Baseline Unknown | Future Skill reuse in a different product or task family | 2026-09-10 |
| Agent Design | Not Assessed | L3-L4 | CORE-SUPPORT | Can conceptually distinguish Agent runtime decision rights, observations, action selection, tool/capability use, stopping conditions and control boundaries from a fixed Workflow. No real Agent Runtime implementation evidence or assessed design capability. | Low | P6 Agent delegation/control design; real Agent Runtime only when the product needs it | 2026-09-08 |
| Integration Engineering | Not Yet Assessed | L2-L3 | CORE-SUPPORT | P4 core conceptual instruction covered: compares structured API, MCP, Browser/Computer Use, RAG and persistent state by authority, completeness, permission risk, latency, cost, verifiability and complexity. No real integration ownership evidence. | Baseline Unknown | First P6/P7/P8 product that naturally requires an external integration | 2026-09-09 |
| Reliability Engineering | Not Yet Assessed | L2-L3 | CORE-SUPPORT | Deferred outside Phase 0 scope; no assessed capability evidence. | Baseline Unknown | First real product risk requiring reliability, recovery or observability | — |
| Memory / State | Not Yet Assessed | L2-L3 | CORE-SUPPORT | P3/P4 core concepts covered: distinguishes Context, runtime State, durable Memory and History; understands selective memory writing, conflict updates, retrieval failure modes, ownership and copy/sync direction. No assessed implementation or capability conclusion. | Baseline Unknown | P6 natural product state/memory need or later triggered integration | 2026-09-09 |
| Model Literacy | Confirmed L1 | L2-L3 | CORE-SUPPORT | P1 concepts include Model API / SDK roles, instructions/input, Token and Context Window basics, schema validity versus semantic correctness, and product-level Token / cost / latency trade-offs. Real Provider API use remains unverified. | Medium | Deferred real Provider Model API lab | 2026-09-04 |

## SUPPORTING ENGINEERING LITERACY

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Frontend Engineering (including Web / Frontend boundary) | Confirmed L1 | L2-L3 | SUPPORT | Can trace a basic Browser/Client/Server request-to-state-to-render path and verify a targeted stale-response repair. Broader frontend implementation and interaction design remain unverified. | Medium | P6 real product code mapping, targeted modification and verification | 2026-09-02 |
| TypeScript | Confirmed L1 | L2-L3 | SUPPORT | Can explain why compile-time types do not validate external runtime data and verify a schema-invalid payload failure path. Broader type design and independent implementation remain unverified. | Medium | P6 data-contract work when required by the product | 2026-09-02 |
| React | Confirmed L1 | L2-L3 | SUPPORT | Can trace request, state and render responsibilities and verify a targeted stale-response repair. Broader component and state design remain unverified. | Medium | P6 real product interaction work when needed | 2026-09-02 |
| Testing / Code Review | Not Assessed | L2-L3 | SUPPORT | Can perform targeted runtime verification and distinguish build/type success from verified behavior. The completed practice reran seven test groups and exercised visual QA, rejection/restore, checkpoint integrity and final acceptance; systematic independent test strategy and broader regression ownership remain unverified. | Low | P7 independent verification and regression design on a new product | 2026-09-10 |
| Harness | Not Yet Assessed | L1-L2 | SUPPORT | P3 core instruction covered Harness as the external action/observation/feedback environment. The completed practice provides project-level evidence through checkpoint persistence, process rediscovery, restore verification, Candidate state and acceptance gates; broader Harness design remains unverified. | Baseline Unknown | Future project-level Harness design across a new environment | 2026-09-10 |
| JavaScript | Confirmed L1 | L2-L3 | SUPPORT | Can read and run basic request-lifecycle and asynchronous code to trace behavior. Broader language foundations and independent implementation remain unverified. | Medium | P6 targeted product modification when needed | 2026-09-02 |
| Next.js | Confirmed L1 | L2-L3 | SUPPORT | Can use a small application to trace Browser and Server responsibilities. Broader Next.js implementation and routing remain unverified. | Medium | P6 product implementation when the selected stack requires it | 2026-09-02 |
| HTTP / API | Confirmed L1 | L2-L3 | SUPPORT | Can trace request/response behavior and distinguish transport success from invalid runtime data or failure states. P4 concepts add contract-risk awareness for completeness, pagination, rate limits, freshness/cache, versioning/deprecation and error semantics; external integration remains unverified. | Medium | First P6/P7/P8 external API need | 2026-09-09 |
| Async Programming | Provisional L2 | L2-L3 | SUPPORT | Can reason about delay, failure, race, cancellation, stale results and targeted repair in a small UI flow. Broader production async design remains unverified. | Medium | P6 async product behavior when needed | 2026-09-02 |
| Git | Confirmed L0 | L2 | SUPPORT | Understands version-control purpose, change scope, checkpoints and how Git records can ground Agent reports. Direct Git operations and independent Git review remain unverified. | High | P6 real Git status/diff/commit and review workflow | 2026-09-04 |
| Backend | Not Yet Assessed | L2 | SUPPORT | No assessed capability conclusion. | Baseline Unknown | First P6/P7/P8 server or capability-boundary need | — |
| Database / Data Modeling | Not Yet Assessed | L2 | SUPPORT | P4 core concepts covered: distinguishes conversation/context, files and database by reuse, scale and structured read/write needs; separates runtime from persistent state and clarifies Owner, Writer and copy/sync direction. No implementation evidence. | Baseline Unknown | First real product persistent-state need | 2026-09-09 |
| Authentication / Authorization | Not Yet Assessed | L2 | SUPPORT | P4 core concepts covered: distinguishes identity from permission, least privilege from login, approval from authorization, and UI hiding from execution-layer enforcement. Object-level authorization, OAuth/RBAC depth and real implementation remain unverified. | Baseline Unknown | First real product permission or identity need | 2026-09-09 |
| RAG | Confirmed L1 | L2-L3 | SUPPORT | Distinguishes knowledge retrieval from authoritative real-time state; P4 concepts cover Retrieval Miss, Wrong Retrieval, Stale Source and Synthesis Error attribution plus grounding/citation limits. Implementation and Eval evidence remain unverified. | Medium | First real product retrieval need | 2026-09-09 |
| MCP | Not Yet Assessed | L2 | SUPPORT | P4 core concepts covered: distinguishes MCP as an Agent-facing interface from ordinary APIs and compares structured Tool surfaces with GUI/Computer Use by stability, verification, permission control and reuse. No MCP implementation evidence. | Baseline Unknown | First real product need where MCP is preferable to direct API/Tool use | 2026-09-09 |
| Security | Not Yet Assessed | L2 | SUPPORT | Deferred outside Phase 0 scope; no assessed capability evidence. | Baseline Unknown | First real product security, permission or side-effect risk | — |

## AWARENESS / TRIGGERED

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Python | Not Yet Assessed | L1-L2 | AWARENESS | Deferred outside Phase 0 scope | Baseline Unknown | First real project need | — |
| Deployment | Not Yet Assessed | L1-L2 | AWARENESS | Deferred outside Phase 0 scope. | Baseline Unknown | First real product delivery need | — |
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
