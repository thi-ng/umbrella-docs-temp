<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/dsp](./dsp.md) &gt; [osc](./dsp.osc.md)

## osc variable

Higher order oscillator gen, wrapping a [StatelessOscillator](./dsp.statelessoscillator.md) function and supporting either constant or [IGen](./dsp.igen.md)<!-- -->-based frequency and amplitude, thus allowing for FM/AM modulation. Furthermore, a constant `dc` offset (center value) can be specified (default: 0).

<b>Signature:</b>

```typescript
osc: (osc: StatelessOscillator, freq: number | IGen<number>, amp?: number | IGen<number> | undefined, dc?: number | undefined) => Osc
```

## Remarks

If `freq` is a number, it must be given as normalized frequency. If `freq` is an `IGen`<!-- -->, it must be configured to produce normalized frequency values (e.g. if using an `Osc` by setting its `amp` to a normalized freq and its `dc` offset to `baseFreq * TAU`<!-- -->). Also see  for syntax sugar.

The oscillator initializes to zero and its [IDeref.deref()](./api.ideref.deref.md) value is only available / valid after the first invocation of [IGen.next()](./dsp.igen.next.md)<!-- -->.

