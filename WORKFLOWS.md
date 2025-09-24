## Hello CI
- Purpose: sanity check to confirm Actions is working.
- Triggers: push, manual.
- Jobs: say-hello (prints a message).
- Secrets: none.

## CI Pipeline
- Purpose: simple CI with lint, test, build (simulated with echo).
- Triggers: push to main, pull_request to main, manual.
- Jobs: lint → test → build (separate jobs).
- Secrets: none.
- Troubleshooting: make sure file is in `.github/workflows/ci.yml`.

## Advanced Workflows
- Purpose: scheduled maintenance + simulated deploy.
- Triggers: daily schedule, manual.
- Jobs: dependency-check, deploy (echo steps).
- Secrets: none.
- Troubleshooting: if it doesn’t run immediately, use the manual **Run workflow** button.
MD
git add WORKFLOWS.md
git commit -m "add WORKFLOWS.md documentation"
git push origin main


