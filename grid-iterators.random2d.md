<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/grid-iterators](./grid-iterators.md) &gt; [random2d](./grid-iterators.random2d.md)

## random2d() function

Yields 2D grid coordinates in random order w/ support for optional `IRandom` implementation (default: [SYSTEM](./random.system.md) aka `Math.random`<!-- -->).

<b>Signature:</b>

```typescript
export declare function random2d(cols: number, rows?: number, rnd?: IRandom): Generator<number[], void, unknown>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  cols | <code>number</code> |  |
|  rows | <code>number</code> |  |
|  rnd | <code>IRandom</code> |  |

<b>Returns:</b>

`Generator<number[], void, unknown>`
