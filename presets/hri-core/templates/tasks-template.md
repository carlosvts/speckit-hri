## HRI Tasks *(mandatory — hri-core)*

<!--
  ACTION REQUIRED: hri-core section. Derived from "HRI Design" in plan.md.
  These tasks are NOT optional, even when tests were not requested.
  Placement rules:
  - Safety-limit enforcement (SAFE-) and timing instrumentation (TIM-) are
    blocking: generate them inside Phase 2 (Foundational), tagged [HRI:<ID>].
  - Verification tasks below run after the user stories they cover, before Polish.
  Tag every HRI task with the spec ID it satisfies, e.g. [HRI:SAFE-001].
-->

### Foundational HRI (place in Phase 2)

- [ ] TXXX [HRI:SAFE-001] Enforce hard output limits in [component], independent of inference/mapping
- [ ] TXXX [P] [HRI:TIM-001] Add per-stage timestamps for the end-to-end timing budget
- [ ] TXXX [P] [HRI:CTRL-001] Implement pause/stop path that bypasses the pipeline

### HRI Verification (after user stories, before Polish)

- [ ] TXXX [P] [HRI:SAFE-001] Test that extreme/invalid inferred states never exceed output limits
- [ ] TXXX [P] [HRI:TIM-001] Measure end-to-end and per-stage latency (p95/p99) against the budget
- [ ] TXXX [P] [HRI:FAIL-001] Inject each failure in the Failure Handling table and verify fallback + recovery
- [ ] TXXX [P] [HRI:PRIV-001] Verify no raw sensor data is persisted or leaves the device unless specified
- [ ] TXXX [P] [HRI:CTRL-001] Verify pause/stop takes effect within the planned worst-case time
- [ ] TXXX [HRI:EVAL-001] Prepare evaluation protocol, consent form and instruments per the Evaluation Plan
