<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/dsp](./dsp.md) &gt; [filterResponseRaw](./dsp.filterresponseraw.md)

## filterResponseRaw variable

Returns filter response for given filter coefficients at normalized frequency `f`<!-- -->. If `db` is true (default), the magnitude in the returned object will be in dBFS.

References:

- https://www.earlevel.com/main/2016/12/01/evaluating-filter-frequency-response/ - https://www.earlevel.com/main/2016/12/08/filter-frequency-response-grapher/ - https://github.com/mohayonao/freqr

<b>Signature:</b>

```typescript
filterResponseRaw: (zeroes: NumericArray, poles: NumericArray, freq: number, db?: boolean) => FilterResponse
```