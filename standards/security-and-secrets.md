---
title: Security and Secrets
version: 0.1.0
read_when:
  - handling inputs secrets or deployment
skip_when:
  - the task does not concern this document
priority: conditional
---

# Security and Secrets

Use `.env` locally and Codespaces/Actions secrets remotely. Commit only `.env.example` with placeholders. Never use company code/data/logs/credentials in public portfolios.

Bound upload bytes/pixels, validate schemas and reject malformed inputs. Avoid unsafe archive extraction and executable model deserialization. Keep raw uploads out of logs. Limit CI permissions and pin third-party actions.

Demo services bind locally by default. Public exposure needs authentication, TLS, rate limits, monitoring and explicit retention decisions. Review staged files for secrets and artifacts before publishing.

