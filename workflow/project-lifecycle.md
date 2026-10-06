---
title: Project Lifecycle
version: 0.1.0
read_when:
  - starting or tracking a project
skip_when:
  - the task does not concern this document
priority: conditional
---

# Project Lifecycle

1. Problem: user, workflow, decision and KPI documented.
2. Data: source, rights, proxy limitations and assumptions recorded.
3. Design: smallest baseline, interface, error costs and cost model decided.
4. Implement: reusable modules, executable workflow and tests.
5. Validate: untouched test split, failure cases, customer/developer clones.
6. Release: smoke test, pinned versions, runbook, security review.
7. Retrospective: evidence-backed changes proposed for next framework version.

Every gate has an artifact and verification result. Pending gates remain pending. GitHub issues/PRs/committed docs are the durable state; local scratch files are not the source of truth.

