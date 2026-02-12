# FHNW BSc BAI -- AI-assisted Software Development

Welcome to the official GitHub organization of the module **AI-assisted Software Development** in the **BSc Business Artificial Intelligence (BAI)** program at FHNW.

This organization hosts:

-   Reference implementations (e.g., BAIssue)
-   Capstone project repositories
-   Architecture examples
-   CI/CD templates
-   AI-assisted SDLC documentation
-   Tooling and workflow standards

---

# AI-Assisted Software Development Life Cycle (AI-SDLC)

This document describes the AI-Assisted SDLC used in this project.  
It aligns with:

- Clean Architecture principles
- Test-Driven Development (TDD)
- Spec-Driven Development (SDD)
- CI/CD practices
- SAFe-compatible iterative delivery
- AI-assisted engineering (completion, vibe coding, agentic coding)

---

## Overview

The AI-Assisted SDLC is iterative and quality-driven.  
Architecture and tests are defined **before** implementation.  
AI tools assist throughout the process, but engineering responsibility remains with the team.

---

## Process Model

(1) Business Use Case / Epic Definition  
        ↓  
(2) Requirement & Spec-Driven Development (SDD)  
        ↓  
(3) AI-Assisted Architecture Definition / Validation  
        ↓  
(4) AI-Assisted Test-Driven Development (TDD)  
        ↓  
(5) AI-Assisted Implementation & Local Unit Testing  
        ↺ Iteration back to 2–4  
        ↓  
(6) Continuous Integration & Multi-Level Testing  
        ↺ Iteration back to 2–5  
        ↓  
(7) Containerized Release Build & End-to-End Testing  
        ↺ Iteration back to 2–5  
        ↓  
(8) Continuous Deployment  
        ↓  
(9) Operation, Monitoring & Feedback  
        ↺ Feedback back to 1–2  

---

## Phase Descriptions

### 1. Business Use Case / Epic Definition

- Define business value  
- Create epics, features, or user stories  
- Define acceptance criteria  
- Track work via GitHub Issues or Boards  

No implementation work happens here.

---

### 2. Requirement & Spec-Driven Development (SDD)

Before writing code:

- Define API contracts (e.g., OpenAPI)  
- Define domain concepts and entities  
- Define acceptance criteria formally  
- Document architectural intent (e.g., in AGENTS.md)  

Specification precedes implementation.

---

### 3. AI-Assisted Architecture Definition / Validation

Define or validate:

- Domain layer (entities)  
- Application layer (use cases/services)  
- Interface layer (API boundaries)  
- Infrastructure layer (database, frameworks)  

Dependency direction must follow Clean Architecture rules.

AI may suggest structures, but decisions remain architectural decisions.

---

### 4. AI-Assisted Test-Driven Development (TDD)

Before implementing use cases:

- Write or generate unit tests  
- Define integration scenarios  
- Define E2E scenarios  

Tests represent executable specifications.

---

### 5. AI-Assisted Implementation & Local Unit Testing

Only after requirements, architecture, and tests are defined:

- Implement use cases  
- Keep business logic framework-independent  
- Ensure unit tests pass locally  

If inconsistencies arise, iterate back to previous phases.

---

### 6. Continuous Integration & Multi-Level Testing

On every push:

- Run unit tests  
- Run integration tests  
- Validate architecture constraints  

CI enforces built-in quality.

---

### 7. Containerized Release Build & End-to-End Testing

Before release:

- Build Docker image  
- Run container  
- Execute E2E tests against the running artifact  

The deployable artifact is tested, not only the source code.

---

### 8. Continuous Deployment

- Tag-based releases  
- Docker image publishing  
- Cloud deployment  

Deployment is automated but controlled.

---

### 9. Operation, Monitoring & Feedback

- Health checks  
- Logging  
- Observability  
- User feedback  

Feedback loops create new requirements.

---

## AI Usage Guidelines

AI tools may be used for:

- Architecture proposals  
- Test generation  
- Code scaffolding  
- Refactoring suggestions  
- Documentation assistance  

However:

- Developers remain responsible for correctness.  
- Generated code must be reviewed.  
- Architecture decisions must be justified.

---

## Quality Principles

This AI-Assisted SDLC enforces:

- Specification before implementation  
- Tests before business logic  
- Clean separation of concerns  
- Automated quality gates  
- Deployable artifacts validated before release  
- Continuous learning and iteration  

---

## Alignment with Clean Architecture

The SDLC directly supports the architectural structure:

- Domain: protected by unit tests  
- Application: tested via integration tests  
- Interfaces: validated via API and contract tests  
- Infrastructure: validated through containerized E2E testing  

---

## Summary

This AI-Assisted SDLC ensures:

- Structured agility  
- Built-in quality  
- Architecture-first thinking  
- Responsible AI usage  
- Continuous improvement  

It is intentionally lightweight but disciplined.

---

## Educational Objective

The goal of this module is not only to build software but to understand how AI transforms the software engineering process.

Students learn to:

-   Structure enterprise applications
-   Apply TDD and SDD rigorously
-   Integrate CI/CD pipelines
-   Use AI responsibly and effectively
-   Reflect on tooling decisions

---

© FHNW -- BSc Business Artificial Intelligence
