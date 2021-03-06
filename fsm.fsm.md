<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/fsm](./fsm.md) &gt; [fsm](./fsm.fsm.md)

## fsm() function

Finite-state machine transducer / iterator with support for single lookahead value.

<b>Signature:</b>

```typescript
export declare function fsm<T, C, R>(states: IObjectOf<Matcher<T, C, R>>, ctx: C, initial: string | number, update?: Fn2<C, T, void>): Transducer<T, R>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  states | <code>IObjectOf&lt;Matcher&lt;T, C, R&gt;&gt;</code> | FSM state matchers |
|  ctx | <code>C</code> | FSM context object |
|  initial | <code>string &#124; number</code> |  |
|  update | <code>Fn2&lt;C, T, void&gt;</code> | context update fn |

<b>Returns:</b>

`Transducer<T, R>`

## Remarks

Takes an object of `states` and their matchers, an arbitrary context object and an `initial` state ID (default: "start").

The returned transducer consumes inputs of type `T` and produces results of type `R`<!-- -->. The results are produced by callbacks of the given state matchers. Each can produce any number of values. If a callback returns a result wrapped w/ , the FSM causes early termination of the overall transducer pipeline. Failed state callbacks too can produce outputs, but will afterwards terminate the FSM.

An [IllegalStateError](./errors.illegalstateerror.md) will be thrown if a transition to an undefined state ID occurs.

The optional `update` function will be invoked for each input prior to executing the currently active state matcher. It is intended to update the context object (e.g. to update input location info for generating error messages).

If the optional `src` iterable is given, the function returns a transforming iterator of the FSM results.

