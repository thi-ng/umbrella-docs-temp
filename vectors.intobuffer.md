<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/vectors](./vectors.md) &gt; [intoBuffer](./vectors.intobuffer.md)

## intoBuffer variable

Writes given `src` vector values into mapped `ArrayBuffer` of stated `type` and from given offset &amp; stride/spacing.

 mapBuffer

<b>Signature:</b>

```typescript
intoBuffer: <T extends Type>(type: T, buf: ArrayBuffer | SharedArrayBuffer, src: Iterable<import("@thi.ng/api").ArrayLikeIterable<number>>, byteOffset: number, byteStride: number) => void
```