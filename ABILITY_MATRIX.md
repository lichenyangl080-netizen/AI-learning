# Ability Matrix

本矩阵同时记录当前可归档证据与计划目标深度。`Current Status` 不得由历史聊天、项目经历、阅读资料或 Codex 产出自动赋值；项目完成与工具产出均不能单独证明掌握。

## Phase 0 Scope

Phase 0 只主测以下范围：Web / Frontend boundary、JavaScript / TypeScript、React / Next.js 基础、HTTP / API、Async、Git、Model Literacy 基础、Structured Output、Tool Calling、Workflow 基本判断、RAG 基本判断、Product Judgment、AI UX、AI-assisted Engineering 与 Testing / Code Review baseline。其余能力延期，保持 `Not Yet Assessed`，直至其首次实际需要的 Phase 或 triggered 情况。

## PRIMARY CORE

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Product Judgment | Confirmed L2 | L4 | CORE | Product-semantic, deterministic-vs-LLM, risk/permission judgment; real discovery/metrics unverified. | High | Natural P1 project verification | 2026-08-27 |
| AI UX / Human-AI Interaction | Provisional L2 | L4 | CORE | Loading/success/failure, approval and uncertainty reasoning; practical AI UI/streaming unverified. | Medium | P1 project UX verification | 2026-08-27 |
| Workflow Design | Provisional L2 | L4 | CORE | Deterministic/model/tool/validator responsibility and perturbation adaptation; implementation evidence needed. | Medium | P1/P2 workflow implementation | 2026-08-27 |
| Context Engineering | Not Yet Assessed | L4 | CORE | P1 exposure only: Context Window; Input / Output / Reasoning Tokens; context selection, compaction, and retrieval. No assessed capability conclusion; remains deferred. | Baseline Unknown | P3 first required practice | — |
| Tool / Capability Design | Not Yet Assessed | L4 | CORE | Deferred outside Phase 0 scope | Baseline Unknown | P3 first required practice | — |
| Eval | Not Yet Assessed | L4 | CORE | Deferred outside Phase 0 scope | Baseline Unknown | P1 basic Eval, then P6 deepening | — |
| AI-assisted Engineering | Provisional L2 | L4 | CORE | P1 Micro Labs include code tracing, meaningful modifications, failure injection, and runtime verification. Systematic diff review and broader debugging ownership remain limited. | Medium | P1 diff review and verification | 2026-09-02 |

## SECONDARY DESIGN AXIS

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Visual / Interaction Design | Not Yet Assessed | L3-L4 | CORE-SUPPORT | Formal secondary learning axis; no current capability evidence. | Baseline Unknown | Natural P1 AI UI practice, then P7 studio verification | — |

## CORE-SUPPORT

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Structured Output | Provisional L2 | L3 | CORE-SUPPORT | P1 reinforced prompt constraint vs schema/constrained output, schema drift, and retry / repair / fallback. Local Zod validation behavior was verified, but real Provider Structured Output, independent schema authoring, and Provider response handling remain unverified. | Medium | Deferred real Provider Structured Output lab, then P1 schema implementation | 2026-09-02 |
| Tool Calling | Confirmed L1 | L3 | CORE-SUPPORT | Understands tool/API, read/write, approval and permission boundary; real calls/schema unverified. | Medium | P1/P2 practical tool use | 2026-08-27 |
| Skill Design | Not Yet Assessed | L3-L4 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P3 first required practice | — |
| Agent Design | Not Yet Assessed | L3-L4 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P2 basic agent loop | — |
| Integration Engineering | Not Yet Assessed | L2-L3 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P4 first required practice | — |
| Reliability Engineering | Not Yet Assessed | L2-L3 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P5 first required practice | — |
| Memory / State | Not Yet Assessed | L2-L3 | CORE-SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P3 basics, then P4 persistent state | — |
| Model Literacy | Confirmed L1 | L2-L3 | CORE-SUPPORT | P1 concepts include Model API / SDK roles, instructions/input, Token and Context Window basics, and schema validity versus semantic correctness. Real Provider API use remains unverified. | Medium | Deferred real Provider Model API lab | 2026-09-02 |

## SUPPORTING ENGINEERING LITERACY

| Ability | Current Status | Target Level | Priority | Evidence | Confidence | Next Verification | Last Verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Frontend Engineering (including Web / Frontend boundary) | Confirmed L1 | L2-L3 | SUPPORT | Confirmed L1 covers Web/Frontend boundary plus P1 Request Trace and React request → state → render inspection; a request-ID stale-response fix was run and verified. Broader frontend implementation remains unverified. | Medium | P1 feature code mapping and modification | 2026-09-02 |
| TypeScript | Confirmed L1 | L2-L3 | SUPPORT | P1 TypeScript/Zod lab: real code reading and runtime verification of HTTP 200 with schema-invalid payload; broader type design and independent implementation remain unverified. | Medium | P1 practical foundation and data-contract modification | 2026-09-02 |
| React | Confirmed L1 | L2-L3 | SUPPORT | P1 React lab: traced request → state → render and applied a request-ID stale-response fix with runtime verification; broader component and state design remains unverified. | Medium | P1 feature state and interaction work | 2026-09-02 |
| Testing / Code Review | Not Assessed | L2-L3 | SUPPORT | P1 failure injection and runtime verification cover delayed responses, HTTP 500, stale response, and schema-invalid payload paths. Systematic test authoring, diff review, and independent debugging evidence remain limited. | Low | P1 testing and diff review | 2026-09-02 |
| Harness | Not Yet Assessed | L1-L2 | SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P3 application-level introduction | — |
| JavaScript | Confirmed L1 | L2-L3 | SUPPORT | P1 code reading and running verification across request lifecycle and async labs; broader language foundations and independent implementation remain unverified. | Medium | P1 practical foundation and code modification | 2026-09-02 |
| Next.js | Confirmed L1 | L2-L3 | SUPPORT | P1 Micro Lab code was read and run to trace Browser / Server behavior; broader Next.js implementation and routing remain unverified. | Medium | P1 feature implementation | 2026-09-02 |
| HTTP / API | Confirmed L1 | L2-L3 | SUPPORT | P1 Request Trace plus HTTP 200, HTTP 500, and HTTP-success/schema-invalid payload paths were run and verified; API design, auth, and external integration remain unverified. | Medium | P1 practical API use | 2026-09-02 |
| Async Programming | Provisional L2 | L2-L3 | SUPPORT | P1 Async lab ran delay, HTTP 500, race, cancellation, and stale-response scenarios; a request-ID stale-response repair was run and verified. Broader production async design remains unverified. | Medium | P1 await/timeout/cancellation and failure-path transfer | 2026-09-02 |
| Git | Confirmed L0 | L2 | SUPPORT | Version-control purpose and isolation understood; operations unverified. | High | P1 Git operations | 2026-08-27 |
| Backend | Not Yet Assessed | L2 | SUPPORT | Deferred outside Phase 0 scope | Baseline Unknown | P1 Server / Client boundary, then P5 depth | — |
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


