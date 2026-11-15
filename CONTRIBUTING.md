# Contributing to Meala (`mealadev`)

Thank you for contributing to Meala! Whether you are adding support for a new autopilot telemetry message, improving the web dashboard, or refining documentation, your contributions help small UAV teams fly safer.

## Getting Started

1. Fork the target repository under `github.com/mealadev`.
2. Create a descriptive feature or fix branch (`git checkout -b feat/px4-ekf-parser`).
3. Make your changes and verify locally using Docker Compose or the Jupyter test suite.
4. Ensure no private flight logs, GPS coordinates from restricted sites, or API keys are committed.
5. Open a Pull Request using the PR template.

## Telemetry Schema Guidelines

When adding new extracted signals to the canonical DataFrame/Parquet pipeline:
* Use explicit SI units in column names (`_ms`, `_mps`, `_m`, `_v`, `_a`, `_deg`, `_pct`).
* Ensure missing topics in a given autopilot format degrade gracefully (defaulting to `NaN` or `0.0`) rather than crashing ingestion.
