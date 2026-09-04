# Learning Log

## Planning Stage

状态：正式学习尚未开始。

已完成：

- 职业路线研究
- Curriculum v1.0 主骨架
- 能力深度体系
- 课程运行系统设计

第一条正式学习日志必须来自：`Phase 0 Ability Assessment`

本文件以后以追加方式为主，不篡改历史记录。

## Phase 0 Ability Assessment

- Date Completed: 2026-08-27
- Run: `ASSESSMENT_RUN_001`
- P0 Exit Gate: `PASSED`
- Formal Learning: `NO`
- Baseline established; no L3/L4 certification.
- P1 minimum learning density established.
- Next step: select or confirm the P1 training product, then start P1 when the learner explicitly begins formal learning.

## P1 Checkpoint — 2026-09-02

- Formal P1 learning started; current Micro Lab: `p1-async-micro-lab`.
- Completed request lifecycle, async failure/race/cancellation, React stale-response, and TypeScript/Zod runtime-validation labs; Model API / Structured Output concepts covered.
- Real Provider Model API and Provider Structured Output labs are deferred until a provider API key is available; they remain required before the P1 Exit Gate.
- Next: continue the next P1 module; retain deferred Provider evidence in the review queue.

## P1 Checkpoint — 2026-09-04

- Completed Streaming / AI UI State and Tool Calling basics; the standalone Integrated Feature chapter/practice was compressed because it combined previously learned mechanisms and produced no independent integration-practice evidence.
- Streaming runtime evidence: normal `done → completed`; HTTP 200 with partial content followed by stream close without `done` → `interrupted`; after regenerate, late `content_delta` / `done` events from the prior generation were ignored.
- Tool Calling runtime evidence: `tool_call_id` matched multiple Tool Results; invalid Tool Schema caused runtime rejection with no Tool Execution; dependent Tool Calls were created only after the prior Tool Result returned.
- Completed Basic Testing / Eval / Verification conceptual coverage. In a Codex-assisted mutation-testing demonstration, a Schema reject was deliberately changed to still execute a Tool: `next build` passed, but the `tool_execution count = 0` runtime Oracle failed; after correct behavior was restored, the Oracle passed again.
- Real Provider Model API, Structured Output, Tool Calling, and end-to-end integration evidence remain deferred until Provider API access is available. This checkpoint does not assert independent learner mastery from Codex-assisted work.

## P1 Local Completion Checkpoint — 2026-09-04

- Completed Chapter 10 Cost / Latency / Model-use Decisions: product-level reasoning covered token and call-cost drivers, expected cost, retry and parallelization trade-offs, actual versus perceived latency, context compression trade-offs, and marginal cost versus quality / risk gain.
- Completed Chapter 11 AI-assisted Engineering Ownership in `p1-async-micro-lab`: the learner defined expected behavior, then personally verified Delay, HTTP 500, and Race behavior in the webpage and made the final Accept judgment for the Codex-assisted scoped change.
- Completed P1 Consolidation: connected Client / UI State → HTTP / Async → Streaming → Race / stale generation → Runtime Validation → Retry / Repair / Fallback / Error, including stale-event suppression and schema-invalid output handling.
- Current state: `P1 Local Learning Complete / Exit Gate Provider Evidence Deferred`; P1 is not formally passed. Provider Model API, API Key / Secret handling, Structured Output, and real end-to-end integration evidence remain deferred; Provider Tool Calling remains verification evidence unless the integration needs it.
- Next: Begin P2 — Workflow + Tool + AI-native Interaction.
