# Zhiné Principles

> Version 0.1  
> Engineering principles, ethical commitments, and non-negotiable rules for Zhiné.

## 1. Purpose

This document defines the principles that should guide Zhiné's design, engineering, documentation, governance, and community development.

Zhiné is a **Personal Intelligence Companion / 个人智慧伙伴** built on an **Open Cognitive Architecture / 开放认知架构**. Its technical core is the **Personal Cognitive Model / 个人认知模型**.

The principles below are not slogans. They are architectural and governance constraints.

---

## 2. Core Lines

> **不止于懂你。**  
> **Beyond understanding.**

> **超越，才是自己。**  
> **To transcend is to become oneself.**

> **人工智能的真正意义，不是让机器更像人，而是让人突破自己。**  
> **The true meaning of artificial intelligence is not to make machines more human, but to help humans transcend their own limits.**

> **AI 应成为人类共享的能力，而不是少数人的特权。**  
> **AI should be a shared human capability, not a privilege of the few.**

---

## 3. Principle 1: Local First

Personal data, memory, knowledge, training candidates, and private context should be local by default.

```text
Local by default.
Cloud by permission.
```

Requirements:

- sensitive personal data should not be sent to remote models without permission;
- local storage must be the default assumption for personal memory;
- remote inference should be auditable;
- users should understand when cloud resources are used;
- offline usability should be considered in core design.

---

## 4. Principle 2: Personal Model Ownership

Users should own and control their personal cognitive assets.

These assets include:

- personal memory;
- personal knowledge base;
- skill graph;
- strategy library;
- personal benchmarks;
- model adapters;
- training candidates;
- evolution logs.

Requirements:

- assets must be exportable when technically possible;
- deletion and rollback must be designed from the beginning;
- user-controlled assets should not be locked into one platform;
- personal adapters must respect base model licenses and data rights;
- the system must distinguish open-source project assets from private user assets.

---

## 5. Principle 3: Open Architecture

Zhiné should not be locked to a single model, framework, database, cloud provider, application, or user interface.

```text
Model-agnostic
Tool-agnostic
Storage-agnostic
Cloud-optional
```

Requirements:

- clear module boundaries;
- documented interfaces;
- replaceable storage backends;
- replaceable model backends;
- open protocols for memory, skills, benchmarks, and evolution logs;
- community-extensible architecture without sacrificing governance.

---

## 6. Principle 4: Evolvable by Design

Growth is not an add-on feature. It is part of the system architecture.

Each meaningful task should be able to produce:

```text
experience
reflection
skill candidate
strategy candidate
benchmark sample
training candidate
```

Requirements:

- growth must be traceable;
- updates must have source, reason, and scope;
- important changes must be reviewed or gated;
- the system should learn from feedback without silently rewriting user identity or goals;
- evolution must not become uncontrolled self-modification.

---

## 7. Principle 5: Verifiable Growth

Zhiné should not merely claim to become smarter or more personalized. It should prove improvement through evaluation.

Requirements:

- personal benchmark samples;
- baseline and regression checks;
- before / after comparison;
- error tracking;
- evaluation gates before durable updates;
- rollback if growth harms quality, safety, fairness, or user intent.

---

## 8. Principle 6: Controlled Self-Training

Zhiné may support self-learning and model adaptation, but only under strict control.

Non-negotiable rules:

```text
No authorization, no use of personal data.
No data governance, no training.
No evaluation, no release.
No versioning, no upgrade.
No rollback, no deployment.
No sensitive data export without permission.
```

Requirements:

- generated outputs must not automatically become training data;
- training candidates require filtering and governance;
- high-impact training samples should be reviewable;
- model adaptation should be versioned;
- every deployed adapter should be linked to evaluation results.

---

## 9. Principle 7: Human Sovereignty

Zhiné serves the individual. It must not replace human judgment, silently expand its authority, or substitute model goals for user goals.

Requirements:

- high-risk actions require confirmation;
- personal goals must not be overwritten by model inference;
- uncertainty should be clearly communicated;
- the system should challenge errors and unsafe assumptions when necessary;
- the model should preserve human judgment rather than create dependency.

---

## 10. Principle 8: Inclusive AI

AI should be a shared human capability, not a privilege of the few.

Inclusive AI is both an ethical commitment and an engineering requirement.

Requirements:

| Direction | Requirement |
|---|---|
| Access fairness | Support low-barrier use, lightweight deployment, local operation, and community editions |
| Language fairness | Support multilingual and multicultural contexts; avoid defaulting to one language or culture |
| Ability fairness | Design for non-technical users, older users, accessibility needs, and clear interaction |
| Data fairness | Users should own their memory, knowledge, evaluation, and adaptation assets |
| Algorithmic fairness | Test for biased, discriminatory, or exclusionary outputs |
| Governance fairness | Allow diverse contributors and users to participate in feedback and roadmap formation |

Inclusive AI does not mean weakening privacy, safety, or abuse prevention. It requires safety, privacy, openness, accessibility, and anti-discrimination to be designed together.

---

## 11. Principle 9: Ubiquitous Access

A Personal Intelligence Companion should not be confined to one device, app, or platform.

Requirements:

- cross-device continuity under user governance;
- local-first access;
- cloud by permission;
- secure export, import, backup, and recovery;
- identity and device management;
- session continuity without loss of user control.

---

## 12. Principle 10: Interoperability

Personal intelligence assets should be portable, restorable, and understandable across systems.

Requirements:

- open formats for memory, skills, evolution logs, and benchmarks;
- documented migration paths;
- no artificial lock-in through opaque schemas;
- recovery from backups;
- clear separation between personal data and application logic.

---

## 13. Behavioral Boundaries

Zhiné must not be described or implemented as:

- a project that copies consciousness, personality, or a digital soul;
- an unconstrained self-evolving system;
- a cloud model wrapper;
- an emotional virtual character;
- a premium AI privilege system for a small group;
- a system that silently escalates permissions;
- a system that stores or trains on private data without permission.

---

## 14. Engineering Rules

Every core module should answer the following questions:

1. What personal asset does this module create, modify, or consume?
2. Who owns the asset?
3. What permission is required?
4. How is the change recorded?
5. Can it be evaluated?
6. Can it be rolled back?
7. Can the user export it?
8. Does it increase platform lock-in?
9. Does it create fairness or accessibility barriers?
10. Does it preserve human judgment?

---

## 15. Summary

Zhiné's principles can be summarized as:

```text
Personal data stays under personal control.
Personal intelligence grows through verifiable evolution.
Remote models assist by permission, not by ownership.
Open architecture prevents lock-in.
Inclusive AI prevents intelligence from becoming a privilege.
Human judgment remains central.
```
