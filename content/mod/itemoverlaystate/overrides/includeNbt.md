---
title: "包含nbt includeNbt"
cascade:
  type: docs
---

## includeNbt
值类型：字符串类型、字符串列表类型

按照物品nbt中是否包含json所列出的nbt判断  
只会查找nbt和nbt的tag里面的第一层

{{< callout type="info" >}}
**提示：** 按（默认）F6获取手持物品nbt
{{< /callout >}}

### 示例
```json lines {linenos=table,filename="json"}
{ "ios:includeNbt": "nbt名称" }

{ "ios:includeNbt": ["nbt名称1", "nbt名称2"] }
```