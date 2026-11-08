# Contributing

Thanks for helping. Repository-specific rules (in that repo's `CONTRIBUTING.md` or `.claude/`)
take precedence over this file.

## Workflow

1. Open or find an issue first for anything larger than a typo.
2. Branch from the default branch: `feat/<name>`, `fix/<name>`, `docs/<name>`.
3. Keep the pull request focused; fill in the template; CI must be green.
4. One maintainer approval is required to merge.

## Standards

| Topic | Rule |
|-------|------|
| Commits | [Conventional Commits](https://www.conventionalcommits.org/) with a scope: `fix(control): clamp PWM duty` |
| Versions | [SemVer](https://semver.org/); user-visible changes get a `CHANGELOG.md` entry |
| Headers | `SPDX-License-Identifier: Apache-2.0` + `Copyright (c) 2025 TNG-Blue` in every source file |
| Style | Python: `black` + `flake8` · C/C++/CUDA: `clang-format` (Google) · Go: `gofmt` · Shell: `shellcheck` |
| Tests | New behaviour comes with a test; bug fixes with a regression test |

## Control and estimation code

Anything that reads a sensor and commands an actuator must follow the chain
**sensor → filter → estimator → controller → actuator → feedback**, closed loop unless the
controlled state is unobservable (then: state why, bound the error, add a watchdog). The pull
request must state the plant model, sample time, filter and estimator choice, controller
derivation, and stability margins (GM ≥ 6 dB, PM ≥ 45°, delays included) or a Lyapunov argument,
with a cited reference. No tuned-by-feel constants.

## Licence and CLA

Contributions are accepted under Apache-2.0. Where a repository has a `CLA.md`, comment
`I have read and agree to the CLA` on your first pull request.
