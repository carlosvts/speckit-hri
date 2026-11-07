# [PROJECT_NAME] Constitution
<!-- Generated from the hri-core preset (speckit-hri). Sections marked "hri-core" are
     fixed baseline principles: projects may make them stricter, never weaker,
     without an amendment recorded under Governance.
     Sources: https://github.com/carlosvts/speckit-hri/blob/main/presets/hri-core/REFERENCES.md -->

## HRI Principles (hri-core)

### I. Human Wellbeing & Safety First
No system output may cause physical or psychological harm to the people it interacts
with. Every output channel MUST declare hard limits (e.g., intensity, rate, duration)
enforced in code, independent of any model or inferred state. Safety limits win over
every other requirement, including responsiveness and engagement.

### II. Privacy & Consent by Design
Sensing of people MUST be minimal, purposeful, and consented. Raw sensor data
(images, audio, physiological signals) is processed locally and discarded by default;
any storage or transmission requires an explicit, documented purpose, retention
period, and opt-in. People MUST be able to tell when they are being sensed.

### III. Inferred Human State Is Uncertain
Any estimate of a person's state (emotion, attention, engagement, intent) is a
hypothesis, not a fact. Estimates MUST carry a confidence or validity signal, and the
system MUST behave acceptably when the estimate is wrong. Features MUST NOT rely on
the assumption that internal states can be read reliably from surface signals.

### IV. Explicit Signal Contracts
Every mapping from input signal to inferred state to system output MUST be specified:
units, ranges, sampling or update rates, semantics, and behavior on missing or
out-of-range data. Unspecified signals are not allowed into the pipeline.

### V. Timing Is a Requirement
Latency, update rate, and pacing are functional requirements, not optimizations.
Each interaction loop MUST have an explicit end-to-end timing budget, broken down
per stage, and verified by measurement.

### VI. Graceful, Legible Failure
Every component MUST define its failure modes and fall back to a safe, neutral
behavior. When the system degrades, the person MUST be able to perceive that
something changed. Silent failure is a defect.

### VII. Transparency & Human Control
People MUST be able to understand, at an appropriate level, what the system senses
and why it responds as it does, and MUST be able to pause or stop it at any time.
Design aims for calibrated trust, not maximal trust.

### VIII. Evaluate With People
Success is measured with the people the system serves, not only with technical
metrics. Each feature MUST define how it will be evaluated with humans, preferring
validated instruments and stating their known limitations.

## Project Principles

### [PRINCIPLE_1_NAME]
<!-- Example: IX. Real-Time Audio Path Is Allocation-Free -->
[PRINCIPLE_1_DESCRIPTION]

### [PRINCIPLE_2_NAME]
<!-- Add or remove project principles as needed; numbering continues after VIII -->
[PRINCIPLE_2_DESCRIPTION]

## [SECTION_2_NAME]
<!-- Example: Additional Constraints, Hardware & Platform Requirements, etc. -->
[SECTION_2_CONTENT]

## Governance
<!-- hri-core principles (I–VIII) may be tightened by a project but only weakened
     through a documented amendment stating the rationale and the mitigation. -->
[GOVERNANCE_RULES]

**Version**: [CONSTITUTION_VERSION] | **Ratified**: [RATIFICATION_DATE] | **Last Amended**: [LAST_AMENDED_DATE]
