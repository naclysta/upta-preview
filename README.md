# UPTA — Investor Preview

Public-facing governance and product overview for UPTA Beta.

> **Important:** This repository is an investor-facing transparency layer. It is not the private engineering repository and does not contain production secrets, credentials, private learner data, or internal implementation details.

## What is UPTA?

UPTA is an AI-assisted UTBK-SNBT learning and assessment platform focused on structured question generation, quality control, assessment delivery, analytics, and adaptive learning.

UPTA is currently at **MVP / pre-client stage**.

## Governance Position

UPTA currently uses COBIT 2019 as an internal governance-system design reference.

This repository **does not claim COBIT 2019 certification or formal compliance**.

The current assessment focuses on evidence-based alignment in areas such as:

- risk optimization;
- resource and AI cost optimization;
- security;
- architecture;
- quality management;
- operational controls;
- internal control;
- monitoring and assurance.

## Current Verification Snapshot

| Area | Current state |
|---|---|
| PU AI runtime | Full smoke / real-provider testing completed |
| PBM AI runtime | Smoke / real-provider testing in progress |
| PPU AI runtime | Pending |
| PK AI runtime | Pending |
| LBI AI runtime | Pending |
| LBE AI runtime | Pending |
| PM AI runtime | Pending |
| AI cost telemetry | Implemented; full seven-subtest baseline pending |
| Security controls | Implemented with regression/runtime evidence in audited areas |
| Adaptive learning empirical validation | Pending |
| Browser E2E | Existing evidence; broader runtime validation continues |
| Formal external compliance assessment | Not yet performed |
| Independent assurance | Not yet performed |

## Documents

- [COBIT 2019 Design Assessment](governance/COBIT-2019-Design-Assessment.md)
- [COBIT 2019 Evidence Matrix](governance/COBIT-2019-Evidence-Matrix.md)
- [Governance Roadmap](governance/COBIT-2019-Roadmap.md)
- [Architecture Overview](architecture/system-overview.md)
- [AI Governance](architecture/ai-governance.md)

## Evidence Principle

UPTA uses a strict evidence hierarchy:

**IMPLEMENTED → TESTED → VERIFIED → PRODUCTION-READY**

A control is not described as verified merely because the implementation looks reasonable.

## COBIT Reference

The COBIT 2019 design approach uses design factors to tailor a governance system to enterprise context and prioritize the 40 governance and management objectives.

Reference: https://www.isaca.org/resources/cobit
