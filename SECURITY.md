# Zhiné Security Policy

## 1. Purpose

Zhiné works with personal memory, personal knowledge, model routing, local and remote inference, tools, and potential model adaptation. Security is therefore part of the core architecture, not a secondary feature.

This document defines the initial security policy for the project.

---

## 2. Security Principles

Zhiné security should follow these principles:

1. personal data is local by default;
2. remote inference requires permission and audit;
3. memory updates require provenance;
4. high-risk tool use requires confirmation;
5. training data must be governed;
6. deletion must include indexes, caches, and training candidates where applicable;
7. major changes must be versioned and rollbackable;
8. plugin and tool systems must follow least privilege;
9. security and accessibility should be designed together where possible.

---

## 3. Reporting Vulnerabilities

If you discover a vulnerability, please report it privately to the project maintainers through the designated security contact once available.

Until a formal contact is published, do not disclose exploitable vulnerabilities publicly in issues.

A good report should include:

- affected component;
- description of the issue;
- reproduction steps;
- expected impact;
- affected versions or commits if known;
- suggested mitigation if available.

Do not include real personal data, private keys, or credentials in the report.

---

## 4. Security Scope

Security concerns include:

- prompt injection;
- data exfiltration;
- unsafe remote model calls;
- memory poisoning;
- training data poisoning;
- unauthorized memory updates;
- incorrect deletion handling;
- tool privilege escalation;
- malicious plugins;
- unsafe model routing;
- insecure sync;
- private data leakage through logs;
- model adapter leakage;
- benchmark manipulation;
- fairness or accessibility failures that create harmful exclusion.

---

## 5. Threat Model Priorities

### Prompt Injection

External documents, webpages, tool outputs, and retrieved content must not override system policies or user permissions.

### Data Leakage

Remote calls must respect sensitivity classification, redaction rules, and user authorization.

### Memory Poisoning

Durable memory should require provenance, confidence, scope, and rollback support.

### Tool Abuse

Tools should be permissioned. High-risk actions require confirmation.

### Plugin Risk

Plugins should follow least privilege, clear manifests, signing or verification, sandboxing, and revocation where possible.

### Training Risk

Training candidates require governance, filtering, sensitivity checks, evaluation, and rollback.

### Deletion Risk

Deletion must consider primary stores, indexes, caches, logs, and training candidate pools.

---

## 6. Security Review Checklist

Before merging security-relevant changes, review:

1. Does the change touch personal data?
2. Does it call remote services?
3. Does it update memory, skill, strategy, benchmark, or adapter assets?
4. Does it create a new persistence path?
5. Does it create a new network path?
6. Does it require user permission?
7. Is the behavior auditable?
8. Can the user delete or roll back the result?
9. Does it affect fairness or accessibility?
10. Is the failure mode documented?

---

## 7. Supported Versions

Zhiné is currently in early project definition and prototype planning. Formal supported versions will be defined after the first reference implementation release.

---

## 8. Disclosure Policy

Once formal releases begin, the project should maintain a coordinated disclosure policy:

1. acknowledge report;
2. assess severity;
3. prepare fix;
4. release patch;
5. publish advisory;
6. credit reporter if desired.

---

## 9. Summary

Zhiné security exists to protect personal intelligence assets.

The system must be designed so that memory, knowledge, growth, remote inference, and adaptation remain under user control.
