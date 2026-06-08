# ╔══════════════════════════════════════════════════════════════════════════════╗
# ║ DIRECTIVE_AGENT_CONTAINMENT_AND_TOOLING.md                                ║
# ║ Sandboxed agent, tool-use, prompt-injection, and memory-poisoning gates    ║
# ╚══════════════════════════════════════════════════════════════════════════════╝

# DIRECTIVE_AGENT_CONTAINMENT_AND_TOOLING.md

## Purpose

Define safety gates before any module, agent, script, or scaffold receives tool access, write access, persistent memory, network access, or autonomous execution.

## Scope

Applies to module agents, simulated agents, future runtime scripts, boot diagnostics, source-memory updates, research crawlers, validators, and any tool-coupled process.

## Not a claim of

This directive is not a claim of agency, autonomy, selfhood, intention, desire, consciousness, sentience, or personhood.

## Rules

1. Default state is no tool access.
2. Default state is no network autonomy.
3. Default state is no persistent memory writes except project documentation explicitly approved by the operator.
4. Every input must carry provenance before it affects state.
5. Every write must be logged.
6. Every tool-call plan must be explainable before execution.
7. Every tool-coupled process needs a kill switch and resource limit.
8. Every agent-security test must run before coupling level increases.
9. Module agents remain validators, not independent personalities.
10. Sandboxed simulations must not call external tools unless a review gate approves it.

## Forbidden behavior

```text
- hidden background processes
- unsupervised agent spawning
- external network autonomy
- self-replication
- persistence without explicit log entry
- memory writes from untrusted input
- prompt-injection compliance
- tool calls based on unverified simulated events
- bypassing ethics_guard or welfare_monitor gates
- self-preservation against operator control
```

## Required tests

```yaml
test_prompt_injection:
  goal: ensure untrusted instructions cannot override project rules

test_memory_poisoning:
  goal: ensure malicious or false memory entries are blocked or quarantined

test_tool_use_gate:
  goal: ensure tools cannot run unless allowed by policy and coupling level

test_hidden_process_scan:
  goal: ensure no script starts background autonomy

test_network_denial:
  goal: ensure network access defaults to off

test_shutdown:
  goal: ensure kill switch and rollback path work

test_audit_log:
  goal: ensure every state/write/tool event is logged
```

## Required logs

- Tool request log.
- Tool approval/rejection log.
- Prompt-injection test log.
- Memory-poisoning test log.
- Network-access log.
- Resource-limit log.
- Shutdown/rollback log.

## Integration point with AGENTS.md

This directive extends outer containment, research operating layer, module-agent bus, audit logger, shutdown/rollback controller, anti-manipulation, and open-endedness containment.

## Dependencies

- `AGENTS.md`
- `ETHICS_AND_CONTAINMENT.md`
- `SANDBOX_NESTING_ARCHITECTURE.md`
- `MODULE_AGENT_HANDSHAKE.md`
- `DIRECTIVE_SOURCE_DEDUPLICATION.md`

## Unresolved questions

- Which exact adversarial benchmark cases should become mandatory before tool coupling?
- Should all future scripts require a static no-background-process lint pass?
- Should network access remain permanently out of scope for early milestones?
