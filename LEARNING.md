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

## Session 6 — Open Source Collaboration

**Date:** June 2026

### What I learned

- The difference between team collaboration and open source collaboration
- How forking works — your personal copy of someone else's repo
- The three locations in open source: upstream, origin, local
- How to add an upstream remote to track the original repo
- How to open a PR from a fork to the original repository
- How to sync a fork after changes are merged upstream
- What happens after opening a PR: merge, request changes, or close

### Commands covered

- `git clone <fork-url>` — clone your fork locally
- `git remote add upstream <original-url>` — track the original repo
- `git remote -v` — verify remote connections
- `git pull upstream master` — sync from original repo
- `git push origin master` — update your fork on GitHub

### Key concepts

- origin = your fork on GitHub
- upstream = the original repository you forked from
- Always pull upstream before starting new work
- PRs go from your fork to the original repo, not within your fork
- Your contribution graph updates when PRs are merged into others' repos

### Full open source workflow

1. Fork the repo on GitHub
2. Clone your fork locally
3. Add upstream remote
4. Create a feature branch
5. Make changes, commit, push to your fork
6. Open PR from your fork to the original repo
7. Maintainer reviews and merges
8. Sync your fork: pull upstream → push origin

## Changelog

### v0.1.0 — June 2026

- Initialised learning log
- Documented Git fundamentals, branching, GitHub workflow
- Added professional workflow notes (rebase, squash, conventional commits)
- Documented UTF-16 .gitignore fix for Windows

### v0.2.0 — June 2026

- Added Session 5 notes covering professional Git usage
- Added troubleshooting entry for Windows .gitignore UTF-16 issue

### v0.3.0 — June 2026

- Added Session 6 notes covering open source collaboration
- Documented fork, upstream, and sync workflow
