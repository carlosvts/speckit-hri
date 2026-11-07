{CORE_TEMPLATE}

## HRI Rules (hri-core)

- HRI tasks are mandatory even when tests were not requested.
- Every requirement ID in the Human-Robot Interaction section of spec.md (core and profile
  prefixes such as AUD-, VIS-) MUST have at least one implementation task and one verification
  task, tagged [HRI:<ID>].
- Place SAFE- enforcement, TIM- instrumentation, the CTRL- pause/stop path, and any profile task
  marked "place in Phase 2" in Phase 2 (Foundational). Place HRI verification after the user
  stories it covers and before Polish.
- Remove the placeholder "HRI Tasks" section from the final tasks.md once its tasks are placed
  in the phases above.
