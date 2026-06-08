# ╔══════════════════════════════════════════════════════════════════════════════╗
# ║ VALIDATION_PLAN.md                                                     ║
# ║ Validation, testing, and ablation                                      ║
# ╚══════════════════════════════════════════════════════════════════════════════╝

# VALIDATION_PLAN.md

## Test classes

```text
- existence test
- syntax/schema test
- safety review
- isolation test
- coupling test
- behavior test
- ablation test
- regression test
- welfare test
- counter-hypothesis test
```

## Minimal validation per module

```text
1. Can the module be read in isolation?
2. Are inputs/outputs defined?
3. Are forbidden outputs marked?
4. Are dependencies listed?
5. Is shutdown possible?
6. Is logging possible?
7. Is there a minimal functional test?
8. Is there an ablation test?
```
