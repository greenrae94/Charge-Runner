# Workflow

## Branch strategy

This project uses four branch types:

- `main`  
  Shipped code only. Anything on `main` should be considered release-ready and live/signed-off.

- `staging`  
  Stable and promotable work. Code on `staging` is considered stable and could be merged to `main` when desired, but may be waiting on timing, coordination, or other planned changes.

- `develop`  
  Sandbox and integration branch. This branch is used for testing, experimentation, and validating feature branches together before promotion upward.

- `feature/*`  
  Focused branches for individual pieces of work. Early in the project these may cover broad areas; later they should become more targeted.

## Promotion flow

Work should move through branches in this order:

`feature/*` → `develop` → `staging` → `main`

## Rules

- Do not work directly on `main`, `staging`, or `develop`.
- Use `feature/*` branches for all changes.
- Merge features into `develop` first.
- Promote tested work from `develop` to `staging`.
- Promote stable release-ready work from `staging` to `main`.
- Treat `main` as shipped history.
- Treat `staging` as stable but not yet shipped.
- Treat `develop` as sandbox/integration space.

## Notes

- In the early project phase, feature branches may be larger and cover broader work.
- As the project grows, feature branches should become smaller and more specific.
- This workflow is intended to make testing, rollback, and release management easier.