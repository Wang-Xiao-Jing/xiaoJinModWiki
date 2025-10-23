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
{{< callout type="info" >}}
**提示：** 数字（字节，整数，浮点数）判断走的是大小判断，json小于的判断的数字则触发成功，判断只有1或0的字节判断请走布尔值判断
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