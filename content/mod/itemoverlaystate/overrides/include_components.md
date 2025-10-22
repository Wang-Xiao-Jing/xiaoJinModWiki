---
title: "包含组件 include_components"
cascade:
  type: docs
---

{{< callout type="info" >}}
**提示：** 可以忽略原版组件命名空间
{{< /callout >}}
{{< callout type="info" >}}
**提示：** 我的世界版本1.20.5之前的版本请使用[include_nbt](../include_nbt)
{{< /callout >}}
{{< callout type="info" >}}
**提示：** 按（默认）F6获取手持物品信息
{{< /callout >}}

### 示例
```json lines {linenos=table,filename="json"}
// 原版附魔可以省去命名空间
{ "ios:include_components": "物品组件id" }

{ "ios:include_components": ["物品组件id1", "物品组件id2"] }
```