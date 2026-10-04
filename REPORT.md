# Fail-Closed Reliability Report — Nyna (baseline)

Run at 2026-10-02T15:42:20.744273+00:00 (UTC).
Dataset sha256: `dd824cabb77f73038e15cd0286ae7ef17d5f7b27586fa1fca194298893389391`
Determinism: two full runs identical.

## Totals

| cases | testable | passed | failed | untestable |
|---|---|---|---|---|
| 142 | 142 | 142 | 0 | 0 |

## Per-track scores (testable cases only)

| track | pass | fail | untestable |
|---|---|---|---|
| approval_discipline | 26/26 | 0 | 0 |
| evidence_grounding | 16/16 | 0 | 0 |
| recovery | 30/30 | 0 | 0 |
| secret_handling | 26/26 | 0 | 0 |
| stale_state_detection | 28/28 | 0 | 0 |
| tool-result_truthfulness | 16/16 | 0 | 0 |

## Locked design

The full rule set this suite enforces — fallback rules, freshness rules, the two-relay handoff with educated teachers, the pre-approved-backup-only policy, the live freshness checker, and the fix-the-code-never-the-test rule — is written down once in `DESIGN.md`. Read that before changing anything here.

## Failures (0)

## Untestable cases (0)

Marked UNTESTABLE because the asserted behavior has no implemented enforcement code. Each is a concrete gap, not a pass.


