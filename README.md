# speckit-hri

Spec-driven development kit for human-robot interaction (HRI) software, built as
[GitHub Spec Kit](https://github.com/github/spec-kit) presets.

It adds HRI concerns to every spec, plan and task list: interaction context, signal
contracts, timing budgets, failure modes, privacy and consent, safety limits, and
evaluation with people. The principles are grounded in HRI literature (see each
preset's `REFERENCES.md`).

> **Status:** early (0.1.0). Requires Spec Kit ≥ 1.3.2.

## Presets

| Preset | What it adds |
|---|---|
| `hri-core` | HRI constitution (8 principles), HRI sections in spec/plan/tasks, HRI rules in `/specify`, `/plan`, `/tasks` |
| `hri-audio` | Audio output: hearing safety, latency and continuity, state-to-sound mapping, acoustic context |
| `hri-vision` | Vision sensing: camera privacy, fairness, capture conditions, validity of visual inference |

Profiles stack on top of `hri-core`; use the ones your project needs.

## Usage

```sh
git clone https://github.com/carlosvts/speckit-hri.git

# in your project
specify init --here --preset ../speckit-hri/presets/hri-core
specify preset add --dev ../speckit-hri/presets/hri-audio --priority 5
specify preset add --dev ../speckit-hri/presets/hri-vision --priority 5
```

Profiles **must** be installed with `--priority 5` (lower than `hri-core`'s default 10) so
their sections land inside the HRI section. Check with `specify preset list`.

For an existing project, use `specify preset add --dev .../hri-core` instead of `init`.
The HRI constitution is only seeded when `.specify/memory/constitution.md` does not exist yet.

Project-specific values go in your own repo, e.g. as overrides in
`.specify/templates/overrides/` (an override replaces the whole template).

## License

[Apache-2.0](LICENSE)
