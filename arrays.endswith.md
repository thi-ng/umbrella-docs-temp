<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/arrays](./arrays.md) &gt; [endsWith](./arrays.endswith.md)

## endsWith variable

Returns true if the last items of `buf` are the same items as in `needle`<!-- -->.

<b>Signature:</b>

```typescript
endsWith: <T>(buf: ArrayLike<T>, needle: ArrayLike<T>, equiv?: (a: any, b: any) => boolean) => boolean
```

## Remarks

This means `buf` should have at least the same length as `needle` for this to be true.

By default, uses [equiv](./equiv.equiv.md) for equality checking.

[startsWith](./arrays.startswith.md)

