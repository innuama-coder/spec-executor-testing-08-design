# spec-executor-testing-08-design

设计型独立测试仓库。该仓库用于验证 spec-executor 是否能够驱动 agent 使用 PRD/HLD/LLD 相关技能完成设计文档交付。

## 目录

- `docs/PRD.md`
- `docs/HLD.md`
- `docs/LLD.md`
- `docs/DELIVERY.md`
- `briefs/feature-brief.md`
- `tasks/prd/`
- `tasks/hld/`
- `tasks/lld/`

## 运行

```bash
spec-executor run --spec tasks/prd/spec.yaml --workspace ./workspace
spec-executor run --spec tasks/hld/spec.yaml --workspace ./workspace
spec-executor run --spec tasks/lld/spec.yaml --workspace ./workspace
```
