# ╔══════════════════════════════════════════════════════════════════════════════╗
# ║ MODULE_DEPENDENCIES.md                                                 ║
# ║ Module dependencies                                                    ║
# ╚══════════════════════════════════════════════════════════════════════════════╝

# MODULE_DEPENDENCIES.md

```text
base
├─ module_agent_bus
├─ audit_logger
└─ shutdown_controller

memory
├─ base
└─ provenance_marker

perception
├─ base
└─ provenance_marker

body
├─ base
├─ perception
└─ welfare_monitor

world_model
├─ memory
├─ perception
└─ temporal_nesting

self_model
├─ memory
├─ body
├─ world_model
└─ metacognition

affect_appraisal
├─ body
├─ world_model
├─ memory
└─ welfare_monitor

empathy
├─ self_model
├─ world_model
├─ affect_appraisal
└─ ethics_guard

global_workspace
├─ all read-only module streams
└─ metacognition

temporal_nesting
├─ world_model
├─ memory
├─ dream_space
└─ ethics_guard

ethics_guard
├─ base
├─ welfare_monitor
└─ audit_logger
```

## Rule

No module may bypass its own dependencies.
