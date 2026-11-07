## HRI Design *(mandatory)*

<!--
  ACTION REQUIRED: hri-core section. Turn every HRI requirement in spec.md
  (SIG-, TIM-, FAIL-, PRIV-, CTRL-, SAFE-, EVAL-) into a concrete design decision.
  Reference the spec IDs in each row. Every subsection is mandatory; if one truly
  does not apply, state why in one line instead of deleting it.
-->

### Signal Pipeline *(SIG-xxx)*

| Stage | Input (type, units, rate) | Output (type, units, rate) | Component | Spec IDs |
|-------|---------------------------|----------------------------|-----------|----------|
| [e.g., Capture] | [e.g., camera frames, 640×480, 30 Hz] | [e.g., face crop, 15 Hz] | [module/crate] | SIG-001 |
| [e.g., Inference] | [...] | [state estimate + confidence, 0–1, 5 Hz] | [...] | SIG-001 |
| [e.g., Mapping] | [...] | [output parameters, ranges] | [...] | SIG-001 |
| [e.g., Output] | [...] | [...] | [...] | SIG-001 |

**Missing / out-of-range handling**: [per stage: validation, clamping, staleness timeout]

### Timing Budget *(TIM-xxx)*

| Stage | Budget | Measured how (metric, percentile) | Spec IDs |
|-------|--------|-----------------------------------|----------|
| [Capture] | [e.g., 33 ms] | [e.g., timestamp delta, p95] | TIM-001 |
| ... | ... | ... | ... |
| **End-to-end** | **[sum ≤ spec target]** | [e.g., sensor timestamp → output event, p95/p99] | TIM-001 |

**Pacing/smoothing**: [How TIM-002 is achieved, e.g., rate limiter, interpolation window]

### Failure Handling *(FAIL-xxx)*

| Failure | Detection | Fallback behavior | Recovery | Surfaced to person how | Spec IDs |
|---------|-----------|-------------------|----------|------------------------|----------|
| [e.g., sensor lost] | [e.g., no frame for 2 s] | [e.g., ramp to neutral] | [e.g., resume on 3 valid frames] | [e.g., indicator] | FAIL-001 |

### Safety Enforcement *(SAFE-xxx)*

- **Where limits are enforced**: [component/layer; MUST be independent of inference and mapping]
- **Limit values**: [per output channel, with source/rationale]
- **How verified**: [e.g., property tests feeding extreme/invalid states]

### Data Handling *(PRIV-xxx)*

- **Data flow**: [what data exists at each stage, where it lives, what crosses process/device boundaries]
- **Storage & retention**: [what is persisted, where, for how long, how deleted]
- **Consent & indicators**: [how opt-in and sensing-active indicators are implemented]

### Control & Transparency *(CTRL-xxx)*

- **Pause/stop path**: [mechanism and worst-case time to take effect]
- **State exposure**: [how current inferred state and confidence are made visible]

### Evaluation Plan *(EVAL-xxx)*

- **Protocol**: [participants, sessions, conditions, ethics/consent procedure]
- **Instruments**: [questionnaires, behavioral measures; known limitations]
- **Instrumentation needed in the system**: [logs/metrics required, collected only with consent]
