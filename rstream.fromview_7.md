<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [fromView](./rstream.fromview_7.md)

## fromView() function

<b>Signature:</b>

```typescript
export declare function fromView<T, A, B, C, D, E, F, G, R = undefined>(parent: ReadonlyAtom<T>, opts: FromViewOpts<Path7<T, A, B, C, D, E, F, G>, OptPathVal<T, [A, B, C, D, E, F, G]>, R>): Stream<R extends undefined ? OptPathVal<T, [A, B, C, D, E, F, G]> : R>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  parent | <code>ReadonlyAtom&lt;T&gt;</code> |  |
|  opts | <code>FromViewOpts&lt;Path7&lt;T, A, B, C, D, E, F, G&gt;, OptPathVal&lt;T, [A, B, C, D, E, F, G]&gt;, R&gt;</code> |  |

<b>Returns:</b>

`Stream<R extends undefined ? OptPathVal<T, [A, B, C, D, E, F, G]> : R>`
