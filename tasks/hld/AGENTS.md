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

## spec-executor 2.3 Agent Task Lifecycle 约束

- 本任务包通过 `spec.yaml` 的 `execution.agent` 声明 Agent 角色、上下文、工具和权限边界。
- `ENV` 仅用于 tmux session 环境变量注入，不作为普通上下文文件读取、总结或输出。
- 默认输出、报告和交付说明不得包含 `ENV` 变量值。
- `spec.yaml` 中存在 review items 时，必须在同一 JOB 内逐条完成修复、验证和交付记录。
- 运行过程必须保持 log-first detection 边界；screen capture 只作为显式查看或失败证据。
