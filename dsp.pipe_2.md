<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/dsp](./dsp.md) &gt; [pipe](./dsp.pipe_2.md)

## pipe() function

<b>Signature:</b>

```typescript
export declare function pipe<A, B, C, D>(src: IGen<A>, a: IProc<A, B>, b: IProc<B, C>, c: IProc<C, D>): IGen<D>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  src | <code>IGen&lt;A&gt;</code> |  |
|  a | <code>IProc&lt;A, B&gt;</code> |  |
|  b | <code>IProc&lt;B, C&gt;</code> |  |
|  c | <code>IProc&lt;C, D&gt;</code> |  |

<b>Returns:</b>

`IGen<D>`
