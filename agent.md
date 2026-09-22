# ProcessIQ Agent Guide

## Project overview

ProcessIQ is an AI-powered manufacturing process planning and optimization platform for the SISTEC Hackathon (IA-10). The platform generates candidate manufacturing processes, then uses deterministic validation and optimization components to verify and refine those outputs before they can be treated as valid manufacturing instructions.

## Core operating principles

- AI-generated suggestions are candidates only.
- Validation and optimization must verify all AI output before it can be used as manufacturing guidance.
- Never assume AI output is correct or safe for production use.
- Do not fabricate manufacturing data or process information.
- Keep implementations aligned with the hackathon problem statement and project intent.
- Do not copy code from the Bulwark reference repository.
- Bulwark is permitted only as an architectural/documentation reference.

## Repository structure

- `frontend/` — Frontend application
- `backend/` — Backend API
- `ai/` — AI and optimization logic
- `data/` — Manufacturing knowledge
- `docs/` — Documentation
- `tests/` — Testing
- `scripts/` — Development utilities

## Required workflow

1. Never work directly on `main`.
2. Create and use feature branches for changes.
3. Keep commits focused and small.
4. Never commit API keys, credentials, or secrets.
5. Keep API contracts explicit and documented.
6. Document any architectural or system-level changes.
7. Prefer minimal, necessary technologies over broad or unnecessary additions.
8. Validate AI outputs before integrating or exposing them.
9. Keep the implementation faithful to the problem statement.

## Branch strategy

- `main` — Stable release
- `develop` — Integration branch
- `feature/frontend` — Frontend work
- `feature/backend` — Backend work
- `feature/ai-planner` — AI and optimization work
- `feature/validation` — Knowledge, validation, and testing work

## Development expectations

- Favor deterministic validation flows over trusting generated output.
- Maintain clean separation between AI generation, validation, and optimization.
- Ensure tests cover critical logic, validation behavior, and integration boundaries.
- Be explicit when assumptions are made about manufacturing knowledge or process rules.
- Prefer clarity and maintainability over cleverness.

## Response style for future agent work

When making changes in this repository:

- Work from a feature branch instead of `main`.
- Keep edits scoped to the relevant area.
- Update docs when architecture or contracts change.
- Avoid introducing hidden dependencies or broad refactors without necessity.
- Flag any risk where AI-generated content may be treated as authoritative without validation.

## Summary

This repository is a disciplined engineering project: build AI-assisted manufacturing planning with strong verification, explicit contracts, and careful validation of all generated outputs.
