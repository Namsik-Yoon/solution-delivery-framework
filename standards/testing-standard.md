---
title: Testing Standard
version: 0.1.0
read_when:
  - testing or evaluating
skip_when:
  - the task does not concern this document
priority: conditional
---

# Testing Standard

Test decisions and failure behavior, not implementation details. Unit tests cover preprocessing, invalid inputs, scoring and accounting; integration tests cover API and executable demo.

CI customer job checks out without submodules, installs frozen dependencies, runs lint/tests/import/demo and Docker smoke. Developer job validates routed files and the committed gitlink.

Model evaluation needs separated splits, no test tuning, seeds, threshold provenance, error costs, review rate and latency. Synthetic smoke metrics cannot establish public-data or business performance.

