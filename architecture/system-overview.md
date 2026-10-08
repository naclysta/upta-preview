# UPTA — System Architecture Overview

## Product Architecture

~~~
Learner Browser
      |
      v
React / Vite Frontend
      |
      v
FastAPI Application
      |
      +--------------------+
      |                    |
      v                    v
 PostgreSQL            AI Worker
                           |
                           v
                  AI Provider Layer
~~~

## Core Product Flow

~~~
Assessment Contract
        ↓
Subtest Blueprint
        ↓
AI Generation
        ↓
Deterministic QC
        ↓
AI QA
        ↓
Human Review
        ↓
Versioned Question Bank
        ↓
Eligible Package
        ↓
Student Assessment
        ↓
Submission / Grading
        ↓
Analytics
        ↓
Adaptive Learning
~~~

## Governance-relevant architecture principles

### Contract-driven assessment

The canonical assessment contract defines:
- subtest;
- question count;
- duration;
- engine version;
- answer format;
- generation job type.

### Separation of concerns

Question generation, application services, persistence, assessment delivery, and analytics are separated into distinct responsibilities.

### AI is not the final authority

AI generates content.

Application-controlled mechanisms determine whether generated content can proceed:

- schema;
- deterministic QC;
- QA;
- package integrity;
- eligibility;
- grading;
- lifecycle controls.

### Security boundary

Production architecture separates public edge, application services, worker processes, database access, and privileged migration credentials.

### Current maturity note

This architecture is being validated incrementally. Not every subtest or operational scenario has yet received real-provider or production-scale evidence.
