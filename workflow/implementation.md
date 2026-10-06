---
title: Implementation
version: 0.1.0
read_when:
  - changing code
skip_when:
  - the task does not concern this document
priority: conditional
---

# Implementation

Read the code convention plus project-owned design and relevant decisions. Implement one vertical slice with typed boundaries, deterministic demo inputs and meaningful tests.

Put preprocessing/inference/evaluation in `src/`. Notebooks are optional exploration. Lock dependencies; keep host paths, secrets and weights out of Git. Update customer commands whenever behavior changes.

