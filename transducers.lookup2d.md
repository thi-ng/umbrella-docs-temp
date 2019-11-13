<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [lookup2d](./transducers.lookup2d.md)

## lookup2d variable

Returns function accepting a single `[x, y]` index tuple, used to lookup value in given array. Useful for transducers processing 2D data. \*\*Note\*\*: The source data MUST be in row major linearized format, i.e. 1D representation of 2D data (pixel buffer). No bounds checks are done.

```
[...map(lookup2d([...range(9)], 3), range2d(2, -1, 0, 3))]
// [ 2, 1, 0, 5, 4, 3, 8, 7, 6 ]

```

<b>Signature:</b>

```typescript
lookup2d: <T>(src: T[], width: number) => (i: number[]) => T
```