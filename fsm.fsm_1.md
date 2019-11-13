<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/fsm](./fsm.md) &gt; [fsm](./fsm.fsm_1.md)

## fsm() function

<b>Signature:</b>

```typescript
export declare function fsm<T, C, R>(states: IObjectOf<Matcher<T, C, R>>, ctx: C, initial: string | number, update?: Fn2<C, T, void>, src?: Iterable<T>): IterableIterator<R>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  states | <code>IObjectOf&lt;Matcher&lt;T, C, R&gt;&gt;</code> |  |
|  ctx | <code>C</code> |  |
|  initial | <code>string &#124; number</code> |  |
|  update | <code>Fn2&lt;C, T, void&gt;</code> |  |
|  src | <code>Iterable&lt;T&gt;</code> |  |

<b>Returns:</b>

`IterableIterator<R>`
