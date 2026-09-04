# Current Learning State

Curriculum Version: v1.2
Assessment Spec Version: v1.0.1

Lifecycle Position: P1 In Progress
Current Phase: P1 — AI Product Technical Literacy / Engineering Literacy Foundation
Current Learning Position: Formal P1 Learning
Module: P1 — Chapter 9 complete; Provider integration labs deferred
Status: P1 IN PROGRESS

Formal Learning Started: YES
Formal Assessment Active: NO
Phase 0 Assessment Completed: YES
Active Assessment Run: None
Completed Assessment Run: ASSESSMENT_RUN_001
Baseline Reference: ASSESSMENT_RUN_001.md — read when P1 startup or evidence-boundary clarification is needed.

## Current Focus

P1 formal learning is in progress as the AI Product Technical Literacy / Engineering Literacy Foundation. Completed evidence includes: Web request lifecycle; JavaScript async/error/timeout/cancellation/race behavior; React request-to-state-to-render interaction; TypeScript/Zod runtime validation; Model API / Structured Output concepts; Streaming / AI UI State; Tool Calling basics; and Basic Testing / Eval / Verification conceptual coverage with one Codex-assisted mutation-testing demonstration. `p1-async-micro-lab` remains the current P1 Micro Lab.

The standalone Integrated Feature chapter/practice was compressed because it primarily combined mechanisms already learned; it does not create independent integration-practice evidence or waive the real Provider end-to-end integration required before the P1 Exit Gate. Real Provider Model API, Structured Output, Tool Calling, and end-to-end integration remain deferred until Provider API access is available. Codex-assisted demonstration is not independent learner mastery.

## P1 Minimum Learning Density

High density: Browser / Client / Server responsibility, AI UI state / Streaming, Tool vs deterministic logic, Model integration, runtime validation, Testing / Eval / verification, and AI-agent diff review / ownership. Supporting engineering literacy: JavaScript, TypeScript, React, Next.js, HTTP/API, Async, secrets, Git and backend basics are learned to read, trace, modify and verify critical product paths, not as long-term framework-proficiency targets. Product Judgment, AI UX and Visual / Interaction quality remain active through P1.

Minimum Learning Density is a calibration overlay, not a replacement for the full P1 Core Capabilities in `CURRICULUM.md`. High density identifies current product and verification priorities; supporting literacy identifies the minimum technical depth required for ownership. Unmentioned P1 capabilities are not automatically skipped and enter when the P1 feature requires them.

## P1 Remaining Execution Plan

### Chapter 10 — Cost / Latency / Model-use Decisions

Build product-level cost and latency judgment: Token cost drivers (Input / Output / Reasoning), model choice and quality trade-offs, single versus multiple calls, workflow call accumulation, actual versus perceived latency, Streaming, and basic serial / parallel effects. Do not memorize Provider pricing, pursue traditional performance optimization, or study infrastructure / profiling depth. The required outcome is a reasonable product judgment about where an AI feature's cost and latency arise.

### Chapter 11 — AI-assisted Engineering Ownership

Practice responsibility-layer judgment (Client / Server / State / Validation / Provider / Tool Runtime), basic `git status` / `git diff` / commit and previous-version literacy, key diff review, acceptance criteria, runtime and failure-path verification, and final accept / reject judgment. Use `p1-async-micro-lab` for one small real behavior change: decide the responsibility layer and expected behavior first; let Codex implement; review the key diff; run minimal verification; inspect or create one meaningful failure / edge case; then decide acceptance. Do not re-teach the existing Deduplication-set mechanisms in full.

### P1 Consolidation / Exit Gate Readiness

After Chapter 11, do not add new default P1 Chapters. Connect the completed P1 mental models, inspect learner evidence versus Codex-assisted evidence, missing evidence, and deferred Provider evidence, and only fill real gaps. This is neither a new theory Chapter nor broad reassessment; if evidence is sufficient, proceed directly to Exit Gate readiness.

### Deferred Provider Labs

When Provider API access is available, run two compact labs without reopening basic theory:

- **Provider Lab A — Real Model + Structured Output:** API Key / Secret boundary, real Provider Model API, real Structured Output, runtime validation, and at least one failure path.
- **Provider Lab B — Real End-to-End AI Feature:** `UI → Server → Provider → Model Output → Validation → UI State`, including a normal result, at least one failure path, runtime verification, and a user-visible state. This supplies the real Provider integration evidence required by the P1 Exit Gate.

Real Provider Tool Calling remains deferred verification evidence for P1/P2. Do it only when the actual integration naturally needs it; it is not a standalone P1 Exit Gate requirement.

### Provider-Access Contingency

If Chapters 10 and 11 plus P1 Consolidation / Exit Gate Readiness are complete but Provider API access remains unavailable, set the current state to `P1 Local Learning Complete / Exit Gate Provider Evidence Deferred`. Do not manufacture additional P1 Chapters or let external API access block subsequent learning: P2 formal learning may begin while P1 remains not formally `PASSED`. Return to the Provider Labs and P1 Exit Gate when access becomes available.

P1 Exit Gate requirements remain defined by `CURRICULUM.md`; this execution plan adds none.

Next Action: Begin Chapter 10 — Cost / Latency / Model-use Decisions.
