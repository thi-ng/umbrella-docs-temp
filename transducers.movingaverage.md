<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [movingAverage](./transducers.movingaverage.md)

## movingAverage() function

Computes the Simple Moving Average of given period. [https://en.wikipedia.org/wiki/Moving\_average\#Simple\_moving\_average](https://en.wikipedia.org/wiki/Moving_average#Simple_moving_average)

Note: the number of results will be `period-1` less than the number of processed inputs and no outputs will be produced if there were less than `period` input values.

Also see the  package for more optimized and alternative MAs.

<b>Signature:</b>

```typescript
export declare function movingAverage(period: number): Transducer<number, number>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  period | <code>number</code> |  |

<b>Returns:</b>

`Transducer<number, number>`
