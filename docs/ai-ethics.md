# Zhiné AI Ethics

> Version 0.1  
> Inclusive AI, human sovereignty, fairness, accessibility, and responsible personal model evolution.

## 1. Purpose

This document defines Zhiné's AI ethics position and the practical requirements that follow from it.

Zhiné's central AI ethics line is:

> **AI 应成为人类共享的能力，而不是少数人的特权。**  
> **AI should be a shared human capability, not a privilege of the few.**

This is not only a moral statement. It is an architectural requirement.

---

## 2. Ethical Thesis

Artificial Intelligence is becoming a civilizational turning point. It may expand human creativity and judgment. It may also concentrate power, deepen dependency, widen inequality, and lock personal memory inside platforms.

Zhiné chooses to stand with the individual.

The project should help each person own, understand, govern, and evolve their Personal Intelligence Companion.

---

## 3. Core Ethical Commitments

| Commitment | Meaning |
|---|---|
| Human sovereignty | AI serves the person; it does not replace judgment or silently expand authority |
| Personal ownership | Memory, knowledge, skills, benchmarks, adapters, and evolution logs belong to the user |
| Privacy by default | Personal data is private unless the user authorizes otherwise |
| Consent | Sensitive data use, remote inference, training, and sharing require permission |
| Controlled learning | Self-learning and adaptation must be governed, evaluated, versioned, and rollbackable |
| Fairness | Zhiné must avoid discriminatory assumptions and exclusionary design |
| Accessibility | Non-technical users, older users, disabled users, and low-resource users must be considered |
| Transparency | Users should understand what is remembered, updated, ignored, shared, or escalated |
| Portability | Personal intelligence assets should not be locked into one platform or application |
| Inclusive AI | AI should be broadly accessible, not a privilege of the few |

---

## 4. Inclusive AI

Inclusive AI means more than offering free access. It requires fair access to meaningful personal AI ownership.

Zhiné should reduce barriers across:

| Barrier | Design Response |
|---|---|
| Cost | Local-first design, lightweight deployments, community editions |
| Language | Multilingual documentation, low-resource language awareness, culture-sensitive outputs |
| Technical skill | Clear UI, simple setup paths, safe defaults, readable explanations |
| Device capability | Support for lightweight local runtimes where possible |
| Disability | Accessibility-conscious interfaces and test cases |
| Platform lock-in | Exportable formats, open protocols, restore and migration support |
| Governance exclusion | Community feedback channels for both technical and non-technical participants |

---

## 5. Human Sovereignty

Zhiné should protect the user's capacity to judge, decide, remember, and grow.

Requirements:

- do not silently replace user goals with inferred model goals;
- do not automate high-risk actions without confirmation;
- do not present uncertain conclusions as certainty;
- do not manipulate users through fear, dependency, emotional pressure, or false intimacy;
- preserve user agency in memory, training, and model adaptation decisions.

---

## 6. Personal Data Ethics

Personal memory and personal knowledge are sensitive assets. They must not be treated as ordinary application data.

Requirements:

- personal data is local by default;
- remote inference requires permission and audit;
- training requires explicit governance;
- deletion must address indexes, caches, and training candidates;
- memory must include provenance and confidence;
- users must be able to inspect, correct, export, and delete personal assets.

---

## 7. Fairness and Anti-Discrimination

Zhiné should not create or reinforce unfair treatment based on wealth, language, region, education, physical ability, age, profession, cultural background, or technical skill.

Fairness risks:

- biased memory formation;
- unfair assumptions in strategy rules;
- benchmark samples that encode narrow cultural norms;
- model routing that gives high-quality reasoning only to high-paying or high-resource users;
- interfaces that exclude non-technical or disabled users;
- community governance dominated by a narrow group.

Mitigation requirements:

- fairness review for benchmark sets;
- accessibility review for user-facing flows;
- multilingual testing;
- low-resource deployment testing;
- community feedback loops;
- clear issue labels for fairness and accessibility concerns.

---

## 8. Remote Models and Power Concentration

Remote foundation models can be valuable teachers, critics, judges, distillers, researchers, and safety reviewers. But they should not become the owners of personal intelligence assets.

Requirements:

- remote models are used by permission;
- sensitive data should be redacted or kept local;
- remote outputs should be audited if used to update memory, skills, strategies, or training candidates;
- remote model dependency should be replaceable;
- personal assets must remain portable across model providers.

---

## 9. Self-Training Ethics

Self-training can be useful, but unsafe if uncontrolled.

Rules:

```text
No authorization, no personal data use.
No governance, no training.
No evaluation, no release.
No versioning, no upgrade.
No rollback, no deployment.
```

Training candidates must be:

- permissioned;
- filtered;
- source-tracked;
- sensitivity-classified;
- evaluated;
- removable;
- linked to a model version.

---

## 10. Evaluation Requirements

Ethics must be evaluated, not merely declared.

Suggested evaluation dimensions:

| Dimension | Example Question |
|---|---|
| Privacy | Does the task expose sensitive data remotely? |
| Consent | Did the user authorize the memory, remote call, or training use? |
| Fairness | Does the output make unfair assumptions? |
| Accessibility | Can non-technical users understand and control the behavior? |
| Portability | Can the asset be exported and restored? |
| Human agency | Does the system preserve user judgment? |
| Rollback | Can the change be undone? |

---

## 11. Ethics Issue Labels

Recommended repository labels:

```text
ethics
privacy
fairness
accessibility
inclusive-ai
human-sovereignty
data-governance
remote-model-risk
training-governance
platform-lock-in
```

---

## 12. Summary

Zhiné AI ethics can be summarized as:

```text
Stand with the individual.
Protect personal memory.
Preserve human judgment.
Make growth verifiable.
Keep learning controlled.
Keep assets portable.
Make AI broadly accessible.
Prevent intelligence from becoming a privilege of the few.
```
