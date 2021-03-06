<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/interceptors](./interceptors.md)

## interceptors package

## Classes

|  Class | Description |
|  --- | --- |
|  [EventBus](./interceptors.eventbus.md) | Stateful version of [StatelessEventBus](./interceptors.statelesseventbus.md)<!-- -->. |
|  [StatelessEventBus](./interceptors.statelesseventbus.md) | Batched event processor for using composable interceptors for event handling and side effects to execute the result of handled events. |

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [Event](./interceptors.event.md) |  |
|  [IDispatch](./interceptors.idispatch.md) |  |
|  [Interceptor](./interceptors.interceptor.md) |  |
|  [InterceptorContext](./interceptors.interceptorcontext.md) |  |

## Variables

|  Variable | Description |
|  --- | --- |
|  [dispatch](./interceptors.dispatch.md) | Higher-order interceptor. Returns interceptor which assigns given event to <code>FX_DISPATCH</code> side effect. |
|  [dispatchNow](./interceptors.dispatchnow.md) | Higher-order interceptor. Returns interceptor which assigns given event to <code>FX_DISPATCH_NOW</code> side effect. |
|  [ensureParamRange](./interceptors.ensureparamrange.md) | Specialization of [ensurePred](./interceptors.ensurepred.md) to ensure an event's payload value is within given <code>min</code> / <code>max</code> closed interval. By default, assumes event format like: <code>[event-id, value]</code>. However if <code>value</code> is given, the provided function can be used to extract the value to be validated from any event. If the value is outside the given interval, triggers <code>FX_CANCEL</code> side effect and if <code>err</code> is given, the error interceptor can return any number of other side effects and so be used to dispatch alternative events instead. |
|  [ensurePred](./interceptors.ensurepred.md) | Higher-order interceptor for validation purposes. Takes a predicate function and an optional interceptor function, which will only be called if the predicate fails for a given event. By default the <code>FX_CANCEL</code> side effect is triggered if the predicate failed, thus ensuring the actual event handler for the failed event will not be executed anymore. However, this can be overridden using the error interceptor's result, which is merged into the result of this interceptor.<!-- -->The error interceptor can return any number of other side effects and so be used to dispatch alternative events instead, for example:
```
// this interceptor will cause cancellation of current event
// and trigger an "error" event instead
ensurePred(
  // a dummy predicate which always fails
  () => false
  // error interceptor fn
  () => ({[FX_DISPATCH_NOW]: ["error", "reason"]})
)

```
Note: For this interceptor to work as expected, it needs to be provided BEFORE the main handler in the interceptor list for a given event, i.e.
```
[
   ensurePred((state, e) => false),
   // actual event handler
   (state, e) => console.log("no one never calls me")
]

```
 |
|  [ensureStateGreaterThan](./interceptors.ensurestategreaterthan.md) | Specialization of [ensurePred](./interceptors.ensurepred.md) to ensure a state value is greater than given min. See [ensureStateLessThan](./interceptors.ensurestatelessthan.md) for further details. |
|  [ensureStateLessThan](./interceptors.ensurestatelessthan.md) | Specialization of [ensurePred](./interceptors.ensurepred.md) to ensure a state value is less than given max at the time when the event is being processed. The optional <code>path</code> fn is used to extract or produce the path for the state value to be validated. If omitted, the event's payload item is interpreted as the value path.<!-- -->For example, without a provided <code>path</code> function and for an event of this form: <code>[&quot;event-id&quot;, &quot;foo.bar&quot;]</code>, the term <code>&quot;foo.bar&quot;</code> would be interpreted as path.<!-- -->If the event has this shape: <code>[&quot;event-id&quot;, [&quot;foo.bar&quot;, 23]]</code>, we must provide <code>(e) =&gt; e[1][0]</code> as path function to extract <code>&quot;foo.bar&quot;</code> from the event. |
|  [ensureStateRange](./interceptors.ensurestaterange.md) | Specialization of [ensurePred](./interceptors.ensurepred.md) to ensure a state value is within given <code>min</code> / <code>max</code> closed interval. See [ensureStateLessThan](./interceptors.ensurestatelessthan.md) for further details. |
|  [EV\_REDO](./interceptors.ev_redo.md) | Event ID to trigger redo action. See <code>EventBus.addBuiltIns()</code> for further details. Also see [snapshot](./interceptors.snapshot.md) interceptor docs. |
|  [EV\_SET\_VALUE](./interceptors.ev_set_value.md) |  |
|  [EV\_TOGGLE\_VALUE](./interceptors.ev_toggle_value.md) |  |
|  [EV\_UNDO](./interceptors.ev_undo.md) | Event ID to trigger undo action. See <code>EventBus.addBuiltIns()</code> for further details. Also see [snapshot](./interceptors.snapshot.md) interceptor docs. |
|  [EV\_UPDATE\_VALUE](./interceptors.ev_update_value.md) |  |
|  [forwardSideFx](./interceptors.forwardsidefx.md) | Higher-order interceptor. Returns interceptor which unpacks payload from event and assigns it as is to given side effect ID. Assigns <code>true</code> to side effect if event has no payload. |
|  [FX\_CANCEL](./interceptors.fx_cancel.md) |  |
|  [FX\_DELAY](./interceptors.fx_delay.md) |  |
|  [FX\_DISPATCH\_ASYNC](./interceptors.fx_dispatch_async.md) |  |
|  [FX\_DISPATCH\_NOW](./interceptors.fx_dispatch_now.md) |  |
|  [FX\_DISPATCH](./interceptors.fx_dispatch.md) |  |
|  [FX\_FETCH](./interceptors.fx_fetch.md) |  |
|  [FX\_STATE](./interceptors.fx_state.md) |  |
|  [LOGGER](./interceptors.logger.md) |  |
|  [setLogger](./interceptors.setlogger.md) |  |
|  [snapshot](./interceptors.snapshot.md) | Higher-order interceptor. Returns interceptor which calls <code>ctx[id].record()</code>, where <code>ctx</code> is the currently active [InterceptorContext](./interceptors.interceptorcontext.md) passed to all event handlers and <code>ctx[id]</code> is assumed to be a [History](./atom.history.md) instance, passed to [EventBus.processQueue()](./interceptors.eventbus.processqueue.md)<!-- -->. The default ID for the history instance is <code>&quot;history&quot;</code>.<!-- -->Example usage: |
|  [trace](./interceptors.trace.md) | Debug interceptor to log the current event to the console. |
|  [valueSetter](./interceptors.valuesetter.md) | Higher-order interceptor. Returns new interceptor to set state value at provided path. This allows for dedicated events to set state values more concisely, e.g. given this event definition: |
|  [valueUpdater](./interceptors.valueupdater.md) | Higher-order interceptor. Returns new interceptor to update state value at provided path with given function. This allows for dedicated events to update state values more concisely, e.g. given this event definition: |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [AsyncEffectDef](./interceptors.asynceffectdef.md) |  |
|  [EffectDef](./interceptors.effectdef.md) |  |
|  [EffectPriority](./interceptors.effectpriority.md) |  |
|  [EventDef](./interceptors.eventdef.md) |  |
|  [InterceptorFn](./interceptors.interceptorfn.md) |  |
|  [InterceptorPredicate](./interceptors.interceptorpredicate.md) |  |
|  [SideEffect](./interceptors.sideeffect.md) |  |

