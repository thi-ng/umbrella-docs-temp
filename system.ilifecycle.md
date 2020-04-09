<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/system](./system.md) &gt; [ILifecycle](./system.ilifecycle.md)

## ILifecycle interface

<b>Signature:</b>

```typescript
export interface ILifecycle 
```

## Methods

|  Method | Description |
|  --- | --- |
|  [start()](./system.ilifecycle.start.md) | Starts component. Defined as async method to simplify internal use of <code>await</code> for starting any child/sub-components. Usually called by [System.start()](./system.system.start.md) which synchronously starts all of its components in dependency order.<!-- -->Returns false to indicate component startup failed and to cancel initialization of dependent components. Alternatively, an error can be thrown, but it's the user's responsibility to catch it. |
|  [stop()](./system.ilifecycle.stop.md) | Similar to [ILifecycle.start()](./system.ilifecycle.start.md) but for stopping components.<!-- -->Returns false to indicate component startup failed and log a warning message to the console. Unlike with <code>start()</code>, returning false will NOT stop decommision other components. |
