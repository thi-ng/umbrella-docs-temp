<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/ecs](./ecs.md) &gt; [LRU](./ecs.lru.md)

## LRU class

<b>Signature:</b>

```typescript
export declare class LRU<T> implements ICache<T> 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(cap)](./ecs.lru._constructor_.md) |  | Constructs a new instance of the <code>LRU</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [capacity](./ecs.lru.capacity.md) |  | <code>number</code> |  |
|  [index](./ecs.lru.index.md) |  | <code>Map&lt;number, ConsCell&lt;LRUEntry&lt;T&gt;&gt;&gt;</code> |  |
|  [items](./ecs.lru.items.md) |  | <code>DCons&lt;LRUEntry&lt;T&gt;&gt;</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [delete(key)](./ecs.lru.delete.md) |  |  |
|  [get(key)](./ecs.lru.get.md) |  |  |
|  [getSet(key, notFound)](./ecs.lru.getset.md) |  |  |
|  [keys()](./ecs.lru.keys.md) |  |  |
|  [release()](./ecs.lru.release.md) |  |  |
|  [set(key, val)](./ecs.lru.set.md) |  |  |
