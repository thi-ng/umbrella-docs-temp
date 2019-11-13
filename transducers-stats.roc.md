<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers-stats](./transducers-stats.md) &gt; [roc](./transducers-stats.roc.md)

## roc() function

Rate of change.

[https://en.wikipedia.org/wiki/Momentum\_(technical\_analysis)](https://en.wikipedia.org/wiki/Momentum_(technical_analysis))

Note: the number of results will be `period` less than the number of processed inputs and no outputs will be produced if there were less than `period` input values.

<b>Signature:</b>

```typescript
export declare function roc(period: number): Transducer<number, number>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  period | <code>number</code> |  |

<b>Returns:</b>

`Transducer<number, number>`
