# AGENTS.md

## Current Task

Create `outputs/LLD.md` for the execution summary feature.
If `outputs/PRD.md` or `outputs/HLD.md` is missing or insufficient, stop with a blocker instead of inventing upstream design.

## Source Of Truth

- `PROMPT.md`
- `outputs/PRD.md`
- `outputs/HLD.md`

## Allowed Scope

- `outputs/LLD.md`

## Forbidden Scope

- Do not edit task package files.
- Do not implement code.

## Completion Criteria

LLD is complete, verifiable, and references the existing `outputs/PRD.md` and `outputs/HLD.md`.

## Required Verification

Run the verify command in `spec.yaml`.
