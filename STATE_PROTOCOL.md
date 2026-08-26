# State Protocol

## State File Responsibilities

- `CURRENT_STATE.md`: sole current learning progress and next action.
- `ABILITY_MATRIX.md`: capability evidence, confidence, targets, priorities, and verification gaps; not a project checklist.
- `ASSESSMENT_SPEC.md`: the operating specification for Phase 0 evidence gathering.
- `REVIEW_QUEUE.md`: review or re-verification needs.
- `PROJECT_STATE.md`: project delivery state, separate from learning state.
- `LEARNING_LOG.md`: learning history.
- `CHANGELOG.md`: versions of course and operating specifications.

## Single Source of Truth

Current state is `CURRENT_STATE.md`; capability conclusions require evidence in `ABILITY_MATRIX.md`; project completion never proves mastery. Conflicts resolve as: current repository state files > committed history > conversation memory > model inference.

## Operating States

### Planning

Formal Learning: `NO`; Formal Assessment: `NO`; no formal evidence yet.

### Phase 0 Formal Assessment

Formal Learning: `NO`; Formal Assessment: `YES`; assessment evidence is valid, the Ability Matrix may update when evidence is sufficient, and an assessment run state may be maintained.

### P1+ Formal Learning

Formal Learning: `YES`; Formal Assessment is `YES` or `NO` depending on whether a formal assessment is active.

## Archival

After a formal learning session, project milestone, or formal Phase 0 assessment checkpoint, record only actual completion, evidence, unresolved risks, review/re-verification needs, the next minimal action, and any route deviation with reason. Do not record plans as completion. Phase 0 assessment may be checkpointed even while Formal Learning remains `NO`.
