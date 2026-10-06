---
title: Solution Delivery Framework
version: 0.1.0
read_when:
  - starting a project
skip_when:
  - the task does not concern this document
priority: conditional
---

# Solution Delivery Framework

This versioned developer playbook turns a business decision into a reproducible software delivery. Current release: **v0.1.0**.

Start with `agent/agent-entrypoint.md` and `principles/business-first.md`; route all other reads by task. The framework is Markdown guidance, never a runtime library.

Projects pin this repository at `.framework/solution-delivery-framework` using a Git submodule. Customer installation, tests, Docker images, data pipelines and deployment must work without it.

## Lifecycle

Problem → assumptions/data rights → design → baseline → workflow → validation → release → retrospective. See `workflow/project-lifecycle.md` for evidence gates.

## Upgrade policy

Use semantic versioning. Tags are immutable. A project records old/new version and commit, reason, impact, migration, and measured or unavailable quality/token change in its own architecture decisions. No automatic submodule upgrades.

## Contents

- `principles/`: decision principles
- `workflow/`: stages and completion gates
- `standards/`: implementation, data, testing and cost rules
- `templates/`: copy/adapt into project-owned `docs/`
- `agent/`: small task-specific context routes

MIT applies to this framework, not to any project dataset. Improve the next version from completed project retrospectives; preserve older project pins.

