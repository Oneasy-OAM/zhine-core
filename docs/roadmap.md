# Zhiné Roadmap

> Version 0.1  
> A phased roadmap for moving Zhiné from charter and whitepaper into an open-source project.

## 1. Purpose

This roadmap defines the staged development direction of Zhiné. It is not a fixed product delivery schedule. It is a technical and community path for validating the Zhiné thesis step by step.

The roadmap should remain conservative. Zhiné should first prove a minimal personal evolution loop before attempting broad automation, self-training, ecosystem expansion, or multi-device production deployment.

---

## 2. Roadmap Principles

1. Do not overbuild before the architecture is clear.
2. Do not train before data governance is clear.
3. Do not sync widely before local ownership is clear.
4. Do not build ecosystem features before core protocols are stable.
5. Do not claim growth unless evaluation can prove it.
6. Do not compromise user sovereignty for convenience.
7. Do not let AI become a privilege of the few.

---

## 3. Phase Overview

| Phase | Name | Goal |
|---|---|---|
| Phase 0 | Project Definition | Clarify brand, technical thesis, architecture, and governance principles |
| Phase 1 | Minimal Working Prototype | Validate personal memory, personal knowledge, local model, remote teacher, experience extraction, and reuse |
| Phase 2 | Protocols and Evaluation | Build memory governance, skill graph, benchmark protocol, model routing, safety guard, and access continuity |
| Phase 3 | Personal Model Adaptation | Add controlled training candidates, adapters, distillation, evaluation gates, and model registry |
| Phase 4 | Open Ecosystem | Enable community skills, plugins, memory backends, model backends, benchmarks, and applications |

---

## 4. Phase 0: Project Definition

### Goal

Make the project direction clear before engineering implementation.

### Deliverables

| Deliverable | Description |
|---|---|
| `docs/charter.md` | Brand positioning, core lines, principles, and expression boundaries |
| `docs/whitepaper.md` | Technical thesis, system definition, architecture, risks, and roadmap |
| `README.md` | GitHub entry document |
| `docs/architecture.md` | Conceptual system architecture |
| `docs/principles.md` | Engineering and ethical principles |
| `docs/roadmap.md` | Development direction and phase criteria |
| `docs/governance.md` | Initial governance model |
| `docs/ai-ethics.md` | Inclusive AI, fairness, accessibility, and anti-discrimination principles |
| Initial specs | Personal memory, evolution log, personal benchmark protocol |

### Exit Criteria

Phase 0 is complete when:

1. the project can be explained clearly in one README;
2. the architecture has stable conceptual layers;
3. personal cognitive assets are defined;
4. local-first and user ownership principles are explicit;
5. the project has clear boundaries around consciousness, privacy, training, and remote models;
6. minimum contribution and governance rules exist.

---

## 5. Phase 1: Minimal Working Prototype

### Goal

Validate the minimal personal evolution loop.

```text
Personal Memory
+ Personal Knowledge Base
+ Local Model
+ Remote Teacher by Permission
+ Experience Extraction
+ Skill Formation
+ Future Reuse
```

### Recommended First Scenario

```text
Personal Research Intelligence Companion for One User
```

### Core Features

| Feature | Priority | Description |
|---|---|---|
| Local model runtime | P0 | Run a local LLM or local inference backend |
| Embedding and retrieval | P0 | Enable personal knowledge search |
| Personal memory store | P0 | Store structured personal memory with provenance and permissions |
| Personal knowledge base | P0 | Import documents and retrieve relevant context |
| Remote model adapter | P0 | Use remote teacher models by permission |
| Model router | P0 | Route tasks based on privacy, complexity, and confidence |
| Experience engine | P0 | Extract lessons from completed tasks |
| Evolution log | P0 | Record memory, skill, and strategy changes |
| Skill card store | P1 | Save reusable skills |
| Strategy rule store | P1 | Save preferred methods and decision patterns |
| Personal benchmark samples | P1 | Evaluate whether the system improves |
| Export and restore | P1 | Export core personal assets and restore them locally |

### Exit Criteria

Phase 1 is complete when the prototype can:

1. ingest user documents;
2. answer using local personal context;
3. store and retrieve personal memory;
4. distinguish memory from chat history;
5. ask permission before remote teacher use;
6. produce an experience event after a task;
7. form a basic skill card or strategy rule;
8. reuse that skill or strategy in a later task;
9. record the change in an evolution log;
10. pass a small personal benchmark before and after improvement.

---

## 6. Phase 2: Protocols and Evaluation

### Goal

Turn the prototype into a more rigorous open architecture with reusable protocols and evaluation gates.

### Core Workstreams

| Workstream | Description |
|---|---|
| Memory governance | Source, confidence, conflict handling, deletion, rollback |
| Skill graph | Skills as composable, versioned, evaluable nodes |
| Personal benchmark protocol | Evaluation samples, scoring, gates, regression tests |
| Model router protocol | Rules for local, remote, and hybrid execution |
| Safety guard | Data classification, redaction, permission, tool control |
| Access & Sync | Identity, device authorization, export, import, recovery, encrypted sync direction |
| Fairness and accessibility | Language coverage, low-resource deployment, accessibility testing |

### Exit Criteria

Phase 2 is complete when:

1. memory format has versioned schema;
2. skill graph has a reference format;
3. evolution log can support audit and rollback;
4. personal benchmark protocol can block unsafe or low-quality updates;
5. model routing is explainable and policy-controlled;
6. safety guard handles remote calls and tool permissions;
7. basic access and recovery flows are implemented;
8. fairness and accessibility guidelines are testable.

---

## 7. Phase 3: Personal Model Adaptation

### Goal

Allow each person to form a controlled model adaptation layer.

### Core Workstreams

| Workstream | Description |
|---|---|
| Training candidate pool | Curated candidate examples from user-approved experience |
| Data curator | Cleaning, filtering, sensitivity classification, deduplication |
| Personal adapter manager | LoRA, adapter, preference model, router policy management |
| Distillation pipeline | Remote teacher examples used under permission and governance |
| Evaluation gate | Benchmark and safety tests before adapter deployment |
| Model registry | Versioned personal model assets and rollback points |

### Exit Criteria

Phase 3 is complete when:

1. training candidates are explicitly governed;
2. personal data is not used without authorization;
3. adapters are versioned and linked to evaluation results;
4. rollback works for harmful or low-quality adaptation;
5. base model license constraints are tracked;
6. deployment decisions are explainable;
7. user ownership and portability are preserved.

---

## 8. Phase 4: Open Ecosystem

### Goal

Enable a community ecosystem around skills, plugins, model backends, memory backends, benchmarks, and user interfaces.

### Ecosystem Components

| Component | Examples |
|---|---|
| Skills | writing, research, coding, learning, planning, decision support |
| Memory backends | SQLite, PostgreSQL, Qdrant, Neo4j |
| Model backends | Ollama, llama.cpp, vLLM, SGLang |
| Tool plugins | browser, files, code, MCP tools, local apps |
| Benchmarks | personal evaluation, growth evaluation, safety evaluation, fairness evaluation |
| UI | desktop, web, mobile, browser extension, local server |

### Exit Criteria

Phase 4 is complete when:

1. external developers can build compatible skills;
2. personal assets remain portable across implementations;
3. plugin permissions are enforceable;
4. memory and benchmark formats are stable enough for community use;
5. governance can handle proposals, releases, security issues, and disputes;
6. the ecosystem does not undermine user sovereignty or inclusive access.

---

## 9. Near-Term Priorities

Immediate project priorities:

1. freeze Charter v0.3 and Whitepaper v0.3 as baseline documents;
2. stabilize README and core documentation;
3. complete architecture, principles, roadmap, governance, and AI ethics documents;
4. draft the first three specifications:
   - personal memory format;
   - evolution log format;
   - personal benchmark protocol;
5. prepare contribution, conduct, security, and license files;
6. define Phase 1 reference implementation scope.

---

## 10. What Not to Prioritize Yet

The project should not prematurely prioritize:

- broad commercial packaging;
- full autonomous agents;
- unconstrained self-training;
- public sharing of personal cognitive assets;
- production-grade cloud sync before local governance is stable;
- large plugin ecosystem before permissions and sandboxing are clear;
- model adaptation before evaluation gates are stable.

---

## 11. Summary

Zhiné should move carefully from vision to architecture, from architecture to prototype, from prototype to protocols, and from protocols to ecosystem.

The first goal is not scale. The first goal is proof:

```text
Can a personal AI system remember, reason, learn, evaluate, and grow under user sovereignty?
```

Only after that loop is proven should the project expand into broader adaptation, synchronization, and ecosystem development.
