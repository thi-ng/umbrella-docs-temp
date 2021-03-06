<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream-graph](./rstream-graph.md)

## rstream-graph package

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [Node](./rstream-graph.node.md) |  |
|  [NodeInputSpec](./rstream-graph.nodeinputspec.md) | Specification for a single input, which can be given in different ways:<!-- -->1) Create a stream for given path in state atom (passed to [initGraph](./rstream-graph.initgraph.md)<!-- -->):
```
{ path: "nested.src.path" }
{ path: ["nested", "src", "path"] }

```
2) Reference path to another node's output in the GraphSpec object. See [@thi.ng/resolve-map](./resolve-map.md) for details.
```
{ stream: "/node-id/node" } // main node output
{ stream: "/node-id/outs/foo" } // specific output

```
3) Reference another node indirectly. The passed in <code>resolve</code> function can be used to lookup other nodes, with the same logic as above. E.g. the following spec looks up the main output of node "abc" and adds a transformed subscription, which is then used as input for current node.
```
{ stream: (resolve) =>
    resolve("/abc/node").subscribe(map(x => x * 10)) }

```
4) Provide an external input stream:
```
{ stream: () => fromIterable([1,2,3], 500) }

```
5) Single value input stream:
```
{ const: 1 }
{ const: () => 1 }

```
If the optional <code>xform</code> is given, a subscription with the given transducer is added to the input and then used as input instead. |
|  [NodeSpec](./rstream-graph.nodespec.md) | Specification for a single "node" in the dataflow graph. Nodes here are actually just wrappers of streams / subscriptions (or generally any form of [ISubscribable](./rstream.isubscribable.md)<!-- -->), usually with an associated transducer to transform / combine the inputs and produce values for the node's result stream.<!-- -->The <code>fn</code> function is responsible to produce such a stream transformer construct. The keys used to specify inputs in the <code>ins</code> object are dictated by the actual node <code>fn</code> used. Most node functions with multiple inputs will be implemented as [StreamSync](./rstream.streamsync.md) instances and the input IDs are used to locally rename input streams within the [StreamSync](./rstream.streamsync.md) container.<!-- -->Alo see [initGraph](./rstream-graph.initgraph.md) and  (in /src/nodes.ts) for more details how these specs are compiled into stream constructs. |

## Variables

|  Variable | Description |
|  --- | --- |
|  [add](./rstream-graph.add.md) | Addition node.<!-- -->Inputs: any |
|  [addNode](./rstream-graph.addnode.md) | Compiles given [NodeSpec](./rstream-graph.nodespec.md) and adds it to graph. Returns compiled [Node](./rstream-graph.node.md) object for the given spec. Throws error if the graph already contains a node with given <code>id</code>. |
|  [div](./rstream-graph.div.md) | Division node.<!-- -->Inputs: <code>a</code>, <code>b</code> |
|  [ensureInputs](./rstream-graph.ensureinputs.md) | Helper function to verify given object of inputs has required input IDs. Throws error if validation fails. |
|  [extract](./rstream-graph.extract.md) | Nested value extraction node. Higher order function.<!-- -->Inputs: 1 |
|  [initGraph](./rstream-graph.initgraph.md) | Dataflow graph initialization function. Takes a state Atom (or <code>null</code> if not needed) and an object of [NodeSpec](./rstream-graph.nodespec.md) values or functions returning [Node](./rstream-graph.node.md) objects. Calls <code>nodeFromSpec()</code> for each spec and then recursively resolves references via [resolve](./resolve-map.resolve.md)<!-- -->. Returns new initialized graph object of [Node](./rstream-graph.node.md) objects and [@thi.ng/rstream](./rstream.md) stream constructs. Does NOT mutate original [GraphSpec](./rstream-graph.graphspec.md) object. |
|  [mul](./rstream-graph.mul.md) | Multiplication node.<!-- -->Inputs: any |
|  [node](./rstream-graph.node.md) | Higher order node / stream creator. Takes a transducer and (optional) required input stream IDs. The returned function takes an object of input streams and returns a new [StreamSync](./rstream.streamsync.md) instance. The returned function will throw an error if <code>inputIDs</code> is given and the object of inputs does not contain all of them.<!-- -->If <code>reset</code> is true (default: false), the <code>xform</code> will only re-run when all inputs have produced new values. See [StreamSync](./rstream.streamsync.md) for further reference.<!-- -->// TODO add close behavior opts |
|  [node1](./rstream-graph.node1.md) | Similar to [node](./rstream-graph.node.md)<!-- -->, but optimized for nodes using only a single input. Uses "src" as default input ID.<!-- -->// TODO add close behavior opts |
|  [node2](./rstream-graph.node2.md) | Syntax sugar for <code>node()</code>, intended for nodes w/ 2 inputs, by default named <code>a</code> &amp; <code>b</code> (but can be overridden). |
|  [removeNode](./rstream-graph.removenode.md) | Calls <code>.unsubscribe()</code> on given node and all of its outputs, then removes it from graph. Returns <code>false</code> if no node exists for given <code>id</code>. |
|  [stop](./rstream-graph.stop.md) | Calls <code>.unsubscribe()</code> on all nodes in the graph, causing all related streams &amp; subscriptions to terminate. |
|  [sub](./rstream-graph.sub.md) | Subtraction node.<!-- -->Inputs: <code>a</code>, <code>b</code> |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [Graph](./rstream-graph.graph.md) |  |
|  [GraphSpec](./rstream-graph.graphspec.md) | A dataflow graph spec is simply an object where keys are node names and their values are [NodeSpec](./rstream-graph.nodespec.md)<!-- -->s, defining a node's inputs, outputs and the operation to be applied to produce one or more result streams. |
|  [NodeFactory](./rstream-graph.nodefactory.md) | A function which constructs and returns an [ISubscribable](./rstream.isubscribable.md) using given object of inputs and node ID. See <code>node()</code> and <code>node1()</code>. |
|  [NodeInputs](./rstream-graph.nodeinputs.md) |  |
|  [NodeOutputFn](./rstream-graph.nodeoutputfn.md) |  |
|  [NodeOutputs](./rstream-graph.nodeoutputs.md) |  |
|  [NodeOutputSpec](./rstream-graph.nodeoutputspec.md) |  |
|  [NodeResolver](./rstream-graph.noderesolver.md) |  |

