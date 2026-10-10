---
name: GitHub API vs. Git push
description: Distinguishes Replit's GitHub API connector from shell Git authentication.
---

Do not assume that adding a GitHub OAuth connection authenticates `git push` from the workspace shell. The connector routes authenticated GitHub API calls through its proxy; shell Git still depends on its own configured transport credentials.

**Why:** A valid GitHub remote rejected the workspace's shell push with an authentication error, while the Replit integration exposed authenticated API access separately.

**How to apply:** If shell push fails, do not request or print a password or token. Use the user's authenticated GitHub flow or an available supported integration path, and clearly report whether the local branch was pushed.
