---
title: SelectNode 选中节点
order: 16
group:
  path: /api/commands
  title: Command 命令
  order: 2
nav:
  title: API
  path: /api
  order: 1
---

## 移动节点

XFlow 提供节点添加的命令 `XFlowNodeCommands.SELECT_NODE`, 通过该命令可以实现在画布显示选中节点的状态

### Command 示例

<code src="./demos/index.tsx" classname="node-select-demo" />

### 命令参数（IArgs）

|           名称 |     类型 | 必选 | 默认值 | 描述                   |
| -------------: | -------: | ---: | -----: | ---------------------- |
|        nodeIds | string[] |    ✓ |      - | 选中的节点 id          |
| resetSelection |  boolean |      |      - | 取消所有节点的选中状态 |

```tsx | pure
export interface IArgs extends IArgsBase {
  /** 选中的节点id */
  nodeIds: string[]
  /** 取消所有节点的选中状态 */
  resetSelection?: boolean
}
```
