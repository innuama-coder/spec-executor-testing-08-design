# AGENTS.md

## Current Task

Use hld-writing to create `outputs/HLD.md`.
If `outputs/PRD.md` is missing or insufficient, stop with a blocker instead of inventing upstream requirements.

## Source Of Truth

- `PROMPT.md`
- `briefs/feature-brief.md`
- `outputs/PRD.md`

## Allowed Scope

- `outputs/HLD.md`

## Forbidden Scope

- Do not edit task package files.
- Do not implement code.

## Completion Criteria

HLD is complete, verifiable, and references the existing `outputs/PRD.md`.

## Required Verification

Run the verify command in `spec.yaml`.
