# Workflow Changelog

## setup-node-pnpm.yml

- Reusable setup with caching, optional install, build, fix, test, and check steps
- Also runs log-repo-status and exposes repo state outputs

## changeset-pr.yml

- Creates prerelease PRs using changesets/action@v1
- Auto-commits version bump and sets clear title/branch

## release.yml

- Uses `setup-node-pnpm`, blocks if repo is dirty, otherwise proceeds with tagging/publishing

## pre-release.yml

- Uses setup for fix/docs builds and prints finalization placeholder

## release-candidate.yml

- Validates that repo is clean before merging to main, runs fix/test

## test.yml

- Basic test flow that installs, fixes, and tests with logger output
