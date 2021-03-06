<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [tween](./rstream.tween.md)

## tween variable

Takes an existing stream/subscription `src` and attaches new subscription which interpolates between incoming values from `src` using the given `mix` function.

<b>Signature:</b>

```typescript
tween: <T>(src: ISubscribable<T>, initial: T, mix: Fn2<T, T, T>, stop?: Fn2<T, T, boolean> | undefined, clock?: number | ISubscribable<any> | undefined) => import("./subscription").Subscription<{
    src: T;
}, T>
```

## Remarks

The returned construct produces values at a rate controlled by the `clock` stream or frequency. If omitted, `clock` defaults to [fromRAF](./rstream.fromraf.md) (\~60Hz). If the `clock` is given as number, creates a [fromInterval](./rstream.frominterval.md) or else uses the given `clock` stream directly. In general, the frequency of the `clock` should always be higher than that of `src` or else interpolation will have undefined behavior.

If `stop` is given as well, no values will be passed downstream if that function returns true. This can be used to limit traffic once the tween target value has been reached.

The returned subscription closes automatically when either `src` or `clock` are exhausted.

## Example


```ts
val = stream();

tween(
  // consume from `val` stream
  val,
  // initial start value to interpolate from
  0,
  // interpolation fn (LERP)
  (a, b) => a + (b - a) * 0.5,
  // stop emitting values if difference to previous result < 0.01
  (a, b) => Math.abs(a - b) < 0.01
).subscribe(trace("tweened"))

a.next(10)
// 5
// 7.5
// ...
// 9.98046875

a.next(100)
// 55
// 77.5
// ...
// 99.989013671875

```

