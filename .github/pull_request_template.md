## Summary

<!-- What changes and why. Link the issue: Closes #123 -->

## Breaking changes

<!-- None, or what breaks and how to migrate. -->

## Testing

<!-- Commands run and results; hardware/sim used. -->

## Checklist

- [ ] Conventional Commit messages with a scope
- [ ] SPDX Apache-2.0 header in every new source file
- [ ] Formatters and linters pass; tests added or updated and passing
- [ ] Docs and `CHANGELOG.md` updated for user-visible changes
- [ ] CLA accepted (first contribution, where the repository has `CLA.md`)

### Control / estimation changes only

- [ ] Signal chain: sensor → filter → estimator → controller → actuator → feedback (closed loop)
- [ ] Plant model, `T_s`, filter cut-off/phase lag and estimator `Q`/`R` stated with units
- [ ] Margins (GM ≥ 6 dB, PM ≥ 45°, delays included) or Lyapunov argument; reference cited
- [ ] Saturation, anti-windup and failsafe implemented
- [ ] Evidence attached: simulation → SIL → HIL / bench
