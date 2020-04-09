<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/random](./random.md) &gt; [randomBytes](./random.randombytes.md)

## randomBytes variable

Fills given byte array with random values. Wrapper for `crypto.getRandomValues()` with automatic fallback to using `Math.random` if platform doesn't provide global crypto instance.

<b>Signature:</b>

```typescript
randomBytes: (buf: Uint8Array) => Uint8Array
```