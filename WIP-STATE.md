# WIP state — morselhub.com

**Branch:** `wip/2026-09-16-plato` · **Created:** 2026-09-16 · **From:** plato (old Mac)

## Why this branch exists

Uncommitted work was sitting in the working tree on `plato` and existed
**nowhere else** — not on GitHub, not on any other machine. It was committed
here and pushed so the move to the new Mac can't lose it.

It was deliberately **not** pushed to `main`. See "Prod safety" below.

## What's in it

```
10 files changed, 407 insertions(+), 503 deletions(-)
```

Commit: `3e4de93`

## Status

- [ ] **Not reviewed.** This is a snapshot, not considered-good work.
- [ ] **Not merged.** `main` is untouched and still matches origin.
- [ ] Decide per-file what to keep, then merge or cherry-pick into `main`.

## Prod safety

This branch was pushed instead of `main` specifically so no deploy or
release workflow would fire. Before merging to `main`, know what that
triggers in this repo — check `.github/workflows/`.

## Picking this up elsewhere

```bash
git fetch origin
git checkout wip/2026-09-16-plato
git diff main...wip/2026-09-16-plato      # what this snapshot changed
```

Delete this file when the branch is merged or abandoned.
