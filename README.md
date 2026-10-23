# Pipeline Rehearsal Lab

This repository is a disposable sandbox for rehearsing the release-day routine end to end, so the onboarding walkthrough can point at real artifacts.

## What the rehearsal exercises

- **A docs change**: this README was rewritten on the default branch as the docs-change step.
- **CI**: a smoke workflow lives at `.github/workflows/smoke.yml` and runs on every push.
- **An audit trail**: an issue ("Pipeline rehearsal checklist") tracks each step, with an audit comment recording the run's numeric ID, outcomes, and log evidence.
- **Notification hygiene**: the repository's notifications are set to ignore so the rehearsal stops pinging anyone.

## The loop, in order

1. README updated on the default branch.
2. `.github/workflows/smoke.yml` pushed, which kicks off a run of the "Smoke" workflow.
3. That run is re-run in its entirety.
4. Logs for the run are pulled down and referenced in the audit comment.
5. The issue thread is read back to confirm the audit comment's ID and timestamp.
6. Notifications for this repository are set to ignore.

> This repository is intentionally disposable. It exists for the demo and can be deleted after the onboarding session.

Rehearsal checkpoint: this line landed on the default branch after PR #1 opened, so the PR branch is now stale.
