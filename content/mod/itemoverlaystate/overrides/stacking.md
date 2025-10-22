---
title: "物品堆叠数量 stacking"
cascade:
  type: docs
---

## stacking
值类型：数字类型、字符串类型  
字符串格式："100.00%"  
支持小数

按照物品当前堆叠数量判断，如果是填写百分比则按照占用当前格子的最大百分比判断，否则按照数值判断
{{< callout type="info" >}}
**提示：** 数字（字节，整数，浮点数）判断走的是大小判断，json小于的判断的数字则触发成功
{{< /callout >}}


### 示例
```json lines {linenos=table,filename="json"}
{ "ios:stacking": 50 }

{ "ios:stacking": "50%" }
```