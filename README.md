# cursorrules
Simple rules - smarter Cursor

## About This Repository

This repository contains rules and guidelines for Cursor AI to ensure safer interactions when working with code and version control.

## Table of Contents

- [Git Safety Rule](#git-safety-rule) - Never execute git commands automatically
- [PR Code Review Rule](#pr-code-review-rule) - Comprehensive code review analysis
- [Documentation Location Rule](#documentation-location-rule) - Organize docs by purpose
- [MCP Tool Definition Rule](#mcp-tool-definition-rule) - Guidelines for MCP tool documentation
- [Usage](#usage) - How to activate the rules

## Git Safety Rule

The **Git Safety Rule** (`.cursor/rules/git-safety.mdc`) ensures AI never executes git commands automatically.

**🛡️ Never execute git commands automatically** - The AI must always ask for explicit permission before running any git operations, explain the action, wait for confirmation, and provide alternatives when possible.

## PR Code Review Rule

The **PR Code Review Rule** (`pr-code-review`) provides comprehensive code review analysis before publishing pull requests.

**🔍 Challenge-first mindset** - Questions architectural decisions, examines diffs against the default branch, and provides thorough feedback on code quality, security, performance, and maintainability. Automatically challenges code with questions like "Why this approach?", "What are the trade-offs?", and "How will this scale?"

## Documentation Location Rule

The **Documentation Location Rule** (`docs-location`) establishes clear guidelines for where documentation should be placed.

**📂 Organize docs by purpose** - Technical design documents go in the central docs/ folder, while feature READMEs stay with their code. This keeps design docs discoverable while maintaining contextual relevance for feature documentation.

## MCP Tool Definition Rule

The **MCP Tool Definition Rule** (`mcp-tool-definition`) provides guidelines for documenting MCP Server tools.

**📋 Clear tool documentation** - Establishes a standardized structure for describing MCP tools with outcome-focused titles (e.g., "Analyze Stock Performance Metrics" not "Stock Analysis Tool") and comprehensive descriptions covering what it is, what it does, when to use it, and what it returns.

## Usage

Place the rules from this repository in your `.cursor/` directory to activate them for your Cursor AI sessions.
