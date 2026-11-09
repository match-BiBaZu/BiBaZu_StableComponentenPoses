# Df1a: 10,000 drops with the moving belt

[Workpiece catalogue](../../../README.md) · [Run overview](../README.md)

**9,999 of 10,000 trials settled**. Belt speed: 100 ± 3 mm/s. Seed: 42. Workers: 24. Pose grouping was disabled.

The moving outcome is recorded at the virtual exit while the belt runs. The separate post-exit observation brakes the belt over 0.2 s and observes the workpiece for 2 s with the belt stopped.

Each settled trial retains its own orientation and trial ID. The archived frequency rows describe individual trials.

[Simulator revision](https://github.com/match-BiBaZu/BiBaZu_PoseFindingDropSim/commit/72b1ba08aa9b317804cd60e1e2ae6e636910f3fd)

The [complete run archive](simulation_results.tar.xz) includes trial records, roughness events, post-braking observations where recorded, the original configuration, and the manifest. The downloadable configuration beside it uses a relative mesh path.

- [Summary](summary.json)
- [Configuration](config.json)
- [Manifest](manifest.json)
- [Validation](validation.json)
- [Execution record](execution.json)
- [Archive checksums](archive_contents.sha256.json)

Extract with `python -m tarfile -e simulation_results.tar.xz extracted`.
