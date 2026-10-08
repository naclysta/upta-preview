# UPTA — AI Governance

## AI Operating Model

UPTA treats AI as a controlled production dependency, not an unchecked content authority.

~~~
Request
  ↓
Budget preflight
  ↓
Generation
  ↓
Schema validation
  ↓
Deterministic QC
  ↓
Independent QA
  ↓
Repair / replacement when justified
  ↓
Package validation
  ↓
Review
~~~

## Cost Controls

The system tracks:

- input tokens;
- output tokens;
- model;
- provider;
- pricing period;
- estimated USD cost;
- estimated IDR cost;
- provider call count.

A per-generation budget is enforced across the generation lifecycle.

## Reliability Controls

Provider behavior is classified rather than treated as generic randomness.

Failure categories include:

- deterministic code bug;
- fixture bug;
- schema/contract bug;
- prompt bug;
- provider/model behavior;
- reviewer/QC issue;
- integration issue;
- environment issue;
- cost/budget issue.

## Provider Strategy

The current architecture supports a primary AI provider with fallback capability.

The exact runtime mix remains subject to ongoing provider validation and cost measurement.

## Runtime Verification

| Subtest | Runtime evidence |
|---|---|
| PU | Full smoke / real-provider |
| PBM | In progress |
| PPU | Pending |
| PK | Pending |
| LBI | Pending |
| LBE | Pending |
| PM | Pending |

## Financial interpretation

Internal estimated AI cost is an engineering planning figure.

It is not represented as a vendor invoice or guaranteed future unit economics.

## Governance Principle

> Maximize useful question quality while keeping AI spending bounded, observable, and recoverable from provider failure.
