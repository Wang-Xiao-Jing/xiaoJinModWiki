---
title: "物品nbt nbt"
cascade:
  type: docs
---

## nbt
值类型：对象

按照物品nbt中是否匹配json的nbt判断

{{< callout type="info" >}}
**提示：** 按（默认）F6获取手持物品nbt
{{< /callout >}}

### 示例
```json lines {linenos=table,filename="json"}
{
  "ios:nbt": {
    "nbt名称": 1,
    "nbt名称1": "nbt值1",
    "nbt名称2": {
      "nbt名称3": "nbt值3"
    },
    "nbt名称4": [
      "nbt值4", "nbt值5"
    ],
    "nbt名称5": false,
    "nbt名称6": [
      {
        "nbt键1": "nbt值7"
      }
    ]
  }
}
```