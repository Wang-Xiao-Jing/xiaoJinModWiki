---
title: "api接口"
cascade:
  type: docs
weight: 2
---

## 注册predicates

{{< tabs items="forge/neoForge,fabric" >}}

{{< tab >}}
```java {linenos=table,filename="java"}

@SubscribeEvent
public static void registerPredicates(ItemOverridePredicateEvent.NewOverridePredicate event) {
	event.registerIosPredicate("stacking", ItemStackConditionChecker::stacking);
	event.registerIosPredicate("damage", ItemStackConditionChecker::damage);
	event.registerIosPredicate("nbt", NBTConditionChecker::nbt);
	event.registerIosPredicate("include_nbt", NBTConditionChecker::includeNbt);
	event.registerIosPredicate("components", NBTConditionChecker::components);
	event.registerIosPredicate("include_components", NBTConditionChecker::includeComponents);
	event.registerIosPredicate("enchantment", EnchantmentConditionChecker::enchantment);
	event.registerIosPredicate("include_enchantment", EnchantmentConditionChecker::includeEnchantment);
	event.registerIosPredicate("name", ItemStackConditionChecker::name);
	event.registerIosPredicate("day", WorldConditionChecker::day);
	event.registerIosPredicate("time", WorldConditionChecker::time);
}

// 请按照当前的版本选择格式

// 目前1.21.1的
@FunctionalInterface
public interface Predicate {
	boolean test(BakedModel model, ItemStack stack, @Nullable ClientLevel level, @Nullable LivingEntity livingEntity, JsonElement json, int seed);
}

// 目前1.12.2的
@FunctionalInterface
public interface Predicate {
	boolean test(ResourceLocation modelRL, ItemStack stack, @Nullable World worldIn, @Nullable EntityLivingBase livingEntity, JsonElement json);
}
```
{{< /tab >}}

{{< tab >}}
```java {linenos=table,filename="java"}

// 记得调用
// 要在资源包初始化之前调用
public static void registerPredicates() {
	ItemOverridePredicateEvent.NewOverridePredicate.EVENT.register(event1 -> {
		event1.registerIosPredicate("stacking", ItemStackConditionChecker::stacking);
		event1.registerIosPredicate("damage", ItemStackConditionChecker::damage);
		event1.registerIosPredicate("nbt", NBTConditionChecker::nbt);
		event1.registerIosPredicate("include_nbt", NBTConditionChecker::includeNbt);
		event1.registerIosPredicate("components", NBTConditionChecker::components);
		event1.registerIosPredicate("include_components", NBTConditionChecker::includeComponents);
		event1.registerIosPredicate("enchantment", EnchantmentConditionChecker::enchantment);
		event1.registerIosPredicate("include_enchantment", EnchantmentConditionChecker::includeEnchantment);
		event1.registerIosPredicate("name", ItemStackConditionChecker::name);
		event1.registerIosPredicate("day", WorldConditionChecker::day);
		event1.registerIosPredicate("time", WorldConditionChecker::time);
	});
}
```
{{< /tab >}}

{{< /tabs >}}