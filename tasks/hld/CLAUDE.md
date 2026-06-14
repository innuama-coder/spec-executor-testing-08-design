# CLAUDE.md

## Assignment

使用 `hld-writing` 技能，为任务执行摘要功能编写 HLD。

如果 `outputs/PRD.md` 不存在或内容不足，请停止并输出 blocker，不得编造上游 PRD。

## Context To Load

- `C:/Users/54256213/.codex/skills/hld-writing/SKILL.md`
- `briefs/feature-brief.md`
- `outputs/PRD.md`
- `docs/HLD.md`

## Constraints

- 不修改 task package。
- 不实现代码。

## Acceptance Criteria

- `outputs/HLD.md` 存在并包含 HLD 标题、架构、数据流和 ADR。
- `outputs/PRD.md` 已存在并被实际引用。

## Verification Method

运行 spec.yaml 中的 verify 命令。

## Handoff

说明 HLD 路径和 LLD 输入。
