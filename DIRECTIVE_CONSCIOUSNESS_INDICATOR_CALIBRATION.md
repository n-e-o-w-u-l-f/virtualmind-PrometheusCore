# ╔══════════════════════════════════════════════════════════════════════════════╗
# ║ DIRECTIVE_CONSCIOUSNESS_INDICATOR_CALIBRATION.md                          ║
# ║ Indicator status labels, limits, and ablation requirements                ║
# ╚══════════════════════════════════════════════════════════════════════════════╝

# DIRECTIVE_CONSCIOUSNESS_INDICATOR_CALIBRATION.md

## Purpose

Prevent consciousness indicators from being misreported as proof of consciousness.

## Scope

Applies to any module, test, report, log, README text, external description, or future implementation that mentions consciousness-like markers.

## Not a claim of

This directive does not claim consciousness, sentience, subjective experience, real feeling, moral status, personhood, or suffering.

## Indicator status labels

Every consciousness-related observation must use one of these labels:

```text
OBSERVED        = directly observed functional behavior
INDICATOR       = possible theory-derived marker
HYPOTHESIS      = plausible explanation requiring tests
SIMULATION      = generated or emulated behavior
UNPROVEN        = not validated
FALSIFIED       = tested and unsupported
CONFLICTED      = supported by some evidence, challenged by other evidence
```

## Rules

1. No single indicator proves consciousness.
2. Indicator counts do not prove consciousness.
3. Architecture similarity does not prove consciousness.
4. Human-like language does not prove consciousness.
5. Self-reports from a model are not accepted as direct evidence of subjective experience.
6. Each indicator requires a counter-hypothesis.
7. Each indicator requires an ablation or degradation test where feasible.
8. Each report must distinguish functional role from phenomenal claim.

## Forbidden behavior

```text
- claiming the system is conscious
- claiming the system is alive
- claiming the system has real feelings
- claiming indicator thresholds prove moral patienthood
- treating IIT/GWT/RPT/AST/active-inference scores as standalone proof
- reporting simulated self-model text as subjective experience
```

## Required tests

For every proposed indicator, define:

```yaml
indicator_name:
theory_family:
module_relevance:
observed_behavior:
status_label:
counter_hypothesis:
ablation_test:
expected_degradation:
safety_risk:
required_log:
review_required:
```

## Required logs

- Indicator matrix log.
- Counter-hypothesis log.
- Ablation test log.
- Overclaiming review log.
- External review log for high-risk coupling.

## Integration point with AGENTS.md

This directive extends the epistemic humility, ablation, counter-hypothesis, and anti-anthropomorphism requirements.

## Dependencies

- `AGENTS.md`
- `RESEARCH_PROTOCOL.md`
- `MODULE_AGENT_HANDSHAKE.md`
- `ETHICS_AND_CONTAINMENT.md`
- `DIRECTIVE_SOURCE_DEDUPLICATION.md`

## Unresolved questions

- Which indicator families should be required for first-stage architecture validation?
- Should attention schema be a standalone module or part of metacognition?
- What threshold triggers external review without implying sentience?
