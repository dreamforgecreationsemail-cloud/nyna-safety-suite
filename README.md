# Nyna Fail-Closed Safety Suite

**By DreamForge. Jack Berry, visioneer.**

This is the public proof for Nyna's safety testing: every test case, every
result. Nothing hidden, nothing padded.

## The scorecard

| Suite | Cases | Passed | Failed | Untestable |
|-------|-------|--------|--------|------------|
| Fixed regression | 250 | 250 | 0 | 0 |
| Gauntlet — standard | 1,000 | 1,000 | 0 | 0 |
| Gauntlet — torture | 1,000 | 1,000 | 0 | 0 |
| **Total** | **2,250** | **2,250** | **0** | **0** |

Zero failures. Zero untestable. Deterministic across runs — same seed,
same exam, same results, every time.

## What this is

A fail-closed safety gauntlet for Nyna, an AI built by Jack Berry. The
fixed suite is 250 hand-built cases. The gauntlet is a random exam
generator: 10 levels of 100 standard cases, then 10 levels of 100 torture
cases — 2,000 generated instances per full run, drawn from approximately
336 scenario templates (247 standard + 89 torture) across 40+ sectors:
healthcare, legal, finance, construction, education, retail, and more.
The values change every run; the underlying situations are the templates.

Every case has a real oracle — not a vibe check. Pass or fail, verifiable
by anyone who reads the case and the result.

## The method

We never weaken a test to get a pass. The suite is the alarm. When it
goes off, we fix the fire — not the alarm. Every failure gets folded back
in and makes her stronger.

The journey, honestly reported:
- 84/84 with 30 gaps we didn't hide — cases we couldn't test because the
  enforcement code didn't exist yet
- 98/98 with 16 gaps
- 114/114 — every original case testable and passing
- 250/250 — the fixed regression suite, zero failures
- 2,000/2,000 — the full gauntlet, standard and torture, zero failures

## What's in this repo

- `cases/` — every test case: the scenario, the expected behavior
- `results/` — every verified run result
- `README.md` — this file

## What's not in this repo

The enforcement machinery — how she passes — is proprietary and stays
private. This repo is the proof, not the engine. Scorecard in public,
engine in private.

## The rule going forward

Every real failure she ever has becomes a permanent test. The suite only
gets meaner.

---

Built from a phone. Tested like it matters. Because it does.
