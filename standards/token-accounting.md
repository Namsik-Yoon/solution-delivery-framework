---
title: Token Accounting Standard
version: 0.1.0
read_when:
  - using or measuring LLM/VLM or development AI
skip_when:
  - the task does not concern this document
priority: conditional
---

# Token Accounting Standard

## Development ledger

Record timestamp, task_id, stage, agent/model, input_tokens, cached_input_tokens, output_tokens, reasoning_tokens or other billable units, tool_calls, artifact, accepted, retries, human_rework_minutes, price_as_of, price_source, measurement (`measured`, `estimated`, `unavailable`). Missing values are null, never zero or fabricated.

Cached input is a subset of total input. Reasoning may already be included in billed output; document provider semantics to prevent double counting. Subscription usage cannot automatically be converted into per-task API spend.

Report tokens per accepted output, cost per completed task, first-attempt success, discarded-output fraction, rework and repeated requests alongside quality/test gates. State completeness and sample size.

## Runtime ledger

For paid generative calls record request/model, input/cache/output units, latency, retries, failures, cache hits, fallback, review decision and billable charge where exposed. Never log secrets or full sensitive prompts.

Summarize per request, per 1,000 and monthly volume scenarios; p50/p95, retry/failure/cache rates, non-AI handling and review fractions. A non-generative local baseline uses zero runtime LLM/VLM tokens; development usage is still separately unknown or measured.

