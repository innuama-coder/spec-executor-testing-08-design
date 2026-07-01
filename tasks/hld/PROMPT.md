# PROMPT.md

## 任务目标

使用 `hld-writing` 技能，基于 PRD 和功能简报编写 HLD。

如果 `outputs/PRD.md` 不存在或内容不足，请停止并输出 blocker，不得编造上游 PRD。

## 必读上下文

1. `C:/Users/54256213/.codex/skills/hld-writing/SKILL.md`
2. `briefs/feature-brief.md`
3. `outputs/PRD.md`
4. `docs/HLD.md`

## 交付物

- `outputs/HLD.md`

## 验收标准

- 文档使用简体中文。
- 包含架构、数据流、模块边界、ADR 和风险。
- `outputs/PRD.md` 已存在并被实际引用。

## Handoff

最终回复包含 HLD 路径和 LLD 输入。

## spec-executor 2.3 Agent Task Lifecycle 约束

- 本任务包通过 `spec.yaml` 的 `execution.agent` 声明 Agent 角色、上下文、工具和权限边界。
- `ENV` 仅用于 tmux session 环境变量注入，不作为普通上下文文件读取、总结或输出。
- 默认输出、报告和交付说明不得包含 `ENV` 变量值。
- `spec.yaml` 中存在 review items 时，必须在同一 JOB 内逐条完成修复、验证和交付记录。
- 运行过程必须保持 log-first detection 边界；screen capture 只作为显式查看或失败证据。
