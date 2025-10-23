---
title: "附魔 enchantment"
cascade:
  type: docs
---

## enchantment
值类型：对象

按照物品附魔是否满足json判断

{{< callout type="info" >}}
**提示：** 可以忽略原版附魔命名空间
{{< /callout >}}
{{< callout type="info" >}}
**提示：** 数字（字节，整数，浮点数）判断走的是大小判断，json小于的判断的数字则触发成功
{{< /callout >}}

### 示例
```json lines {linenos=table,filename="json"}
{
  "ios:enchantment": {
    // 原版附魔可以省去命名空间
    "附魔注册id": 附魔等级
  }
}
```