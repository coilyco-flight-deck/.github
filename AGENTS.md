---
ward:
  workflow: merge-remote-main
---
# Agent instructions

This repository owns the `coilyco-flight-deck` organization profile and shared
review metadata.

## Boundaries

* Edit `profile/README.md` for the public organization landing page.
* Keep the GitHub and Forgejo CODEOWNERS files aligned unless a platform
  requires a deliberate syntax difference.
* Keep all profile and documentation content public-safe.
* Regenerate the repository pointer skill through agentic-os. Do not hand-edit
  its generated `SKILL.md`.

## Checkout residency

This repo is not in Agent Compose's `repository-plan.yaml`, so it has no
resident checkout under `~/projects/<owner>/`. That is intentional. Work it
from a task-scoped temporary clone, and remove that clone once the work lands.

A temporary root can be purged at any time, so commit and push before pausing,
switching tasks, or ending a session. The remote is the only durable artifact.
