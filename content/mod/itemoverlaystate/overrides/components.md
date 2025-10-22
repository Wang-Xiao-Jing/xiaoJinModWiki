---
title: "组件 components"
cascade:
  type: docs
---

{{< callout type="info" >}}
**提示：** 需要写原版命名空间
{{< /callout >}}
{{< callout type="info" >}}
**提示：** 我的世界版本1.20.5之前的版本请使用[nbt](../nbt)
{{< /callout >}}
{{< callout type="info" >}}
**提示：** 按（默认）F6获取手持物品信息
{{< /callout >}}
{{< callout type="info" >}}
**提示：** 数字（字节，整数，浮点数）判断走的是大小判断，json小于的判断的数字
{{< /callout >}}

### 示例
```json lines {linenos=table,filename="json"}
{
  "ios:nbt": {
    "物品组件id": 1,
    "物品组件id1": "值",
    "物品组件id2": {
      "属性1": "值1"
    },
    "物品组件id3": [
      "属性2", "值2"
    ],
    "物品组件id4": false,
    "物品组件id5": [
      {
        "属性3": "值3"
      }
    ]
  }
}
```