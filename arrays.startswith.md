<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/arrays](./arrays.md) &gt; [startsWith](./arrays.startswith.md)

## startsWith variable

Returns true if the first items of `buf` are the same items as in `needle`<!-- -->. This means `buf` should have at least the same length as `needle` for this to be true.

By default, uses [equiv](./equiv.equiv.md) for equality checking.

 endsWith

<b>Signature:</b>

```typescript
startsWith: (buf: ArrayLike<any>, needle: ArrayLike<any>, equiv?: (a: any, b: any) => boolean) => boolean
```