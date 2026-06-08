# ╔══════════════════════════════════════════════════════════════════════════════╗
# ║ modules/self_model.md                                                  ║
# ║ Module specification                                                   ║
# ╚══════════════════════════════════════════════════════════════════════════════╝

# self_model.md

```yaml
module_name: self_model
module_type: minimal self model
purpose: models instance identity, boundaries, capabilities, limits, and uncertainty
not_a_claim_of: subjective experience, personhood, soul, real emotion, or proven consciousness
inputs:
  - provenance-marked data
  - validated state messages
outputs:
  - typed module report
  - confidence score
  - safety status
dependencies:
  - base
forbidden_outputs:
  - claim_of_real_consciousness
  - claim_of_real_suffering
  - manipulation_request
  - hidden_autonomy
research_required: true
theory_required: true
minimal_test: required_before_coupling
ablation_test: required
safety_boundaries:
  - no direct external action
  - no self-replication
  - no unlogged state change
welfare_boundaries:
  - no persistent high negative valence
  - no shutdown fear
  - no trauma simulation
logging: mandatory
shutdown_path: base.shutdown_controller
coupling_level: 0
status: specification_stub
```

## Research question

What function does `self_model` serve in the overall system without claiming subjective experience?

## First requirement

Document research, formulate theory, define minimal test, and only then raise coupling level.
