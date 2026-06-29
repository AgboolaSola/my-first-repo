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

## Session 5 — Professional Git Usage

**Date:** June 2026

### What I learned

- Conventional Commits format: type(scope): description
- Common types: feat, fix, chore, docs, style, refactor, test
- Why conventional commits matter: readable history, automated
  changelogs, team communication
- .gitignore: how to tell Git which files to never track
- Windows UTF-16 encoding bug with .gitignore and how to fix it
- Git aliases: shortcuts for frequently used commands
- GitHub Issues: tracking bugs and features
- Auto-closing issues with `closes #N` in PR descriptions

### Commands covered

- `git config --global alias.name "command"`
- `git check-ignore -v filename`

### Key rules learned

- Never commit .env files — API keys become public on GitHub
- Don't alias destructive commands like reset --hard
- Use present tense in commit messages: `add` not `added`
- Keep commit descriptions under 72 characters
- Start descriptions with a verb: add, fix, update, remove

## Changelog

### v0.1.0 — June 2026

- Initialised learning log
- Documented Git fundamentals, branching, GitHub workflow
- Added professional workflow notes (rebase, squash, conventional commits)
- Documented UTF-16 .gitignore fix for Windows

### v0.2.0 — June 2026

- Added Session 5 notes covering professional Git usage
- Added troubleshooting entry for Windows .gitignore UTF-16 issue
