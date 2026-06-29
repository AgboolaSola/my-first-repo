# Git Learning Log

## Session 1 — Git Fundamentals

\*\*Date:22 June 2026

### What I learned

- The three areas of Git: Working Directory, Staging Area, Repository
- How to initialise a repo, stage changes, and commit snapshots
- How to read git log and understand commit hashes and HEAD

### Commands covered

- `git init`, `git add`, `git commit`, `git log`, `git status`
- `git restore`, `git restore --staged`

## Session 2 — Branching and Merging

\*\*Date:23 June 2026

### What I learned

- Why branches exist and how to create them
- How to merge branches and resolve conflicts manually
- The difference between fast-forward and merge commits

### Commands covered

- `git branch`, `git switch`, `git merge`

## Session 3 — GitHub

\*\*Date:25 June 2026

### What I learned

- How to connect a local repo to GitHub
- Push and pull workflow
- The difference between clone and pull

### Commands covered

- `git remote add origin`, `git push`, `git pull`, `git clone`

## Session 4 — Professional Workflow

\*\*Date:27 June 2026

### What I learned

- Feature branch workflow and Pull Requests
- Rebasing to keep history linear
- Squashing messy commits into one clean commit
- Conventional Commits format

### Commands covered

- `git rebase`, `git rebase -i`, `git push -u origin branch-name`

## Troubleshooting Log

### .gitignore not working on Windows

**Problem:** Created `.gitignore` using `echo` command on Windows.
Git was not ignoring files listed inside it.

**Cause:** Windows `echo` command saves files as UTF-16 encoding.
Git requires UTF-8.

**Fix:** Open `.gitignore` in VS Code, click the encoding in the
bottom right corner, select "Save with Encoding" → UTF-8.
