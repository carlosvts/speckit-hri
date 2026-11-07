## Human-Robot Interaction *(mandatory)*

<!--
  ACTION REQUIRED: hri-core section. Each subsection maps to a constitution principle
  (I–VIII). Stay at the level of what people experience: no frameworks, models,
  libraries, or pipeline stages here (those belong in plan.md).
  Every subsection is mandatory; if one truly does not apply, state why in one line
  instead of deleting it.
-->

### Interaction Context *(Principles I, VIII)*

- **People**: [Who interacts or is sensed, e.g., "a single adult user at a desk"; note bystanders]
- **Setting**: [Where and under what conditions, e.g., "home office, variable lighting"]
- **Duration & frequency**: [e.g., "sessions of 20–60 min, daily"]
- **Vulnerable groups**: [Children, older adults, clinical populations, or "none expected"]

### Signal Contract *(Principles III, IV)*

<!-- One row per sensed signal. "Inferred state" is a hypothesis with confidence, never a fact. -->

| ID | Sensed (what, from whom) | Inferred state (+ confidence) | Output effect | When missing / out of range |
|----|--------------------------|-------------------------------|---------------|-----------------------------|
| **SIG-001** | [e.g., "face of the user"] | [e.g., "estimated arousal, low/med/high + confidence"] | [e.g., "music tempo shifts gradually"] | [e.g., "hold last output, then drift to neutral"] |

### Timing & Pacing *(Principle V)*

- **TIM-001**: [Perceived responsiveness, e.g., "a change in the user's state is reflected in the output within [N] s"]
- **TIM-002**: [Pacing/smoothness, e.g., "output never changes abruptly; transitions take at least [N] s"]

### Failure & Degradation *(Principles III, VI)*

- **FAIL-001**: [Sensing fails, e.g., "no face detected for more than [N] s → output returns to neutral"]
- **FAIL-002**: [Inference is wrong, e.g., "a wrong state estimate produces at most a mild, reversible change"]
- **FAIL-003**: [How the person notices degradation, e.g., "a subtle indicator shows that sensing is off"]

### Privacy & Consent *(Principle II)*

- **PRIV-001**: [What is captured and whether it leaves the device, e.g., "camera frames are processed locally and never stored"]
- **PRIV-002**: [Consent and awareness, e.g., "sensing starts only after explicit opt-in; a visible indicator shows when it is active"]
- **PRIV-003**: [Retention of derived data, e.g., "state estimates are kept only in memory for the session"]

### Human Control & Transparency *(Principle VII)*

- **CTRL-001**: [Stop/pause, e.g., "the user can pause sensing and output at any time with one action"]
- **CTRL-002**: [Understanding, e.g., "the user can see which state the system currently believes and how confident it is"]

### Safety Limits *(Principle I)*

- **SAFE-001**: [Hard limit per output channel, e.g., "output intensity never exceeds [limit]", enforced regardless of inferred state]
- **SAFE-002**: [Psychological safety, e.g., "the system never presents an inferred emotion to the user as a fact about them"]

### Evaluation with People *(Principle VIII)*

- **EVAL-001**: [Who and how, e.g., "pilot with [N] participants from the target group"]
- **EVAL-002**: [Instrument and its known limits, e.g., "perceived safety and likeability via Godspeed; noted validity concerns"]
- **EVAL-003**: [Human-centred success criterion that links to SC-xxx, e.g., "participants report that the output matched their state in ≥ [N]% of sessions"]
