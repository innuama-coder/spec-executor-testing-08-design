# LLD - 设计型测试仓库

## 任务约束

- PRD 输出必须面向用户价值。
- HLD 输出必须面向架构决策。
- LLD 输出必须面向可实现任务。
- HLD 不得在 `outputs/PRD.md` 缺失时编造 PRD 内容。
- LLD 不得在 `outputs/PRD.md` 或 `outputs/HLD.md` 缺失时编造上游设计。

## 验证

每个输出文档必须存在并包含对应标题。HLD 验收同时检查 PRD 前置产物，LLD 验收同时检查 PRD 和 HLD 前置产物。
