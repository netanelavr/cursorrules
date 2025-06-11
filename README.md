# cursorrules
Simple rules - smarter Cursor

## About This Repository

This repository contains rules and guidelines for Cursor AI to ensure safer interactions when working with code and version control.

## Git Safety Rule

The **Git Safety Rule** (`.cursor/rules/git-safety.mdc`) establishes a critical safety protocol:

**🛡️ Never execute git commands automatically** - The AI must always ask for explicit user permission before running any git operations.

### How It Works

The AI will:
1. **Ask for explicit permission** before any git operation
2. **Explain the action** and why it's needed  
3. **Wait for confirmation** before proceeding
4. **Provide alternatives** when possible

This ensures you maintain full control over your version control workflow.

## Usage

Place the rules from this repository in your `.cursor/` directory to activate them for your Cursor AI sessions.
