<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/atom](./atom.md) &gt; [defView](./atom.defview_9.md)

## defView() function

<b>Signature:</b>

```typescript
export declare function defView<T, A, B, C, D, E, F, G, H, R = undefined>(parent: ReadonlyAtom<T>, path: DeepPath<T, A, B, C, D, E, F, G, H>, tx?: Fn<any, R>, lazy?: boolean, equiv?: Predicate2<any>): View<R extends undefined ? any : R>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  parent | <code>ReadonlyAtom&lt;T&gt;</code> |  |
|  path | <code>DeepPath&lt;T, A, B, C, D, E, F, G, H&gt;</code> |  |
|  tx | <code>Fn&lt;any, R&gt;</code> |  |
|  lazy | <code>boolean</code> |  |
|  equiv | <code>Predicate2&lt;any&gt;</code> |  |

<b>Returns:</b>

`View<R extends undefined ? any : R>`

