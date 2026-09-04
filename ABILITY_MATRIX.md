# Ability Matrix

本矩阵同时记录当前可归档证据与计划目标深度。`Current Status` 不得由历史聊天、项目经历、阅读资料或 Codex 产出自动赋值；项目完成与工具产出均不能单独证明掌握。

## Phase 0 Scope

Phase 0 只主测以下范围：Web / Frontend boundary、JavaScript / TypeScript、React / Next.js 基础、HTTP / API、Async、Git、Model Literacy 基础、Structured Output、Tool Calling、Workflow 基本判断、RAG 基本判断、Product Judgment、AI UX、AI-assisted Engineering 与 Testing / Code Review baseline。其余能力延期，保持 `Not Yet Assessed`，直至其首次实际需要的 Phase 或 triggered 情况。

## PRIMARY CORE

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Product Judgment | Confirmed L2 | L4 | CORE | Product-semantic, deterministic-vs-LLM, risk/permission judgment; P1 cost / latency decisions cover marginal cost versus quality / risk gain, model choice, retry, context, and expected-cost trade-offs. Real discovery/metrics remain unverified. | High | Natural P2 product verification | 2026-09-04 |
| AI UX / Human-AI Interaction | Provisional L2 | L4 | CORE | Loading/success/failure, approval and uncertainty reasoning; P1 runtime streaming evidence covers normal completion, interrupted stream, stale-generation suppression, and ignoring late prior-generation events after regenerate. Broader AI UX and user validation remain unverified. | Medium | P2 workflow / approval UX transfer | 2026-09-04 |
| Workflow Design | Provisional L2 | L4 | CORE | Deterministic/model/tool/validator responsibility and perturbation adaptation; P1 cost / latency reasoning covers call accumulation, conditional expected cost, retry cost, and serial / parallel trade-offs. Workflow implementation evidence remains needed. | Medium | P2 workflow implementation | 2026-09-04 |
| Context Engineering | Not Yet Assessed | L4 | CORE | P1 exposure only: Context Window; Input / Output / Reasoning Tokens; context selection, compaction, and retrieval. No assessed capability conclusion; remains deferred. | Baseline Unknown | P3 first required practice | — |
| Tool / Capability Design | Not Yet Assessed | L4 | CORE | Deferred outside Phase 0 scope | Baseline Unknown | P3 first required practice | — |
| Eval | Not Assessed | L4 | CORE | P1 basic conceptual coverage: Rubric, Eval Set, Regression, Human Judge, Programmatic Judge, LLM Judge, Hard Gate, and Soft Eval. Codex-assisted mutation-testing demonstration verified a runtime Oracle catching build-pass / behavior-fail execution. Evidence remains insufficient for a formal capability level. | Low | P2 workflow verification, then P6 deepening | 2026-09-04 |
| AI-assisted Engineering | Provisional L2 | L4 | CORE | P1 Micro Labs include code tracing, meaningful modifications, failure injection, and runtime verification; this round added Codex-assisted mutation demonstration and runtime-Oracle verification. Chapter 11 added learner-defined acceptance criteria plus personal Delay / HTTP 500 / Race runtime verification and final acceptance of a Codex-scoped change. Systematic critical diff review, broader debugging ownership, and independent verification design remain limited. | Medium | P2 diff review and verification | 2026-09-04 |

## SECONDARY DESIGN AXIS

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Visual / Interaction Design | Not Yet Assessed | L3-L4 | CORE-SUPPORT | Formal secondary learning axis; no current capability evidence. | Baseline Unknown | Natural P2 workflow / approval UX practice, then P7 studio verification | — |

## CORE-SUPPORT

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Structured Output | Provisional L2 | L3 | CORE-SUPPORT | P1 reinforced prompt constraint vs schema/constrained output, schema drift, and retry / repair / fallback. Local Zod validation behavior was verified, but real Provider Structured Output, independent schema authoring, and Provider response handling remain unverified. | Medium | P2 schema / validation transfer; Deferred Provider Lab A when Provider API access is available | 2026-09-02 |
| Tool Calling | Confirmed L1 | L3 | CORE-SUPPORT | Understands tool/API, read/write, approval and permission boundary. P1 local runtime Tool Calling (Codex-assisted) covered Tool Schema validation, `tool_call_id` matching for multiple / parallel Tool Results, dependent serial Tool Calls, and invalid schema → runtime reject → no execution. Real Provider Tool Calling remains unverified. | Medium | P2 practical tool use; Deferred real Provider Tool Calling when Provider API access is available | 2026-09-04 |
| Skill Design | Not Yet Assessed | L3-L4 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P3 first required practice | — |
| Agent Design | Not Yet Assessed | L3-L4 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P2 basic agent loop | — |
| Integration Engineering | Not Yet Assessed | L2-L3 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P4 first required practice | — |
| Reliability Engineering | Not Yet Assessed | L2-L3 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P5 first required practice | — |
| Memory / State | Not Yet Assessed | L2-L3 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P3 basics, then P4 persistent state | — |
| Model Literacy | Confirmed L1 | L2-L3 | CORE-SUPPORT | P1 concepts include Model API / SDK roles, instructions/input, Token and Context Window basics, schema validity versus semantic correctness, and product-level Token / cost / latency trade-offs. Real Provider API use remains unverified. | Medium | Deferred real Provider Model API lab | 2026-09-04 |

## SUPPORTING ENGINEERING LITERACY

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Frontend Engineering (including Web / Frontend boundary) | Confirmed L1 | L2-L3 | SUPPORT | Confirmed L1 covers Web/Frontend boundary plus P1 Request Trace and React request → state → render inspection; a request-ID stale-response fix was run and verified. Broader frontend implementation remains unverified. | Medium | Natural P2 feature code mapping and modification | 2026-09-02 |
| TypeScript | Confirmed L1 | L2-L3 | SUPPORT | P1 TypeScript/Zod lab: real code reading and runtime verification of HTTP 200 with schema-invalid payload; broader type design and independent implementation remain unverified. | Medium | P2 data-contract modification when needed | 2026-09-02 |
| React | Confirmed L1 | L2-L3 | SUPPORT | P1 React lab: traced request → state → render and applied a request-ID stale-response fix with runtime verification; broader component and state design remains unverified. | Medium | P2 workflow state and interaction work | 2026-09-02 |
| Testing / Code Review | Not Assessed | L2-L3 | SUPPORT | P1 failure injection and runtime verification cover delayed responses, HTTP 500, stale response, and schema-invalid payload paths; this round added runtime Oracle and mutation demonstration showing build pass can coexist with runtime behavior failure. Chapter 11 added learner-performed targeted Delay / HTTP 500 / Race runtime verification and final acceptance judgment. Systematic test authoring, persistent behavior tests, broader regression suite, critical diff review, and independent debugging evidence remain limited. | Low | P2 testing and diff review | 2026-09-04 |
| Harness | Not Yet Assessed | L1-L2 | SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P3 application-level introduction | — |
| JavaScript | Confirmed L1 | L2-L3 | SUPPORT | P1 code reading and running verification across request lifecycle and async labs; broader language foundations and independent implementation remain unverified. | Medium | P2 practical code modification when needed | 2026-09-02 |
| Next.js | Confirmed L1 | L2-L3 | SUPPORT | P1 Micro Lab code was read and run to trace Browser / Server behavior; broader Next.js implementation and routing remain unverified. | Medium | Natural P2 UI feature implementation | 2026-09-02 |
| HTTP / API | Confirmed L1 | L2-L3 | SUPPORT | P1 Request Trace plus HTTP 200, HTTP 500, and HTTP-success/schema-invalid payload paths were run and verified; API design, auth, and external integration remain unverified. | Medium | P2 tool / external API use when needed | 2026-09-02 |
| Async Programming | Provisional L2 | L2-L3 | SUPPORT | P1 Async lab ran delay, HTTP 500, race, cancellation, and stale-response scenarios; a request-ID stale-response repair was run and verified. Broader production async design remains unverified. | Medium | P2 workflow await / failure-path transfer | 2026-09-02 |
| Git | Confirmed L0 | L2 | SUPPORT | Version-control purpose and isolation understood; learner understands Git records can ground Agent reports of change scope and checkpoints / previous versions. Direct Git operations and independent Git review remain unverified. | High | P2 Git operations when needed | 2026-09-04 |
| Backend | Not Yet Assessed | L2 | SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P2 tool / server boundary when needed, then P5 depth | — |
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


