---
title: "物品损伤 damage"
cascade:
  type: docs
---

## damage
值类型：数字类型、字符串类型  
字符串格式："100.00%"  
支持小数

按照物品已损伤（耐久）值判断，如果是填写百分比则按照百分比判断，否则按照数值判断

### 示例
```json lines {linenos=table,filename="json"}
{ "ios:damage": 50 }

{ "ios:damage": "50%" }
```