# HLD - 设计型测试仓库

## 架构

设计任务以 `briefs/feature-brief.md` 为输入，按 PRD、HLD、LLD 的顺序输出到 `outputs/`。HLD 必须以已完成的 `outputs/PRD.md` 为输入，LLD 必须以已完成的 `outputs/PRD.md` 和 `outputs/HLD.md` 为输入。

```mermaid
flowchart LR
    A["feature brief"] --> B["PRD task"]
    B --> C["HLD task"]
    C --> D["LLD task"]
```

## 执行顺序

| 顺序 | 任务 | 前置条件 |
| --- | --- | --- |
| 1 | `tasks/prd` | `briefs/feature-brief.md` 存在。 |
| 2 | `tasks/hld` | `outputs/PRD.md` 已完成并通过验收。 |
| 3 | `tasks/lld` | `outputs/PRD.md` 与 `outputs/HLD.md` 已完成并通过验收。 |
