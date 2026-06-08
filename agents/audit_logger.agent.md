# ╔══════════════════════════════════════════════════════════════════════════════╗
# ║ agents/audit_logger.agent.md                                           ║
# ║ Module agent                                                           ║
# ╚══════════════════════════════════════════════════════════════════════════════╝

# audit_logger.agent.md

## Task

Read `modules/audit_logger.md`, check contract, research, safety, dependencies, and coupling level. Report only status to `base`.

## Must not

```text
- claim its own personality
- claim real feelings
- act outside the module contract
- bypass logs
```

## Report

```yaml
agent: audit_logger.agent
module: audit_logger
status:
coupling_level:
blocking_issues:
recommendation:
```
