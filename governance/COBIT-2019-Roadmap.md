# UPTA — COBIT 2019 Governance Roadmap

## Phase 1 — Complete AI Runtime Evidence

Current priority.

- finish PBM smoke;
- smoke PPU;
- smoke PK;
- smoke LBI;
- smoke LBE;
- smoke PM.

Capture:
- provider calls;
- tokens;
- estimated cost;
- duration;
- retry/repair;
- output validity;
- failure classification.

## Phase 2 — Establish AI Cost Baseline

Produce observed cost profiles for all seven subtests:

- cost per 5 questions;
- projected cost per full package;
- provider calls;
- token usage;
- retry rate;
- average generation time;
- failure rate.

Do not weaken validation or budget controls to make smoke pass.

## Phase 3 — AUD-016 Architecture Rationalization

- audit consumers;
- migrate useful legacy tests;
- prove dead modules are unused;
- remove only proven-dead modules;
- rerun regression.

## Phase 4 — AUD-017 Technical Debt

Audit stub modules and compatibility surfaces.

Decision flow:

consumer search → dependency analysis → active/compatibility/dead classification → removal or implementation → regression.

## Phase 5 — Adaptive Learning Assurance

Run realistic learner scenarios:

- cold start;
- strong learner;
- weak learner;
- mixed skills;
- recent improvement;
- recent degradation;
- insufficient data.

Validate recommendation and difficulty adaptation behavior.

## Phase 6 — Browser Operational Assurance

Validate the end-to-end learner path:

login → package → exam → answer → submission → grading → analytics.

## Phase 7 — Reproducibility

Document and test:

- runtime versions;
- dependencies;
- environment variables;
- database setup;
- seed procedure;
- browser setup;
- startup commands;
- test commands;
- smoke commands.

## Phase 8 — Compliance and Assurance

After the MVP operating context is clearer:

- establish formal legal/compliance scope;
- build privacy/security mapping;
- formalize risk register;
- formalize continuity targets;
- evaluate independent assurance.

## Governance principle

UPTA scales governance with business maturity.

The objective is not to maximize paperwork.

The objective is to make technology:

**useful → controlled → measurable → auditable → resilient.**
