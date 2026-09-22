# launch-score-runner

Temporary public CI runner for the Launch Score pipelines while GitHub
Actions is unavailable in the private data repository (provider-side
billing incident, ticket filed).

This repository contains **workflow definitions only**. Every script,
config, and data file lives in the private data repository, which each
run checks out with a fine-grained access token and pushes results back
to. No scripts, no data, and no credentials are stored here; secrets are
GitHub repository secrets.

Reversal: when Actions in the private repository recovers, re-enable the
schedules there, point the external dispatcher back, and archive this
repository.
