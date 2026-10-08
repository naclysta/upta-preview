# UPTA — COBIT 2019 Design Assessment

**Assessment type:** Internal COBIT 2019 alignment and governance-system design  
**Lifecycle:** MVP / Pre-client  
**Basis:** UPTA engineering repository evidence, documented audit evidence, regression evidence, and available runtime/provider evidence.

## 1. Assessment Boundary

This document follows the COBIT 2019 design-factor concept. COBIT 2019 defines 11 design factors that influence governance-system design and uses them to prioritize the 40 governance and management objectives.

This is an **internal design assessment**, not certification.

## 2. UPTA Design Factors

### DF1 — Enterprise Strategy
**Indicator: 9/10**

**Rationale:** UPTA's product is fundamentally digital and differentiates through assessment technology, AI-assisted content generation, analytics, and adaptive learning. Cost efficiency is also strategically important because AI is a variable operating cost.

**Evidence:** Product architecture and AI generation pipeline are core product components.

### DF2 — Enterprise Goals
**Indicator: 9/10**

**Priority themes:**
- product/service quality: 10
- managed technology risk: 10
- learner-oriented service: 9
- operational excellence: 9
- digital transformation: 10
- cost optimization: 9

**Rationale:** UPTA's value depends on correct questions, reliable assessment delivery, useful analytics, and sustainable AI costs.

### DF3 — Risk Profile
**Indicator: 10/10**

**Key risks:**
- AI/provider failure: 10
- security breach: 10
- unauthorized access: 10
- incorrect generated content: 10
- cost overrun: 10
- data integrity: 10
- third-party dependency: 9
- operational failure: 9
- adaptive-learning error: 9

**Evidence:** Authentication, authorization, CSRF protection, rate limiting, AI budget enforcement, deterministic QC, independent QA, package eligibility validation, audit events, logging, and regression testing are present in the engineering system.

### DF4 — I&T-Related Issues
**Indicator: 10/10**

**Known issues:**
- incomplete runtime validation across AI engines;
- provider dependency;
- AI cost baseline not yet complete;
- legacy module duplication;
- adaptive-learning empirical validation pending;
- browser/runner reproducibility work;
- CI resource constraints.

**Rationale:** These issues directly affect product reliability and operating cost.

### DF5 — Threat Landscape
**Indicator: 8/10**

**Rationale:** UPTA is an internet-facing authenticated web platform with administrative functions and external AI dependencies.

**Evidence:** Security boundaries include authentication, authorization, CSRF controls, rate limiting, secure session handling, and edge hardening.

### DF6 — Compliance Requirements
**Indicator: UNKNOWN**

**Rationale:** The current assessment does not have enough evidence to establish final legal entity scope, contractual client requirements, or complete sector/privacy regulatory applicability.

### DF7 — Role of IT
**Indicator: 10/10**

**Classification:** Strategic / Core Product

**Rationale:** Technology is not merely a support function. The product itself is software, assessment logic, AI generation, analytics, and adaptive learning.

### DF8 — Sourcing Model for IT
**Indicator: 8/10**

**Model:**
- insourced engineering;
- cloud infrastructure;
- third-party AI provider;
- external identity integration.

**Rationale:** External dependencies create operational, pricing, and availability risk.

### DF9 — IT Implementation Methods
**Indicator: 9/10**

**Methods observed:**
- iterative development;
- automated regression testing;
- local-first verification;
- selective CI/CD;
- evidence-driven technical audit.

**Rationale:** These methods are appropriate for a fast-moving MVP while maintaining verification discipline.

### DF10 — Technology Adoption Strategy
**Indicator: 9/10**

**Rationale:** AI is a core capability rather than a cosmetic feature. UPTA uses AI generation, automated review, provider failover, cost telemetry, and adaptive-learning logic.

### DF11 — Enterprise Size
**Indicator: UNKNOWN**

**Rationale:** Formal headcount, organizational structure, revenue scale, and production customer scale are not yet sufficiently evidenced in the current assessment.

## 3. Priority Interpretation

The 1–10 indicators above are **UPTA-specific governance priority indicators** used for this assessment. They are not an official COBIT score.

### Critical priority objectives

- EDM03 — Ensured Risk Optimization
- EDM04 — Ensured Resource Optimization
- APO06 — Managed Budget and Costs
- APO11 — Managed Quality
- APO12 — Managed Risk
- APO13 — Managed Security
- BAI03 — Managed Solutions Identification and Build
- DSS01 — Managed Operations
- DSS05 — Managed Security Services
- DSS06 — Managed Business Process Controls
- MEA01 — Managed Performance and Conformance Monitoring
- MEA02 — Managed System of Internal Control

### High priority objectives

EDM01, EDM02, APO01, APO03, APO04, APO09, APO10, BAI02, BAI04, BAI06, BAI07, DSS02, DSS03, DSS04, MEA04.

### Medium priority objectives

APO05, BAI01, BAI05, BAI08, BAI09, BAI10.

### UNKNOWN / pending

EDM05, APO02, APO07, APO08, MEA03.

## 4. Capability Targets

Capability levels use a separate COBIT 0–5 concept and must not be confused with the UPTA 1–10 priority indicator.

| Capability target | Purpose |
|---|---|
| Level 4 | Critical controls requiring predictable operation |
| Level 3 | Established processes appropriate to the MVP |
| Level 2 | Managed processes where evidence is still developing |
| UNKNOWN | Insufficient evidence for a defensible target |

The current target philosophy is deliberately conservative: do not assign high capability targets without the evidence required to sustain them.

## 5. Current Governance Position

**PARTIAL COBIT 2019 ALIGNMENT — STRONG ENGINEERING FOUNDATION**

Strongest current areas:
- security;
- risk management;
- AI cost governance;
- architecture;
- quality controls;
- internal controls;
- monitoring.

Main gaps:
- runtime validation for all AI subtests;
- complete AI cost baseline;
- adaptive-learning empirical validation;
- formal compliance mapping;
- stakeholder evidence;
- independent assurance.

## Investor-safe statement

> UPTA Beta has established an evidence-driven technical governance foundation that aligns with relevant COBIT 2019 governance and management objectives for its current MVP lifecycle. UPTA does not claim COBIT 2019 certification or formal compliance. Governance maturity is being developed incrementally, with technical controls prioritized ahead of enterprise-scale governance overhead.
