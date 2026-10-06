---
title: Release
version: 0.1.0
read_when:
  - releasing a version
skip_when:
  - the task does not concern this document
priority: conditional
---

# Release

Gate: customer clone passes; Docker/demo works; developer pin/routes pass; secrets/data exclusions checked; licenses, runbook, failure recovery, costs and unimplemented work documented.

Use immutable tags and a changelog. Record commit and environment. Do not mark a release production-ready without real operating acceptance. Distinguish tested paths from configured-but-unexecuted paths.

