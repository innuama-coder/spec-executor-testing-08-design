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
