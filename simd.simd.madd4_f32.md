<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/simd](./simd.md) &gt; [SIMD](./simd.simd.md) &gt; [madd4\_f32](./simd.simd.madd4_f32.md)

## SIMD.madd4\_f32() method

Takes three vec4 buffers, computes componentwise `a * b + c` and stores results in `out`<!-- -->. Both AOS / SOA layouts are supported, as long as all buffers are using the same layout.

All strides must by multiples of 4. All pointers should be aligned to multiples of 16. Returns `out` pointer.

<b>Signature:</b>

```typescript
madd4_f32(out: number, a: number, b: number, c: number, num: number, so: number, sa: number, sb: number, sc: number): number;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  out | <code>number</code> |  |
|  a | <code>number</code> |  |
|  b | <code>number</code> |  |
|  c | <code>number</code> |  |
|  num | <code>number</code> | number of vec4 |
|  so | <code>number</code> | out element stride |
|  sa | <code>number</code> | A element stride |
|  sb | <code>number</code> | B element stride |
|  sc | <code>number</code> | C element stride |

<b>Returns:</b>

`number`
