# PROMPT.md

## 任务目标

使用 `prd-writing` 技能，基于功能简报编写 PRD。

## 必读上下文

1. `C:/Users/54256213/.codex/skills/prd-writing/SKILL.md`
2. `briefs/feature-brief.md`
3. `docs/PRD.md`

## 交付物

- `outputs/PRD.md`

## 验收标准

- 文档使用简体中文。
- 包含修订表、目标、范围、FR/NFR、验收标准。

## Handoff

最终回复包含 PRD 路径和开放问题。

## spec-executor 2.3 Agent Task Lifecycle 约束

- 本任务包通过 `spec.yaml` 的 `execution.agent` 声明 Agent 角色、上下文、工具和权限边界。
- `ENV` 仅用于 tmux session 环境变量注入，不作为普通上下文文件读取、总结或输出。
- 默认输出、报告和交付说明不得包含 `ENV` 变量值。
- `spec.yaml` 中存在 review items 时，必须在同一 JOB 内逐条完成修复、验证和交付记录。
- 运行过程必须保持 log-first detection 边界；screen capture 只作为显式查看或失败证据。
