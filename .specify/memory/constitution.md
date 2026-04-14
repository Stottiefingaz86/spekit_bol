# spekit_bol Constitution

## Core Principles

### I. Spec-Driven Development (NON-NEGOTIABLE)

All feature work, refactors, and multi-file or behavior-changing development **must** follow the GitHub Spec Kit pipeline: **specify → plan → tasks → implement**, with artifacts under `specs/` and the Cursor rule `.cursor/rules/spec-kit-required.mdc`. Requirements may be written in chat or imported (PRD, tickets, markdown); they are captured in a feature spec before implementation proceeds.

Optional steps when they reduce risk: clarify before plan; checklist after plan; analyze before implement.

Trivial, single-file, non-behavior edits (typos, comments, formatting only) may skip a new spec when they do not affect product behavior.

### II. Quality and correctness

Implementations must match the approved spec and task list; drift requires updating the spec or plan first, then code.

### III. Stack and structure

The primary application lives under `design-main/`; respect its existing patterns, routing, and component governance rules in `design-main/.cursor/rules/`.

### IV. Safety and review

Do not commit secrets; treat agent-local config under `.cursor/` as sensitive where credentials may appear.

### V. Simplicity

Prefer the smallest change that satisfies the spec; avoid scope creep without an updated spec.

## Additional constraints

Expand here as the product matures: performance budgets, accessibility bar, API contracts, etc.

## Development workflow

1. Use **speckit-constitution** / this file for governing principles.
2. **speckit-specify** — requirements → `specs/<feature>/`.
3. **speckit-plan** — technical plan from the spec.
4. **speckit-tasks** — ordered, implementable tasks.
5. **speckit-implement** — code changes in the repo.

## Governance

This constitution and the Cursor rule `.cursor/rules/spec-kit-required.mdc` define how work is done. Changes to process require updating both together when the rule and constitution should stay aligned.

**Version**: 1.0.0 | **Ratified**: 2026-04-14 | **Last Amended**: 2026-04-14
