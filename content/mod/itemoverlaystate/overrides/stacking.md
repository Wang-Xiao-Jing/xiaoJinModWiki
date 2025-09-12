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

### 示例
```json lines {linenos=table,filename="json"}
{ "ios:stacking": 50 }

{ "ios:stacking": "50%" }
```