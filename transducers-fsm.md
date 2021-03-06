<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers-fsm](./transducers-fsm.md)

## transducers-fsm package

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [FSMOpts](./transducers-fsm.fsmopts.md) |  |
|  [FSMState](./transducers-fsm.fsmstate.md) |  |

## Variables

|  Variable | Description |
|  --- | --- |
|  [fsm](./transducers-fsm.fsm.md) | Finite State Machine transducer. Takes an FSM configuration object and returns a transducer, which processes inputs using the provided state handler functions, which in turn can return any number of outputs per consumed input.<!-- -->Before processing the first input, the FSM state is initialized by calling the user provided <code>init()</code> function, which MUST return a state object with at least a <code>state</code> key, whose value is used for dynamic (i.e. stateful) dispatch during input processing. This state object is passed with each input value to the current state handler, which is expected to mutate this object, e.g. to cause state changes based on given inputs.<!-- -->If a state handler needs to "emit" results for downstream processing, it can return an array of values. Any such values are passed on (individually, not as array) to the next reducer in the chain. If a state handler returns <code>null</code> or <code>undefined</code>, further downstream processing of the current input is skipped.<!-- -->Regardless of return value, if a state handler has caused a state change to the configured <code>terminal</code> state, processing is terminated (by calling [ensureReduced](./transducers.ensurereduced.md)<!-- -->) and no further inputs will be consumed. |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [FSMHandler](./transducers-fsm.fsmhandler.md) |  |
|  [FSMStateMap](./transducers-fsm.fsmstatemap.md) |  |

