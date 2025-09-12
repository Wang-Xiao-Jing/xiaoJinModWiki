---
title: "包含附魔 includeEnchantment"
cascade:
  type: docs
---

## includeEnchantment
值类型：字符串类型、字符串列表类型

按照物品附魔是否包含json所列出的附魔判断

### 示例
```json lines {linenos=table,filename="json"}
// 原版附魔可以省去命名空间
{ "ios:includeEnchantment": "附魔注册id" }

{ "ios:includeEnchantment": ["附魔注册id1", "附魔注册id2"] }
```