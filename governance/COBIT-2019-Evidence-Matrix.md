# UPTA — COBIT 2019 Evidence Matrix

## Evidence IDs

| ID | Evidence | Supports |
|---|---|---|
| EV-001 | Canonical assessment contract | EDM01, APO03, BAI02, MEA02 |
| EV-002 | Active generator registry | APO03, BAI03, MEA01, MEA02 |
| EV-003 | AI generation budget and cost enforcement | EDM03, EDM04, APO06, APO12, MEA01 |
| EV-004 | Version-controlled AI pricing model and telemetry | EDM04, APO06, APO10 |
| EV-005 | Authentication, authorization, CSRF, rate limits, edge controls | EDM03, APO12, APO13, DSS05, DSS06 |
| EV-006 | Regression test suite | APO11, BAI06, MEA01, MEA02 |
| EV-007 | Provider-backed AI smoke tooling | EDM04, DSS01, MEA01 |
| EV-008 | Package eligibility and integrity controls | BAI02, BAI03, DSS06, MEA02 |
| EV-009 | Operational architecture and worker/database separation | APO03, BAI04, DSS01, DSS04 |
| EV-010 | Evidence-driven engineering audit process | EDM01, APO01, APO12, MEA02, MEA04 |

## Runtime Evidence Status

| Subtest | Evidence status |
|---|---|
| PU | Full smoke / real-provider testing completed |
| PPU | Pending |
| PBM | Smoke / real-provider testing in progress |
| PK | Pending |
| LBI | Pending |
| LBE | Pending |
| PM | Pending |

## Evidence quality rule

**Static inspection** → implementation evidence

**Unit/regression test** → tested evidence

**Provider/runtime smoke** → runtime evidence

**Production deployment / real stakeholder operation** → production evidence

No layer is automatically promoted to the next layer.

## Key disclosed limitations

1. UPTA is still MVP / pre-client.
2. Five AI subtests do not yet have runtime/provider evidence.
3. PBM runtime testing is still in progress.
4. Full AI cost baselines across all seven subtests are not yet established.
5. Formal external compliance mapping has not been completed.
6. Independent external assurance has not been performed.
