# GitDone - Usage Guide

## What It Does
Tracks project completion by verifying claims against actual Git commits.

## How It Works
```
Markdown Table --> Parse Tasks --> Check Git --> Calculate % Done
   (plan.md)        (rows)       (commits/PRs)   (verified)
```

## Setup
```bash
pip install gitdone
gitdone init  # Creates plan.md template
```

## Plan Format
| Task | Branch/PR | Status |
|------|-----------|--------|
| Auth system | PR #12 | ✅ Verified |
| API endpoints | main@abc123 | ✅ Verified |
| Frontend | - | ❌ No commit |

## Key Features
- Zero dependencies (Python stdlib only)
- Refuses commits that inflate numbers
- Verifiable progress tracking