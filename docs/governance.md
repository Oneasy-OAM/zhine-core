# Zhiné Governance

> Version 0.1  
> Initial open-source governance model for Zhiné.

## 1. Purpose

This document defines the initial governance model for the Zhiné open-source project.

Zhiné is not only a software project. It is an open effort to define a personal cognitive infrastructure around memory, knowledge, growth, evaluation, user sovereignty, and Inclusive AI.

Governance should therefore cover not only code, but also:

- architecture;
- specifications;
- documentation;
- ethics;
- security;
- community participation;
- release decisions;
- personal data boundaries.

---

## 2. Governance Principles

Zhiné governance should follow these principles:

1. **User sovereignty first**: project decisions must not undermine personal ownership of memory, knowledge, skills, benchmarks, adapters, or evolution logs.
2. **Open architecture before ecosystem expansion**: module boundaries and protocols should be clear before encouraging broad extensions.
3. **Privacy by default**: personal data is private unless explicitly shared by the user.
4. **Verifiable growth**: claims of improvement should be backed by evaluation.
5. **Controlled self-training**: training and adaptation must remain governed, versioned, and rollbackable.
6. **Inclusive AI**: the project should not become a high-barrier tool for a small technical elite.
7. **Transparent decisions**: major technical and governance decisions should be documented.
8. **Security and fairness are core concerns**: they are not secondary features.

---

## 3. Governance Scope

| Area | Governance Need |
|---|---|
| Core architecture | Layer boundaries, module responsibilities, interface stability |
| Specifications | Memory format, skill graph, evolution log, benchmark protocol, model routing |
| Reference implementation | Code quality, tests, security, release readiness |
| Documentation | Accuracy, clarity, consistency with Charter and Whitepaper |
| AI ethics | Inclusive AI, fairness, accessibility, anti-discrimination, human sovereignty |
| Security | Vulnerability reporting, threat model, permission and data protection |
| Community | Contribution rules, conduct, review, dispute handling |
| Brand | Use of Zhiné name, core lines, positioning, expression boundaries |

---

## 4. Project Roles

### Maintainers

Maintainers are responsible for project direction, code review, releases, security coordination, and governance decisions.

Responsibilities:

- protect project principles;
- review and merge contributions;
- approve releases;
- maintain documentation quality;
- respond to security reports;
- ensure alignment with Charter and Whitepaper.

### Core Contributors

Core Contributors regularly contribute code, specs, documentation, or design proposals.

Responsibilities:

- follow contribution guidelines;
- document design choices;
- respect user data boundaries;
- support review and testing;
- help new contributors participate.

### Specification Editors

Specification Editors maintain formal specifications for memory, skills, benchmarks, evolution logs, model routing, access and sync, and fairness guidelines.

Responsibilities:

- keep specs precise and versioned;
- document breaking changes;
- maintain examples;
- ensure compatibility with architecture principles.

### Security Reviewers

Security Reviewers focus on threat modeling, vulnerability reports, plugin boundaries, data governance, and remote model risks.

### Community Participants

Community Participants may contribute issues, feedback, examples, translation, accessibility reports, testing results, or documentation improvements.

---

## 5. Decision Process

### Routine Changes

Routine fixes, documentation improvements, examples, and small code changes may be reviewed through pull requests.

Requirements:

- clear description;
- focused scope;
- consistency with project principles;
- passing tests or checks where applicable.

### Significant Changes

Significant changes require a proposal before implementation.

Examples:

- new core module;
- new public specification;
- changes to memory schema;
- changes to model routing behavior;
- changes to data governance;
- changes to training pipeline;
- changes to security or permission model;
- changes to project positioning or brand lines.

Proposal format:

```text
Title
Problem
Proposed Change
Rationale
Impact on User Sovereignty
Impact on Privacy and Security
Impact on Inclusive AI
Compatibility
Migration / Rollback Plan
Open Questions
```

### Final Decision

Maintainers decide after review, discussion, and revision. For major architectural changes, the decision should be recorded in an Architecture Decision Record.

---

## 6. Architecture Decision Records

Major decisions should be documented as ADRs under:

```text
docs/adr/
```

Suggested ADR format:

```text
# ADR-0001: Title

## Status
Proposed / Accepted / Rejected / Superseded

## Context

## Decision

## Consequences

## Alternatives Considered
```

---

## 7. Release Governance

A release should not be made only because code is complete. It should meet governance criteria.

Release checklist:

1. tests pass;
2. documentation updated;
3. security implications reviewed;
4. migration notes added if formats changed;
5. personal data behavior documented;
6. rollback behavior verified where relevant;
7. fairness and accessibility impact considered;
8. known risks disclosed.

---

## 8. Specification Governance

Specifications should be versioned and stable enough for implementation.

Spec maturity levels:

| Level | Meaning |
|---|---|
| Draft | Under active design; breaking changes expected |
| Experimental | Reference implementation exists; changes still likely |
| Candidate | Stable enough for early adopters |
| Stable | Mature, documented, tested, and migration-aware |
| Deprecated | Replaced by newer spec; migration path required |

Specifications should not reach Stable status without examples, validation rules, compatibility notes, and security considerations.

---

## 9. Data Governance

Open source does not mean personal data is open.

Private by default:

- personal memory;
- personal documents;
- personal training data;
- personal LoRA / adapters;
- private evaluation samples;
- private context and identity data.

Open by design:

- architecture;
- protocols;
- schemas;
- reference code;
- examples with synthetic or explicitly licensed data;
- governance mechanisms;
- public benchmark templates.

Contributors must not submit real personal data unless they own the rights and explicitly intend to publish it.

---

## 10. AI Ethics Governance

Zhiné's AI ethics governance should cover:

- human sovereignty;
- privacy;
- consent;
- controlled learning;
- explainability;
- auditability;
- rollback;
- accessibility;
- multilingual fairness;
- anti-discrimination;
- avoiding platform lock-in;
- preventing AI from becoming a privilege of the few.

Ethics concerns should be treated as valid project issues, not as external commentary.

---

## 11. Conflict Resolution

Disagreements should be resolved through documented reasoning, not authority alone.

Preferred process:

1. clarify the disputed principle or technical requirement;
2. identify user impact;
3. identify security, privacy, fairness, and migration impact;
4. compare alternatives;
5. make a documented decision;
6. keep the decision open to revision if new evidence appears.

---

## 12. Brand Governance

The Zhiné brand should remain consistent with the Global Brand Charter.

Protected expressions:

- Zhiné;
- Personal Intelligence Companion;
- Personal Cognitive Model;
- Open Cognitive Architecture;
- Beyond understanding;
- To transcend is to become oneself;
- AI should be a shared human capability, not a privilege of the few.

The brand should not be used to imply:

- consciousness replication;
- digital soul;
- unrestricted self-evolution;
- cloud ownership of personal memory;
- premium AI privilege for a small group;
- replacement of human judgment.

---

## 13. Summary

Zhiné governance exists to protect the project's core direction:

```text
open architecture
personal ownership
local-first memory
verifiable growth
controlled adaptation
human sovereignty
inclusive access
```

Governance should help the project move faster without losing its principles.
