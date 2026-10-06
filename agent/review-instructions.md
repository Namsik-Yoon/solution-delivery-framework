---
title: Review Instructions
version: 0.1.0
read_when:
  - reviewing a change
skip_when:
  - the task does not concern this document
priority: conditional
---

# Review Instructions

Prioritize incorrect business decisions, leakage, unsafe input handling, secrets, customer-path breakage and missing failure recovery. Check `.framework` independence and dependency pins.

Identify concrete defects with file/line and reproduction; distinguish assumptions from verified findings. Re-run checks only when changes or failures justify it. Never infer production performance from a passing demo.

