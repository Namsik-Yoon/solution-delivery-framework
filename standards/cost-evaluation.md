---
title: Cost Evaluation Standard
version: 0.1.0
read_when:
  - evaluating AI or infrastructure costs
skip_when:
  - the task does not concern this document
priority: conditional
---

# Cost Evaluation Standard

Use dated configuration with model/provider, currency, billing unit and source URL. Never hardcode vendor prices in inference logic.

Generative estimate = (uncached input × input price + cached input × cache price + billable output × output price) / price unit. Add billable retries and provider-specific units without double counting reasoning. Expected retry multiplier is 1/(1-r) only under an explicitly stated independent retry model.

Per-1,000 cost = measured average unit cost × 1,000. Monthly total = variable requests + compute + storage + egress + human review + fixed fees. Report assumed volume, uptime, region, hardware and confidence.

Record price date/source; missing pricing stays unknown. Explain why/when runtime AI calls occur, alternatives (rules, smaller models, batching, caching), caps and fallback. Zero token API cost does not mean zero infrastructure cost.

