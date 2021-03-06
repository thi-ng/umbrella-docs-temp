<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/vector-pools](./vector-pools.md) &gt; [AttribPool](./vector-pools.attribpool.md)

## AttribPool class

<b>Signature:</b>

```typescript
export declare class AttribPool implements IRelease 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(opts)](./vector-pools.attribpool._constructor_.md) |  | Constructs a new instance of the <code>AttribPool</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [addr](./vector-pools.attribpool.addr.md) |  | <code>number</code> |  |
|  [attribs](./vector-pools.attribpool.attribs.md) |  | <code>IObjectOf&lt;TypedArray&gt;</code> |  |
|  [byteStride](./vector-pools.attribpool.bytestride.md) |  | <code>number</code> |  |
|  [capacity](./vector-pools.attribpool.capacity.md) |  | <code>number</code> |  |
|  [maxAttribSize](./vector-pools.attribpool.maxattribsize.md) |  | <code>number</code> |  |
|  [order](./vector-pools.attribpool.order.md) |  | <code>string[]</code> |  |
|  [pool](./vector-pools.attribpool.pool.md) |  | <code>MemPool</code> |  |
|  [resizable](./vector-pools.attribpool.resizable.md) |  | <code>boolean</code> |  |
|  [specs](./vector-pools.attribpool.specs.md) |  | <code>IObjectOf&lt;AttribSpec&gt;</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [addAttribs(specs, alloc)](./vector-pools.attribpool.addattribs.md) |  |  |
|  [attribArray(id)](./vector-pools.attribpool.attribarray.md) |  |  |
|  [attribValue(id, i)](./vector-pools.attribpool.attribvalue.md) |  |  |
|  [attribValues(id)](./vector-pools.attribpool.attribvalues.md) |  |  |
|  [bytes()](./vector-pools.attribpool.bytes.md) |  |  |
|  [computeStride(specs, inclExisting)](./vector-pools.attribpool.computestride.md) |  |  |
|  [ensure(newCapacity, fill)](./vector-pools.attribpool.ensure.md) |  |  |
|  [initDefaults(specs, start, end)](./vector-pools.attribpool.initdefaults.md) |  |  |
|  [realign(newByteStride)](./vector-pools.attribpool.realign.md) |  |  |
|  [release(releasePool)](./vector-pools.attribpool.release.md) |  |  |
|  [removeAttrib(id)](./vector-pools.attribpool.removeattrib.md) |  |  |
|  [setAttribs(specs)](./vector-pools.attribpool.setattribs.md) |  |  |
|  [setAttribValue(id, index, v)](./vector-pools.attribpool.setattribvalue.md) |  |  |
|  [setAttribValues(id, vals, index)](./vector-pools.attribpool.setattribvalues.md) |  |  |
|  [setDefaults(specs, start, end)](./vector-pools.attribpool.setdefaults.md) |  |  |
|  [updateOrder()](./vector-pools.attribpool.updateorder.md) |  |  |
|  [validateSpecs(specs, stride)](./vector-pools.attribpool.validatespecs.md) |  |  |

