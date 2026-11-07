{CORE_TEMPLATE}

## HRI Rules (hri-core)

- Fill the "HRI Design" section. Every requirement ID in the Human-Robot Interaction section of
  spec.md (core prefixes SIG-, TIM-, FAIL-, PRIV-, CTRL-, SAFE-, EVAL- and profile prefixes such
  as AUD-, VIS-) MUST appear in at least one row or bullet of HRI Design.
- The Constitution Check MUST evaluate principles I–VIII explicitly, one line each (pass / fail /
  justified in Complexity Tracking).
- The sum of per-stage timing budgets MUST NOT exceed the corresponding TIM- target. If it does,
  stop and report the conflict instead of inventing slack.
- Safety limits (SAFE-) MUST be enforced in a component independent of inference and mapping.
