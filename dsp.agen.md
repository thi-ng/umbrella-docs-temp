<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/dsp](./dsp.md) &gt; [AGen](./dsp.agen.md)

## AGen class

Abstract base class for unit gens in this package. Provides [IDeref](./api.ideref.md) to obtain the gen's current value and `Iterable` implementations to use gens as ES6 iterables.

<b>Signature:</b>

```typescript
export declare abstract class AGen<T> implements IGen<T> 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(\_val)](./dsp.agen._constructor_.md) |  | Constructs a new instance of the <code>AGen</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [\_val](./dsp.agen._val.md) |  | <code>T</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [\[Symbol.iterator\]()](./dsp.agen._symbol.iterator_.md) |  |  |
|  [deref()](./dsp.agen.deref.md) |  |  |
|  [next()](./dsp.agen.next.md) |  |  |
|  [take(num, out, idx)](./dsp.agen.take.md) |  |  |

