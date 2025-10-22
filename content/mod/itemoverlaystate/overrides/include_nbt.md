---
title: "包含nbt include_nbt"
cascade:
  type: docs
---

## include_nbt
值类型：字符串类型、字符串列表类型

按照物品nbt中是否包含json所列出的nbt判断  
只会查找nbt和nbt的tag里面的第一层

{{< callout type="info" >}}
**提示：** 按（默认）F6获取手持物品nbt
{{< /callout >}}

### 示例
```json lines {linenos=table,filename="json"}
{ "ios:include_nbt": "nbt名称" }

{ "ios:include_nbt": ["nbt名称1", "nbt名称2"] }
```