<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [TweenOpts](./transducers.tweenopts.md)

## TweenOpts interface

<b>Signature:</b>

```typescript
export interface TweenOpts<A, B, C> 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [init](./transducers.tweenopts.init.md) | <code>Fn2&lt;A, A, B&gt;</code> | Interval producer (from 2 keyframe values, i.e. <code>stops</code>) |
|  [max](./transducers.tweenopts.max.md) | <code>number</code> | Max time boundary. Only values in the closed <code>[min..max]</code> time interval will be computed. |
|  [min](./transducers.tweenopts.min.md) | <code>number</code> | Min time boundary. Only values in the closed <code>[min..max]</code> time interval will be computed. |
|  [mix](./transducers.tweenopts.mix.md) | <code>Fn2&lt;B, number, C&gt;</code> | Interval interpolator |
|  [num](./transducers.tweenopts.num.md) | <code>number</code> | Total number (n+1) of tweened values to produce |
|  [stops](./transducers.tweenopts.stops.md) | <code>[number, A][]</code> | Keyframe definitions, i.e. <code>[time, value]</code> tuples |

