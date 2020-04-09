<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/system](./system.md) &gt; [System](./system.system.md)

## System class

<b>Signature:</b>

```typescript
export declare class System<T extends SystemMap<T>> implements ILifecycle 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(map)](./system.system._constructor_.md) |  | Constructs a new instance of the <code>System</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [components](./system.system.components.md) |  | <code>T</code> |  |
|  [graph](./system.system.graph.md) |  | <code>DGraph&lt;Keys&lt;T&gt;&gt;</code> |  |
|  [topology](./system.system.topology.md) |  | <code>Keys&lt;T&gt;[]</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [reset()](./system.system.reset.md) |  | Syntax sugar for <code>stop() &amp;&amp; start()</code> sequence. |
|  [start()](./system.system.start.md) |  | Initializes all system components in dependency order. If any component's <code>start()</code> method returns false, system start up will be stopped and this method returns false itself.<!-- -->Also any errors thrown during child component startup will not be intercepted. |
|  [stop()](./system.system.stop.md) |  | Stops all system components in reverse dependency order. If any component's <code>stop()</code> method returns false, a warning message will be logged, but unlike [System.start()](./system.system.start.md)<!-- -->, the shutdown process of other components will not be stopped.<!-- -->Any errors thrown during child component shutdown will not be intercepted. |
