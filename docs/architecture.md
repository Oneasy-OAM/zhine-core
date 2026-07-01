# Zhiné Architecture

> Version 0.1  
> Based on Zhiné Global Brand Charter v0.3 and Zhiné Technical Whitepaper v0.3

## 1. Purpose

This document defines the conceptual architecture of Zhiné. It is not a final engineering implementation plan. It clarifies the system layers, module boundaries, data flow, governance control points, model routing principles, and first-stage architectural scope.

Zhiné is an open-source project for building a **Personal Intelligence Companion / 个人智慧伙伴** on top of an **Open Cognitive Architecture / 开放认知架构**.

The core technical object is the **Personal Cognitive Model / 个人认知模型**: a governable personal cognitive asset system composed of memory, knowledge, experience, skills, strategies, benchmarks, adapters, and evolution logs.

---

## 2. Architectural Thesis

Zhiné should not be treated as a single chatbot, a task-execution agent, a local RAG demo, or a wrapper around cloud foundation models.

It should be understood as a layered personal cognitive infrastructure:

```text
User Access
→ Access & Sync
→ Governance Plane
→ Cognitive Runtime
→ Personal Cognitive Assets
→ Growth Mechanism
→ Model Execution
```

The architectural goal is to help each individual own, govern, migrate, evaluate, and evolve their personal intelligence assets over time.

---

## 3. High-Level Architecture

```text
┌──────────────────────────────────────────────┐
│                 User Access Layer             │
│   Mobile / Desktop / Web / Browser / Local UI │
└──────────────────────────────────────────────┘
                        │
┌──────────────────────────────────────────────┐
│                Access & Sync Layer            │
│   Identity / Device / Session / Sync / Recovery│
└──────────────────────────────────────────────┘
                        │
┌──────────────────────────────────────────────┐
│                 Governance Plane              │
│   Permission / Audit / Security / Versioning   │
│   Data Classification / Rollback / Deletion    │
└──────────────────────────────────────────────┘
                        │
┌──────────────────────────────────────────────┐
│                Cognitive Runtime              │
│   Reasoning / Planning / Tools / Memory / RAG  │
│   Reflection / Critic / Evaluation / Routing   │
└──────────────────────────────────────────────┘
                        │
┌──────────────────────────────────────────────┐
│              Personal Cognitive Assets        │
│   Memory / Knowledge / Skills / Strategies    │
│   Benchmarks / Adapters / Evolution Logs      │
└──────────────────────────────────────────────┘
                        │
┌──────────────────────────────────────────────┐
│                 Growth Mechanism              │
│   Experience Extraction / Skill Formation      │
│   Strategy Refinement / Benchmark Update       │
└──────────────────────────────────────────────┘
                        │
┌──────────────────────────────────────────────┐
│                Model Execution Layer          │
│   Local LLM / Embedding / Reranker / Router    │
│   Remote Teacher by Permission                │
└──────────────────────────────────────────────┘
```

---

## 4. Layer Definitions

| Layer | Responsibility | First-Stage Scope |
|---|---|---|
| User Access Layer | Provides user-facing interaction entry points | Web UI, local UI, CLI prototype |
| Access & Sync Layer | Manages identity, devices, sessions, sync, recovery | Local identity, local data directory, export / import |
| Governance Plane | Enforces permission, audit, data classification, versioning, rollback | Permission gates, audit log, memory rollback |
| Cognitive Runtime | Coordinates reasoning, planning, tools, memory, RAG, routing, evaluation | Minimal orchestrator, memory retrieval, model router |
| Personal Cognitive Assets | Stores long-term personal memory, knowledge, skills, strategies, benchmarks, adapters, logs | Memory store, personal knowledge base, evolution log |
| Growth Mechanism | Converts tasks into reusable experience and skill updates | Experience extraction, skill cards, strategy rules |
| Model Execution Layer | Runs local models and permitted remote teacher models | Local LLM integration, remote model adapter, router |

---

## 5. Core Modules

### 5.1 Zhiné Core

Zhiné Core is the cognitive runtime. It coordinates task understanding, model routing, tool use, memory retrieval, RAG, reflection, evaluation, and growth updates.

It should remain model-agnostic, tool-agnostic, storage-agnostic, and cloud-optional.

### 5.2 Zhiné Memory

Zhiné Memory stores governable personal memory. It should support provenance, confidence, sensitivity level, permission control, audit, deletion, conflict handling, and rollback.

Memory is not chat history. It is a personal intelligence asset.

### 5.3 Zhiné Knowledge

Zhiné Knowledge manages personal documents, notes, research materials, project files, and knowledge structures. It supports retrieval, indexing, metadata, and user-controlled import / export.

### 5.4 Experience Engine

The Experience Engine turns tasks, feedback, success, failure, and corrections into reusable experience. Its output may become skill cards, strategy rules, benchmark samples, or training candidates.

### 5.5 Skill Graph

The Skill Graph represents reusable personal capabilities as composable, evaluable, and versioned skill nodes.

A skill node should include scenario, input, output, procedure, dependencies, success metrics, failure modes, and version history.

### 5.6 Strategy Library

The Strategy Library records user-preferred ways of thinking, judging, planning, deciding, writing, researching, and solving problems.

Strategy rules must be auditable and reversible.

### 5.7 Personal Benchmark

Personal Benchmark is used to verify whether Zhiné is actually becoming more useful to the individual.

Growth must be measured, not merely claimed.

### 5.8 Evolution Log

Evolution Log records every meaningful update to memory, knowledge, skills, strategies, benchmarks, adapters, and governance state.

No major growth should happen without an evolution event.

### 5.9 Model Router

The Model Router chooses between local models, remote teacher models, and mixed workflows based on sensitivity, permission, complexity, cost, latency, confidence, and safety.

### 5.10 Access & Sync

Access & Sync supports continuity across devices and contexts without making cloud storage the default owner of personal data.

First-stage scope should focus on local identity, data directory structure, export, import, and recovery.

---

## 6. Personal Cognitive Asset Model

| Asset | Description | Governance Requirement |
|---|---|---|
| Personal Memory | Facts, preferences, goals, lessons, values, task history | Provenance, permission, confidence, deletion, rollback |
| Personal Knowledge Base | Documents, notes, project materials, research resources | Import / export, metadata, indexing, source tracking |
| Experience Events | Task outcomes, feedback, lessons, failure analysis | Review status, training eligibility, conversion rules |
| Skill Cards | Reusable capability units | Versioning, success metrics, failure modes |
| Strategy Rules | Preferred thinking and action patterns | Scope, priority, status, audit trail |
| Personal Benchmarks | Evaluation samples and scoring rules | Baseline, regression tests, release gates |
| Personal Adapters | LoRA, adapters, preference models, routing policies | User ownership, license compliance, evaluation gate |
| Evolution Logs | Records of asset changes | Integrity, traceability, rollback availability |

---

## 7. Data Flow

### 7.1 Task Execution Flow

```text
User task
→ Task understanding
→ Permission and sensitivity check
→ Memory and knowledge retrieval
→ Model routing
→ Local or remote-assisted reasoning
→ Output generation
→ Evaluation and feedback
→ Experience extraction
→ Asset update proposal
→ User / policy approval
→ Evolution log
```

### 7.2 Growth Flow

```text
Task result
→ Feedback
→ Error or success analysis
→ Experience event
→ Skill / strategy candidate
→ Personal benchmark update if needed
→ Evaluation
→ Versioned asset update
→ Rollback point
```

### 7.3 Remote Teacher Flow

```text
Task requires remote assistance
→ Data sensitivity check
→ User permission / policy gate
→ Redaction if needed
→ Remote teacher call
→ Local validation / critic review
→ Result integration
→ Audit log
```

Remote teacher models should enhance the local personal model. They should not become the owner of personal memory or personal cognitive assets.

---

## 8. Model Routing Principles

Routing priority:

```text
Safety and permission
> Explicit user instruction
> Data sensitivity
> Task complexity
> Quality requirement
> Cost and latency
> Model availability
```

| Situation | Preferred Route |
|---|---|
| Highly private personal data | Local model only |
| Routine personal tasks | Local model first |
| Large batch processing | Local model first |
| High-stakes output | Multi-step validation, critic review, possible remote teacher by permission |
| Latest technical research | Remote teacher by permission, with source tracking |
| Low local confidence | Escalate to remote teacher by permission |
| Sensitive but complex task | Redact, summarize, or keep local depending on policy |

---

## 9. Governance Plane

The Governance Plane is not an optional security layer. It is part of the cognitive architecture.

It must cover:

- user permission;
- data classification;
- remote call control;
- memory update control;
- tool permission;
- audit trail;
- versioning;
- deletion;
- rollback;
- fairness and accessibility review.

### Non-Negotiable Rules

```text
No authorization, no use of personal data.
No provenance, no durable memory.
No evaluation, no growth release.
No versioning, no model upgrade.
No rollback, no deployment.
No permission, no remote inference for sensitive data.
```

---

## 10. First-Stage Architecture

Phase 1 should validate a minimal personal evolution loop rather than attempt a complete ecosystem.

Required modules:

| Module | Priority | Description |
|---|---|---|
| Local Model Runtime | P0 | Run local LLM and embedding models |
| Remote Model Adapter | P0 | Connect remote teacher models with permission control |
| Personal Memory Store | P0 | Store structured personal memory with governance fields |
| Personal Knowledge Base | P0 | Ingest and retrieve personal documents |
| Model Router | P0 | Decide local, remote, or mixed execution |
| Experience Engine | P0 | Extract task lessons and reusable experience |
| Evolution Log | P0 | Record updates and rollback points |
| Reflection Engine | P1 | Analyze errors, improvements, and strategy updates |
| Skill Store | P1 | Store initial skill cards |
| Personal Benchmark | P1 | Verify improvement and prevent regression |
| Access Layer v0.1 | P1 | Provide local identity, export, import, and recovery |

---

## 11. Excluded from Phase 1

The following should not be included in the first engineering phase unless explicitly justified:

- unconstrained autonomous self-training;
- automatic model weight updates without evaluation;
- public sharing of personal memory;
- cloud-first personal data storage;
- broad plugin marketplace;
- claims about consciousness, personality copying, or digital soul;
- production-grade multi-device encrypted sync before local governance is stable.

---

## 12. Architecture Acceptance Criteria

Phase 1 architecture should be considered valid only if it demonstrates:

1. personal memory can be stored, retrieved, corrected, deleted, and rolled back;
2. personal documents can be indexed and retrieved under user control;
3. local model execution works for ordinary personal tasks;
4. remote teacher calls require permission and can be audited;
5. task experience can be converted into reusable skill or strategy candidates;
6. growth can be evaluated through personal benchmark samples;
7. personal cognitive assets can be exported and restored;
8. sensitive data is local by default;
9. the system can explain why it remembered, ignored, updated, or escalated something;
10. basic fairness, accessibility, and multilingual considerations are visible in design and testing.

---

## 13. Open Questions

The following questions require further engineering design:

- What is the minimum viable memory schema?
- What data store should be used for first-stage local memory?
- How should memory conflicts be resolved?
- What is the first personal benchmark format?
- What counts as a skill update versus a strategy update?
- How should remote teacher responses be audited and redacted?
- What should be exportable in the first release?
- How should local model limitations be communicated to users?
- How should fairness and accessibility be tested in a personal AI system?

---

## 14. Summary

Zhiné architecture is not a model pipeline. It is a personal cognitive infrastructure.

Its core task is to make personal intelligence assets:

```text
ownable
portable
governable
evaluable
recoverable
evolvable
fairly accessible
```

The first engineering goal is not to build everything. It is to prove that a personal AI system can remember, reason, learn, evaluate, and grow under user sovereignty.
