# OctoAcme — Release Checklist

This checklist standardizes pre-release, release, and post-release activities to reduce risk and improve observability.

## Pre-release (Before release window)
- [ ] Acceptance criteria met for all included work
- [ ] All PRs merged and CI green
- [ ] Security scans completed and findings triaged
- [ ] Release notes drafted and reviewed (include migration steps if needed)
- [ ] Rollback / mitigation plan documented
- [ ] Stakeholders notified of release scope and timing
- [ ] Smoke tests identified and automated where possible
- [ ] Support and on-call teams notified and aware of expected changes

## Release (During deployment)
- [ ] Deployment executed via CI/CD pipeline or approved manual steps
- [ ] Post-deploy smoke tests run and passed on production
- [ ] Monitoring and alerts are enabled / verified
- [ ] Release announcement sent to stakeholders and support channels
- [ ] Any migrations performed with verification steps completed

## Post-release (After deployment)
- [ ] Monitor metrics and error rates for the agreed observation window
- [ ] Capture and triage any production issues; create follow-up tasks
- [ ] Update the risk register and project status
- [ ] Retrospective/lessons learned if there were issues or significant changes
- [ ] Finalize and publish release notes (public/internal as required)

## Roles / Responsibilities (example)
- Release Manager: owns checklist, communication, and sign-off
- DevOps: executes pipeline and rollback
- QA: validates smoke tests and production verification
- Support Specialist: monitors incoming user reports

## Release notes template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps:
- Known issues: