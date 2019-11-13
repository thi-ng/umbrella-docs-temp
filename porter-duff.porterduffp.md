<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/porter-duff](./porter-duff.md) &gt; [porterDuffP](./porter-duff.porterduffp.md)

## porterDuffP variable

Higher order function. Takes existing PD operator and returns function which accepts same args as the operator, but pre-multiplies alpha for both input colors and then returns post-multiplied alpha output.

<b>Signature:</b>

```typescript
porterDuffP: (mode: Fn3<Color | null, import("@thi.ng/api").ArrayLikeIterable<number>, import("@thi.ng/api").ArrayLikeIterable<number>, Color>) => (out: Color, src: import("@thi.ng/api").ArrayLikeIterable<number>, dest: import("@thi.ng/api").ArrayLikeIterable<number>) => Color
```