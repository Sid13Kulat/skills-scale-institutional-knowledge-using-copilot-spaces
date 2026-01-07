# OctoAcme — QA Automation Guidelines

Purpose: Provide a pragmatic approach to automated testing that balances speed, reliability, and coverage.

## Testing pyramid (recommended)
- Unit tests: fast, isolated — highest volume
- Integration tests: critical path integrations tested
- End-to-end tests: limited, high-value flows only

## CI gates & thresholds
- All PRs must run unit tests and linting
- Merge blocked if essential unit tests fail
- Smoke or critical-path e2e tests should run on release branches

## Test ownership
- Developers own unit tests for their code
- QA Automation Lead owns test strategy and shared e2e suites
- Developers and QA collaborate on flaky test triage and remediation

## Test data and environments
- Use reproducible test data or fixtures
- Keep e2e environments as close to production as practical
- Isolate test accounts/keys and rotate credentials regularly

## Flaky test policy
- Track flaky tests, add issue with owner for remediation
- Avoid masking flakiness with retries above a project-defined threshold
- Prioritize stable test signals for gating releases

## CI tips
- Keep CI jobs fast and parallelizable
- Cache dependencies where appropriate
- Fail fast: run quick checks before slower suites