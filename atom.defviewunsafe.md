<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/atom](./atom.md) &gt; [defViewUnsafe](./atom.defviewunsafe.md)

## defViewUnsafe() function

<b>Signature:</b>

```typescript
export declare function defViewUnsafe<T = undefined>(parent: ReadonlyAtom<any>, path: Path, tx?: Fn<any, T>, lazy?: boolean, equiv?: Predicate2<any>): View<T extends undefined ? any : T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  parent | <code>ReadonlyAtom&lt;any&gt;</code> |  |
|  path | <code>Path</code> |  |
|  tx | <code>Fn&lt;any, T&gt;</code> |  |
|  lazy | <code>boolean</code> |  |
|  equiv | <code>Predicate2&lt;any&gt;</code> |  |

<b>Returns:</b>

`View<T extends undefined ? any : T>`

