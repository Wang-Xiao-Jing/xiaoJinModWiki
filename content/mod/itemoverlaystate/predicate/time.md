---
title: "世界时间 time"
cascade:
  type: docs
---

## time
值类型：数字类型

按照当前游戏时间判断（游戏刻为单位）

{{< callout type="info" >}}
**提示：** 数字（字节，整数，浮点数）判断走的是大小判断，json小于的判断的数字则触发成功
{{< /callout >}}

### 示例
```json lines {linenos=table,filename="json"}
{ "ios:time": 50 }

```