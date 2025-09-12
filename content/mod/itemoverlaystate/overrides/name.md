---
title: "物品显示名称 name"
cascade:
  type: docs
---

## name
值类型：字符串类型（正则表达式）

以正则表达式的形式判断物品显示的名称（翻译或重命名后的名称）

{{< callout type="info" >}}
**提示：** [正则表达式 - 教程](https://www.runoob.com/regexp/regexp-tutorial.html)
{{< /callout >}}

### 示例
```json lines {linenos=table,filename="json"}
{ "ios:name": "物品名称" }

{ "ios:name": " *-?\d+(\.\d+)? *" }
```