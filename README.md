# cursorrules
Simple rules - smarter Cursor

## About This Repository

This repository contains a collection of rules and guidelines for Cursor AI to ensure safer, more predictable interactions when working with code and version control. The goal is to provide AI assistants with clear boundaries and best practices that protect your codebase and workflow.

## Git Safety Rule

One of the core rules in this repository is the **Git Safety Rule** (`.cursor/git-safety.mdc`), which establishes a critical safety protocol:

**🛡️ Never execute git commands automatically** - The AI must always ask for explicit user permission before running any git operations, regardless of how casual or urgent the request might seem.

### Why This Matters

Git operations can have significant impacts on:
- Project history and collaboration
- Deployment processes  
- Team workflows and CI/CD pipelines
- Risk of data loss through improper operations

### Covered Operations

The rule applies to ALL git commands including:
- `git add`, `git commit`, `git push`
- `git pull`, `git merge`, `git rebase` 
- `git checkout`, `git branch`, `git reset`
- `git stash`, `git fetch`, `git clone`, `git init`
- Any other `git` command

### How It Works

Instead of executing git commands automatically, the AI will:
1. **Ask for explicit permission** before proposing any git operation
2. **Explain the action** and why it's needed
3. **Wait for confirmation** before proceeding
4. **Provide alternatives** when possible

This ensures you maintain full control over your version control workflow while still getting helpful assistance with code changes.

## Usage

Place the rules from this repository in your `.cursor/` directory to activate them for your Cursor AI sessions.
