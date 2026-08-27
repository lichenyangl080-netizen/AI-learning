# Phase 0 Assessment Specification v1.0.1

## 1. Purpose

Phase 0 is an **Evidence-based AI-native Capability Baseline**. It is not a traditional exam, ranking system, or memory test. It determines what the learner understands; what they can design with normal AI/documentation support; whether they can verify AI-generated work; where AI-assisted work becomes a black box; which foundations should be skipped, reviewed, learned, or naturally verified in P1; and the minimum appropriate P1 teaching density.

It establishes starting evidence, not full certification of every curriculum capability. Absence of evidence is not evidence of low ability.

## 2. Assessment Scope

### Main Phase 0 Scope

Only `Not Assessed` abilities in the current Phase 0 scope of `ABILITY_MATRIX.md` are actively assessed: Web / Frontend boundary; JavaScript / TypeScript; React / Next.js fundamentals; HTTP / API; Async Programming; Git fundamentals; Model Literacy fundamentals; Structured Output; Tool Calling; Workflow basic judgment; RAG basic judgment; Product Judgment; AI UX / Human-AI Interaction; AI-assisted Engineering; and Testing / Code Review baseline.

Measure only the depth needed to calibrate early curriculum. One realistic scenario may provide evidence for several abilities; do not create isolated questions merely to cover a table.

### Deferred Capabilities

`Not Yet Assessed` abilities remain deferred and must not be silently inferred, scored, or leveled in P0. This includes Context Engineering depth, Tool / Capability Design depth, Skill Design, Agent Design depth, Integration Engineering, Reliability Engineering, Harness, Backend depth, Database / Data Modeling depth, Authentication / Authorization depth, MCP, Memory / State depth, Security, Python, Deployment, Multi-Agent, and AI Infrastructure. Assess them only when their relevant phase or a real project first requires them.

## 3. Realistic Tool Policy

P0 runs in a normal AI-native engineering environment. ChatGPT, Codex/coding agents, web search, official documentation, IDE, testing, and debugging tools are allowed by default. AI use is not cheating; the assessment evaluates ownership, understanding, judgment, and verification.

For selected tasks, request a short pre-tool snapshot: “Before using tools, what is your current judgment?” It is a diagnostic mental-model snapshot lasting seconds or minutes, never a closed-book section. Normal tools remain available immediately afterward.

## 4. Assessment Shape

P0 uses four adaptive stages. Typical total effort is approximately 2.5–4 hours and may be split across conversations; this is a planning range, not a quota. Stop early when sufficient evidence is reached.

### Stage A — Baseline Map

Typical duration: 20–30 minutes. Use a small number of realistic multi-signal scenarios to map mental models, likely strengths, uncertainty, misconceptions, blocking-gap candidates, and areas needing deep dive. Collect useful First-pass judgments, explanations, uncertainty, and evidence needs. Dispositions are: sufficient initial evidence, uncertain, conflicting evidence, possible blocking gap, or needs adaptive deep dive. Stage A alone does not establish final capability levels.

### Stage B — Adaptive Deep Dive

Typical duration: 45–75 minutes. Select approximately 3–5 areas from Stage A, prioritizing blocking gaps; P1-relevant CORE/CORE-SUPPORT abilities; conflicting evidence; and capabilities that materially change P1 teaching density. Strong areas terminate once evidence is sufficient. Prefer unfamiliar scenarios, decisions, trade-offs, explanation, small modifications, diagnosis, and verification. Avoid syntax, API, framework, and puzzle trivia.

### Stage C — AI-native Work Sample

Typical duration: 60–90 minutes. Provide one unfamiliar, reasonably scoped AI Product Engineering requirement. The normal process is:

`Understand → Research → Plan → Use AI/Codex → Implement → Run → Test → Review Diff → Verify`

AI, search, documentation, and Codex remain allowed. Assess ownership rather than manually typed code volume. The sample may produce evidence for frontend/server boundary, JS/TS/async reasoning, AI-assisted Engineering, Structured Output and/or Tool Calling when appropriate, Testing/Code Review, Product Judgment, and AI UX. Do not force every Phase 0 ability into one artificial task. Use mocks, low-cost models, or realistic substitutes when paid calls are unnecessary.

### Stage D — Technical Defense & Perturbation

Typical duration: 20–40 minutes. This is formal assessment evidence. After Stage C, ask for explanation of key behavior and decisions; change a requirement; introduce or reveal a realistic failure; require diagnosis and/or modification; discuss trade-offs; and verify the changed system. Perturbations may change an output schema, move responsibility between client and server, introduce async failure, return malformed tool data, alter a dependency or UX requirement, expose a subtle bug, or change a business constraint. Tools may remain available. The purpose is to confirm that the learner remains the engineering decision-maker after AI-assisted implementation.

## 5. Evidence Dimensions

Do not use a 0–100 score, global ranking, or total score. Evidence is qualitative and capability-specific. Observe:

- **Understanding**: explains what is happening and why.
- **Judgment**: chooses a reasonable approach for the actual problem.
- **Verification**: determines correctness rather than accepting output.
- **Adaptation**: responds to changed requirements or unfamiliar situations.
- **Tool Use**: identifies investigations, supplies useful context, interprets outputs, rejects weak suggestions, inspects implementation, and verifies behavior.

More prompts, more AI use, or more manual code do not imply stronger performance. Blind delegation is weak evidence.

## 6. Minimum Evidence Rule

Do not derive a level from a simple average. Strong evidence in one dimension cannot compensate for absence of another critical dimension. A fluent explanation does not establish L2 without judgment, modification, or verification. Apply holistic evidence with this Minimum Evidence Rule.

## 7. Phase 0 Capability Status Semantics

P0 may produce `Confirmed L0`, `Confirmed L1`, `Provisional L2`, `Confirmed L2`, or `L3 Candidate`. It must not formally confirm L3 or L4; L4 requires longitudinal cross-project evidence.

- **Confirmed L0**: reliably recognizes purpose and basic boundary, but cannot reliably use it.
- **Confirmed L1**: correctly uses it with examples, normal guidance, documentation, or AI assistance.
- **Provisional L2**: sound understanding, unfamiliar-problem judgment, explain-back after tool use, and one meaningful verification or modification.
- **Confirmed L2**: diversified evidence in more than one meaningful context/stage, including unfamiliar judgment, explanation, verification, and adaptation or modification; at least one piece survives a changed requirement or perturbation.
- **L3 Candidate**: unusually strong P0 evidence of failure diagnosis, cause identification, repair, trade-off analysis, and transfer; it remains a candidate until later project evidence confirms L3.
- **Insufficient Evidence**: do not guess; retain `Not Assessed`, explicitly record insufficient evidence, and route to `VERIFY-IN-PROJECT` or a later targeted check. Never downgrade because evidence was not observed.

## 8. Evidence Sufficiency and Confidence

Evidence Sufficiency is separate from capability level and uses `Sufficient`, `Partial`, `Missing`, or `Conflicting`. Confidence uses only `Low`, `Medium`, or `High`, based on amount, diversity, consistency, and whether evidence survived changed constraints. High confidence is not a high ability level.

When evidence is not sufficient, retain `Not Assessed` and record `Missing` or `Partial` evidence rather than guessing a level.

## 9. Blocking Gaps

A gap is `BLOCKING` only when it prevents safe, meaningful participation in P1: for example, inability to distinguish frontend and server responsibility, safely handle secrets/API keys with guidance, follow the request/async model, or run, inspect, modify, and verify AI-assisted code sufficiently. Most gaps are `NON-BLOCKING`. Prescribe only the smallest coherent remediation needed for early P1; do not create a long prerequisite course without evidence.

## 10. Curriculum Routing

For relevant abilities assign one routing decision: `SKIP` when introductory instruction is unnecessary; `REVIEW` when evidence is unstable or incomplete; `LEARN` for a real gap requiring explicit teaching; or `VERIFY-IN-PROJECT` when natural P1 confirmation is more valuable. Routing never replaces Ability Matrix status.

## 11. Task Quality and Research Judgment

Tasks must represent AI Product Engineering work and prefer embedded evidence. Avoid obscure syntax, version trivia, unrelated knowledge, hidden one-architecture assumptions, and low-product-relevance puzzles. Multiple solutions may be valid; evaluate constraints, reasoning, trade-offs, verification, and actual behavior. Check underspecification before rejecting an unusual answer.

Search is normal engineering behavior. Under AI-assisted Engineering/Tool Use, observe whether the learner identifies what needs research, prefers primary/official documentation when appropriate, checks relevant versions, uses AI as an assistant rather than authority, and verifies information against system behavior. Do not create a separate Ability Matrix row for Research Judgment.

## 12. Fresh Tasks, Metadata, and Privacy

Do not store a live question bank or answer key in this public repository. When formal P0 begins, generate fresh tasks just-in-time; do not publish exact tasks or expected answers before use; use equivalent fresh tasks for reassessment where practical. A run may be named `ASSESSMENT_RUN_001`, but public records store only technical evidence summaries, never complete private transcripts or answer histories.

For meaningful AI-assisted work, record date, assessment-spec version, run ID, task/scenario version, model, coding agent, search availability, approximate time, and material environment constraints. Do not store private conversations, personal-life or medical information, private documents, credentials, API keys, passwords, or full private answers. Example summary: `Async — Provisional L2: diagnosed a missing await, explained error propagation, and verified the fix; transfer evidence still needed.`

## 13. Assessment Run Record and State Transitions

Do not create an assessment run file before formal P0 explicitly starts; after it starts, maintain only the minimum resumable technical state. It contains the minimum state needed to resume: Run ID, spec version, date started, environment metadata, current stage, completed evidence areas, uncertain areas, blocking-gap candidates, and next action.

Before formal P0: Formal Learning `NO`, Formal Assessment `NO`, status `PLANNING`, and no assessment evidence. When the learner explicitly starts P0: Formal Assessment `YES`, Formal Learning `NO`, phase remains P0, and sufficient evidence may update run state, the Ability Matrix, and gap/routing notes. After P0 Exit Gate, update matrix, gaps, routing, CURRENT_STATE, and P1 density; only then select the long-term training product. When P1 begins: Formal Learning `YES`; Formal Assessment is `NO` unless a formal assessment is active.

## 14. Phase 0 Exit Gate

P0 completes only when main-scope abilities have sufficient starting evidence or are explicitly insufficient; deferred abilities remain `Not Yet Assessed`; blocking gaps and early routing are identified; P1 density can be determined; at least one AI-native Work Sample and one Technical Defense/Perturbation are complete; and no L3/L4 was improperly certified. Completion depends on evidence sufficiency, not time or question count.

## 15. Core Philosophy

`Observe → Research → Build → Explain → Modify → Debug → Verify`

The assessment asks whether the learner can use modern AI tools while retaining understanding, judgment, verification, and ownership—not how much syntax they can reproduce without tools.
## 16. Learning During Assessment / Evidence Origin

Phase 0 permits AI, search, documentation, and learning new knowledge. Evidence must distinguish:

- **Initial Evidence**: judgment and understanding demonstrated before help.
- **Assisted Evidence**: performance completed after AI, documentation, hints, or explanation.
- **Ownership Evidence**: after help, whether the learner can re-explain, modify, verify, debug, or transfer the result.

Help does not invalidate assessment, but performance immediately after teaching cannot be treated as independent prior-mastery evidence. Ownership regained after help may inform routing and later capability evidence.

## 17. Assessor Intervention Policy

If the learner is stuck:

1. record the current evidence;
2. allow research;
3. provide a hint when necessary;
4. provide the smallest explanation if progress remains blocked;
5. continue observing modification, verification, debugging, or transfer.

Assessment must not deadlock around one unknown fact. A result explicitly taught during the run is not prior mastery; learning followed by ownership can be valid routing and later-evidence input.


## Evidence Fidelity Refinement

Preserve concrete verified and unverified boundaries, Initial/Assisted/Ownership origin, practical-versus-conceptual evidence, learner corrections, scenario abstraction, and tool/environment failure. Recognition is not independent generation; immediately taught performance is not prior mastery; ownership after help may affect routing.


