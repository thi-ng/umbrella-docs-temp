<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/malloc](./malloc.md) &gt; [MemPool](./malloc.mempool.md)

## MemPool class

<b>Signature:</b>

```typescript
export declare class MemPool implements IMemPool 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(opts)](./malloc.mempool._constructor_.md) |  | Constructs a new instance of the <code>MemPool</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [\_free](./malloc.mempool._free.md) |  | <code>number</code> |  |
|  [\_used](./malloc.mempool._used.md) |  | <code>number</code> |  |
|  [align](./malloc.mempool.align.md) |  | <code>Pow2</code> |  |
|  [buf](./malloc.mempool.buf.md) |  | <code>ArrayBufferLike</code> |  |
|  [doCompact](./malloc.mempool.docompact.md) |  | <code>boolean</code> |  |
|  [doSplit](./malloc.mempool.dosplit.md) |  | <code>boolean</code> |  |
|  [end](./malloc.mempool.end.md) |  | <code>number</code> |  |
|  [minSplit](./malloc.mempool.minsplit.md) |  | <code>number</code> |  |
|  [start](./malloc.mempool.start.md) |  | <code>number</code> |  |
|  [state](./malloc.mempool.state.md) |  | <code>Uint32Array</code> |  |
|  [top](./malloc.mempool.top.md) |  | <code>number</code> |  |
|  [u32](./malloc.mempool.u32.md) |  | <code>Uint32Array</code> |  |
|  [u8](./malloc.mempool.u8.md) |  | <code>Uint8Array</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [blockNext(block)](./malloc.mempool.blocknext.md) |  |  |
|  [blockSize(block)](./malloc.mempool.blocksize.md) |  |  |
|  [calloc(bytes, fill)](./malloc.mempool.calloc.md) |  |  |
|  [callocAs(type, num, fill)](./malloc.mempool.callocas.md) |  |  |
|  [compact()](./malloc.mempool.compact.md) |  | Traverses free list and attempts to recursively merge blocks occupying consecutive memory regions. Returns true if any blocks have been merged. Only called if <code>compact</code> option is enabled. |
|  [free(ptrOrArray)](./malloc.mempool.free.md) |  |  |
|  [freeAll()](./malloc.mempool.freeall.md) |  |  |
|  [initBlock(block, size, next)](./malloc.mempool.initblock.md) |  | Initializes block header with given <code>size</code> and <code>next</code> pointer. Returns <code>block</code>. |
|  [initialTop(\_align)](./malloc.mempool.initialtop.md) |  |  |
|  [insert(block)](./malloc.mempool.insert.md) |  | Inserts given block into list of free blocks, sorted by address. |
|  [malloc(bytes)](./malloc.mempool.malloc.md) |  |  |
|  [mallocAs(type, num)](./malloc.mempool.mallocas.md) |  |  |
|  [realloc(ptr, bytes)](./malloc.mempool.realloc.md) |  |  |
|  [reallocArray(array, num)](./malloc.mempool.reallocarray.md) |  |  |
|  [release()](./malloc.mempool.release.md) |  |  |
|  [setBlockNext(block, next)](./malloc.mempool.setblocknext.md) |  | Sets block next pointer to <code>next</code>. Use zero to indicate list end. |
|  [setBlockSize(block, size)](./malloc.mempool.setblocksize.md) |  | Sets &amp; returns given block size. |
|  [splitBlock(block, blockSize, excess)](./malloc.mempool.splitblock.md) |  |  |
|  [stats()](./malloc.mempool.stats.md) |  |  |
|  [unlinkBlock(prev, block)](./malloc.mempool.unlinkblock.md) |  |  |
