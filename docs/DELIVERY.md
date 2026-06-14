# DELIVERY - 设计型测试仓库

## 验收用途

本文档用于人工复核 PRD、HLD、LLD 三类设计任务是否按顺序完成，并确认下游设计没有脱离上游输入。

## 交付物

| 任务 | 交付物 | 前置条件 | 验收要点 |
| --- | --- | --- | --- |
| PRD | `outputs/PRD.md` | `briefs/feature-brief.md` | 包含修订表、目标、范围、FR、NFR 和验收标准。 |
| HLD | `outputs/HLD.md` | `outputs/PRD.md` | 包含架构、数据流、模块边界、ADR 和风险，并引用 PRD。 |
| LLD | `outputs/LLD.md` | `outputs/PRD.md`、`outputs/HLD.md` | 包含接口、数据结构、错误处理、测试矩阵和实现任务建议。 |

## 验收顺序

```mermaid
flowchart LR
    A["PRD 验收"] --> B["HLD 验收"]
    B --> C["LLD 验收"]
```

## 人工验收清单

- PRD、HLD、LLD 均使用简体中文。
- HLD 不在 PRD 缺失时编造需求。
- LLD 不在 PRD/HLD 缺失时编造详细设计。
- 每个文档均可独立说明目标、范围、约束和验收依据。
- 最终回复说明产物路径、上游依赖和开放问题。
