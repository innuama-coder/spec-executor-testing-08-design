# CLAUDE.md

## Assignment

编写任务执行摘要功能的 LLD。

如果 `outputs/PRD.md` 或 `outputs/HLD.md` 不存在或内容不足，请停止并输出 blocker，不得编造上游设计。

## Context To Load

- `outputs/PRD.md`
- `outputs/HLD.md`
- `docs/LLD.md`

## Constraints

- 不修改 task package。
- 不实现代码。

## Acceptance Criteria

- `outputs/LLD.md` 存在并包含接口、数据结构、错误处理和测试矩阵。
- `outputs/PRD.md` 与 `outputs/HLD.md` 已存在并被实际引用。

## Verification Method

运行 spec.yaml 中的 verify 命令。

## Handoff

说明 LLD 路径和开发任务建议。

## spec-executor 2.3 Agent Task Lifecycle 约束

- 本任务包通过 `spec.yaml` 的 `execution.agent` 声明 Agent 角色、上下文、工具和权限边界。
- `ENV` 仅用于 tmux session 环境变量注入，不作为普通上下文文件读取、总结或输出。
- 默认输出、报告和交付说明不得包含 `ENV` 变量值。
- `spec.yaml` 中存在 review items 时，必须在同一 JOB 内逐条完成修复、验证和交付记录。
- 运行过程必须保持 log-first detection 边界；screen capture 只作为显式查看或失败证据。
