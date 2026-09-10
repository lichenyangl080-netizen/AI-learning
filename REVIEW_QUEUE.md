# Review Queue

Only open verification needs belong here. An item does not trigger theory re-teaching, change `ABILITY_MATRIX.md`, or create an independent Exit Gate unless the current product or `CURRICULUM.md` requires it.

## Current Open Evidence

- P3 deeper cross-project Context / Capability / Tool / Skill / Harness / Eval transfer — natural, nonblocking verification opportunity; P3 Exit Gate is already `PASSED`.

## Deferred External Access

P1 remains not formally `PASSED`; complete these when Provider API access becomes available:

- Real Provider Model API call with API Key / Secret-boundary handling.
- Real Structured Output with runtime validation and at least one failure path.
- Real `UI → Server → Provider → Model Output → Validation → UI` integration.
- Real Provider Tool Calling only when the actual integration requires it; otherwise it remains optional verification evidence.

Do not store credentials. P1 Exit Gate requirements remain defined by `CURRICULUM.md`.

## Natural Support Verification

Verify only when encountered in a real P6/P7/P8 product:

- P4: external API contract and integration boundary; source/cache/sync conflicts; RAG grounding and failure attribution; API/MCP/Computer Use selection; persistent-state ownership.
- P5: permissions, side effects, security, retry/recovery, observability, deployment and reliability.
- P3: Context, Capability/Tool, Skill, Memory, Harness and Eval transfer beyond the current practical validation.

Future verification candidates remain nonblocking until required by the actual product or current mainline Exit Gate. Formal lifecycle state is determined by `CURRENT_STATE.md`.
