<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/hdom](./hdom.md) &gt; [HDOMImplementation](./hdom.hdomimplementation.md) &gt; [hydrateTree](./hdom.hdomimplementation.hydratetree.md)

## HDOMImplementation.hydrateTree() method

Takes a target root element and normalized hdom tree, then walks tree and initializes any event listeners and components with life cycle `init` methods. Assumes that an equivalent "DOM" (minus listeners) already exists when this function is called. Any other discrepancies between the pre-existing DOM and the hdom tree might cause undefined behavior.

Implementations MUST check for the presence of the `__impl` control attribute on each branch. If given, the current implementation MUST delegate to the `hydrateTree()` method of the specified implementation and not descent into that branch further itself.

<b>Signature:</b>

```typescript
hydrateTree(opts: Partial<HDOMOpts>, parent: T, tree: any, child?: number): void;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  opts | <code>Partial&lt;HDOMOpts&gt;</code> |  |
|  parent | <code>T</code> |  |
|  tree | <code>any</code> |  |
|  child | <code>number</code> |  |

<b>Returns:</b>

`void`
