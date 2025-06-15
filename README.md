# cursorrules
Simple rules - smarter Cursor

## About This Repository

This repository contains rules and guidelines for Cursor AI to ensure safer interactions when working with code and version control.

## Table of Contents

- [Git Safety Rule](#git-safety-rule) - Never execute git commands automatically
- [PR Code Review Rule](#pr-code-review-rule) - Comprehensive code review analysis
- [Documentation Location Rule](#documentation-location-rule) - Organize docs by purpose
- [Usage](#usage) - How to activate the rules

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

## PR Code Review Rule

The **PR Code Review Rule** (`pr-code-review`) provides comprehensive code review analysis before publishing pull requests:

**🔍 Challenge-first mindset** - Questions architectural decisions, examines diffs against the default branch, and provides thorough feedback on code quality, security, performance, and maintainability.

### Key Review Areas

The AI will analyze:
1. **Change Scope** - Diff analysis, impact assessment, breaking changes
2. **Architecture & Design** - Patterns, abstractions, SOLID principles
3. **Code Quality** - Naming, complexity, error handling, documentation
4. **Performance & Security** - Bottlenecks, vulnerabilities, resource management
5. **Testing & APIs** - Coverage, compatibility, deployment safety

### Review Questions

Automatically challenges code with key questions:
- Why this approach? Is there a simpler way?
- What are the trade-offs? What are we sacrificing?
- What could go wrong? Failure modes and edge cases?
- How will this scale with 10× load/data/users?
- How will we maintain this over time?

This ensures high-quality, maintainable code that meets project standards.

## Documentation Location Rule

The **Documentation Location Rule** (`docs-location`) establishes clear guidelines for where documentation should be placed:

**📂 Organize docs by purpose** - Technical design documents go in the central docs/ folder, while feature READMEs stay with their code.

### Documentation Structure

The rule enforces:
1. **Technical design documents** must be created in the **docs/** folder at the repository root
2. **Feature README files** must be placed next to the relevant feature code, not in docs/

### Rationale

- **Centralized design docs** in docs/ keeps them discoverable for architectural decisions
- **Co-located feature READMEs** help developers find usage and setup information in context with the code

This ensures documentation is both discoverable and contextually relevant.

## Usage

Place the rules from this repository in your `.cursor/` directory to activate them for your Cursor AI sessions.
