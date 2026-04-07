# library-outsourcer

A Claude Code skill that evaluates whether open-source libraries can improve your coding outputs compared to building from scratch.

## Install

Copy this folder to `~/.claude/skills/library-outsourcer/`.

## Usage

Trigger by asking Claude Code to evaluate library options for a task, or invoke directly with `/library-outsourcer`.

## How it works

The skill runs a 6-phase workflow:

1. **Question** — Clarifies your desired outcome through guided Q&A
2. **Scope** — Explores your codebase to understand the task boundaries
3. **Assess** — Determines if library outsourcing is viable, including hybrid approaches
4. **Identify** — Finds relevant, reliable libraries (uses web search when needed)
5. **Present** — Ranks candidates by impact with clear tradeoffs and risk assessments
6. **Plan** — Creates a detailed integration plan for your approved selections

If libraries aren't viable at any point, the skill exits and lets you proceed from scratch.

## Requirements

- Claude Code
- Web search tool access (optional, improves library discovery in Phase 4)
