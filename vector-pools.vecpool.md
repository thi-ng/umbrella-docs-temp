<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/vector-pools](./vector-pools.md) &gt; [VecPool](./vector-pools.vecpool.md)

## VecPool class

<b>Signature:</b>

```typescript
export declare class VecPool implements IVecPool 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(pool)](./vector-pools.vecpool._constructor_.md) |  | Constructs a new instance of the <code>VecPool</code> class |
|  [(constructor)(opts)](./vector-pools.vecpool._constructor__1.md) |  | Constructs a new instance of the <code>VecPool</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [pool](./vector-pools.vecpool.pool.md) |  | <code>MemPool</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [free(vec)](./vector-pools.vecpool.free.md) |  |  |
|  [freeAll()](./vector-pools.vecpool.freeall.md) |  |  |
|  [malloc(size, type)](./vector-pools.vecpool.malloc.md) |  |  |
|  [mallocArray(num, size, cstride, estride, type)](./vector-pools.vecpool.mallocarray.md) |  | Intended to provide individual vector views of a larger underlying buffer. Attempts to allocate a single block of sufficient memory to hold <code>num</code> vectors of <code>size</code> elements and if successful returns array of vectors mapping the buffer with given stride lengths (both component and element strides can be provided).<!-- -->\*Note:\* Since all result vectors share the same continuous memory block, freeing any of them from the pool will invalidate all of them.<!-- -->Also see: - <code>Vec2.mapBuffer()</code> - <code>Vec3.mapBuffer()</code> - <code>Vec4.mapBuffer()</code> - <code>NDArray1.mapBuffer()</code> |
|  [mallocWrapped(size, stride, type)](./vector-pools.vecpool.mallocwrapped.md) |  |  |
|  [release()](./vector-pools.vecpool.release.md) |  |  |
|  [stats()](./vector-pools.vecpool.stats.md) |  |  |
