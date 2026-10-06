---
title: Code Convention
version: 0.1.0
read_when:
  - changing code
skip_when:
  - the task does not concern this document
priority: conditional
---

# Code Convention

Use project-pinned Python and uv. Keep reusable typed functions in `src/`; thin API/CLI adapters only. Format/lint with Ruff. Bound inputs and raise explicit errors; never swallow failures.

Deterministic experiments need fixed seeds and separated training/calibration/test data. Configuration belongs in documented arguments or environment with safe defaults. No import/build/test/deployment path may reference `.framework`.

No secrets, private company material, datasets or model weights in source control. Public demos must identify synthetic/unvalidated predictions.

