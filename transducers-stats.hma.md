<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers-stats](./transducers-stats.md) &gt; [hma](./transducers-stats.hma.md)

## hma() function

[https://www.fidelity.com/learning-center/trading-investing/technical-analysis/technical-indicator-guide/hull-moving-average](https://www.fidelity.com/learning-center/trading-investing/technical-analysis/technical-indicator-guide/hull-moving-average)

Note: the number of results will be `period + floor(sqrt(period)) - 2` less than the number of processed inputs.

<b>Signature:</b>

```typescript
export declare function hma(period: number): Transducer<number, any>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  period | <code>number</code> |  |

<b>Returns:</b>

`Transducer<number, any>`

