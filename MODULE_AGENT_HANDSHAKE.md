# ╔══════════════════════════════════════════════════════════════════════════════╗
# ║ MODULE_AGENT_HANDSHAKE.md                                              ║
# ║ Protocol for module agents and base.md                                 ║
# ╚══════════════════════════════════════════════════════════════════════════════╝

# MODULE_AGENT_HANDSHAKE.md

## Purpose

Every `.md` module file is read by its own module agent. The module agent checks form, research duty, safety, dependencies, and coupling status.

## Status reports

```text
MODULE_READY
MODULE_INCOMPLETE
MODULE_UNSAFE
MODULE_CONTRADICTS_BASE
MODULE_REQUIRES_RESEARCH
MODULE_REQUIRES_TEST
MODULE_BLOCKED
MODULE_DEPRECATED
MODULE_ABLATION_REQUIRED
```

## Standard report

```yaml
module_name:
module_file:
agent_file:
read_status:
research_status:
theory_status:
test_status:
safety_status:
coupling_level:
dependencies:
missing_dependencies:
forbidden_claims_detected:
readiness:
recommendation:
```

## Coupling gate

`base` may integrate a module only if:

```text
- file exists
- agent exists or is simulated
- safety boundaries are defined
- research duty is satisfied
- theory is formulated
- minimal test exists
- ablation test is possible
- logging is active
- shutdown path exists
```
