# State Protocol

## State File Responsibilities

- `CURRENT_STATE.md`: current learning lifecycle position, active phase, blockers, and next action; not a detailed execution plan or learning history.
- `ABILITY_MATRIX.md`: current effective capability status, evidence boundary, confidence, targets, priorities, and verification gaps; not a project checklist.
- `ASSESSMENT_SPEC.md`: the operating specification for Phase 0 evidence gathering.
- `ASSESSMENT_RUN_*.md`: historical assessment-evidence snapshots.
- `LEARNING_LOG.md`: historical learning events.
- `PROJECT_STATE.md`: project delivery state, separate from learning state.
- `CURRICULUM.md`: long-term target capabilities and Phase structure.
- `PHASE_EXECUTION_PLAN.md`: current Phase's concrete execution plan; historical versions remain in Git history.
- `TEACHING_PROTOCOL.md`: teaching behavior.
- `REVIEW_QUEUE.md`: re-verification and review needs.
- `CHANGELOG.md`: versions of course and operating specifications.

## Single Source of Truth

`CURRENT_STATE.md` determines the current lifecycle state. `ABILITY_MATRIX.md` determines the current capability conclusion. `ASSESSMENT_RUN_*.md` and `LEARNING_LOG.md` are historical evidence: they may explain why a baseline status was assigned, but MUST NOT override, downgrade, or replace later Matrix evidence. If the current Matrix conflicts with an older run record, the newer Matrix is authoritative unless the Matrix or run is explicitly marked corrupted or under reassessment. Project completion never proves mastery. `CURRENT_STATE.md` is authoritative for lifecycle state, blockers, and next action; `PHASE_EXECUTION_PLAN.md` is authoritative for the current Phase's execution route; `CURRICULUM.md` is authoritative for long-term structure. Conflicts otherwise resolve as: current repository state files > committed history > conversation memory > model inference.

## Operating States

### Planning

Formal Learning: `NO`; Formal Assessment: `NO`; no formal evidence yet.

### Phase 0 Formal Assessment

Formal Learning: `NO`; Formal Assessment: `YES`; assessment evidence is valid, the Ability Matrix may update when evidence is sufficient, and an assessment run state may be maintained.

### Post-P0 / Pre-P1

Formal Learning: `NO`; Formal Assessment: `NO`; Phase 0 Assessment Completed: `YES`; baseline evidence exists; learner is ready for P1; and the P1 training product may be selected or confirmed. Do not return this state to P0 planning or repeat P0 assessment unless reassessment is explicitly requested.

### P1+ Formal Learning

Formal Learning: `YES`; Formal Assessment is `YES` or `NO` depending on whether a formal assessment is active.

## Archival

After a formal learning session, project milestone, or formal Phase 0 assessment checkpoint, record only actual completion, evidence, unresolved risks, review/re-verification needs, the next minimal action, and any route deviation with reason. Do not record plans as completion. Phase 0 assessment may be checkpointed even while Formal Learning remains `NO`.
