---
title: "使用方式"
cascade:
  type: docs
weight: 1
---

## 应用版本
{{< tabs items="1.21.4-24w45a以前,1.21.4-24w45a以后" >}}

{{< tab >}}
可参考[物品覆写](https://zh.minecraft.wiki/w/%E6%A8%A1%E5%9E%8B/%E6%A8%A1%E5%9E%8B%E8%A6%86%E5%86%99)
```json lines {linenos=table,filename="json"}
{
	"overrides": [
		{
			"predicate": {
                // 注意一定要在前面加上 ios: 否则无法识别
				"ios:覆写条件": "值"
			},
			"model": "模型路径"
		}
	]
}
```
{{< /tab >}}

{{< tab >}}

{{< /tab >}}

{{< /tabs >}}

## 注册新谓词 predicate
[api 接口](../api)