# Kl4i: 10,000 drops with the stationary belt

[Workpiece catalogue](../../../README.md) · [Run overview](../README.md)

**9,995 of 10,000 trials settled**. Belt speed: 0 mm/s. Seed: 42. Workers: 24. Pose grouping was disabled.

The stationary outcome is evaluated after 10 seconds with the belt stationary from release.

Each settled trial retains its own orientation and trial ID. The archived frequency rows describe individual trials rather than grouped pose classes.

The settings match the archived reference configuration for the earlier twelve-workpiece study. The additional post-exit braking observation remains enabled for the moving condition.

[Simulator revision](https://github.com/match-BiBaZu/BiBaZu_PoseFindingDropSim/commit/72b1ba08aa9b317804cd60e1e2ae6e636910f3fd)

The [complete run archive](simulation_results.tar.xz) preserves all original run files, including CSV/JSONL trial records, the full summary, roughness events, post-braking observations where recorded, the original configuration, and the manifest. The downloadable configuration beside it uses a relative path to the workpiece STL.

- [Compact summary](summary.json)
- [Configuration](config.json)
- [Manifest](manifest.json)
- [Validation](validation.json)
- [Execution record and reference comparison](execution.json)
- [Archive checksums](archive_contents.sha256.json)
- [File checksums](files.sha256.json)

Extract with `python -m tarfile -e simulation_results.tar.xz extracted`.
