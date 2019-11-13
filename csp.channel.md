<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/csp](./csp.md) &gt; [Channel](./csp.channel.md)

## Channel class

<b>Signature:</b>

```typescript
export declare class Channel<T> implements IReadWriteableChannel<T> 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)()](./csp.channel._constructor_.md) |  | Constructs a new instance of the <code>Channel</code> class |
|  [(constructor)(id, buf, tx, err)](./csp.channel._constructor__9.md) |  | Constructs a new instance of the <code>Channel</code> class |
|  [(constructor)(id)](./csp.channel._constructor__1.md) |  | Constructs a new instance of the <code>Channel</code> class |
|  [(constructor)(buf)](./csp.channel._constructor__2.md) |  | Constructs a new instance of the <code>Channel</code> class |
|  [(constructor)(tx)](./csp.channel._constructor__3.md) |  | Constructs a new instance of the <code>Channel</code> class |
|  [(constructor)(tx, err)](./csp.channel._constructor__4.md) |  | Constructs a new instance of the <code>Channel</code> class |
|  [(constructor)(id, buf)](./csp.channel._constructor__5.md) |  | Constructs a new instance of the <code>Channel</code> class |
|  [(constructor)(id, tx)](./csp.channel._constructor__6.md) |  | Constructs a new instance of the <code>Channel</code> class |
|  [(constructor)(id, tx, err)](./csp.channel._constructor__7.md) |  | Constructs a new instance of the <code>Channel</code> class |
|  [(constructor)(id, buf, tx)](./csp.channel._constructor__8.md) |  | Constructs a new instance of the <code>Channel</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [buf](./csp.channel.buf.md) |  | <code>IBuffer&lt;T&gt;</code> |  |
|  [id](./csp.channel.id.md) |  | <code>string</code> |  |
|  [isBusy](./csp.channel.isbusy.md) |  | <code>boolean</code> |  |
|  [MAX\_WRITES](./csp.channel.max_writes.md) | <code>static</code> | <code>number</code> |  |
|  [NEXT\_ID](./csp.channel.next_id.md) | <code>static</code> | <code>number</code> |  |
|  [onerror](./csp.channel.onerror.md) |  | <code>ErrorHandler</code> |  |
|  [reads](./csp.channel.reads.md) |  | <code>DCons&lt;(x: T) =&gt; void&gt;</code> |  |
|  [SCHEDULE](./csp.channel.schedule.md) | <code>static</code> | <code>Fn2&lt;FnAny&lt;void&gt;, number, void&gt;</code> |  |
|  [state](./csp.channel.state.md) |  | <code>State</code> |  |
|  [tx](./csp.channel.tx.md) |  | <code>Reducer&lt;DCons&lt;T&gt;, T&gt;</code> |  |
|  [txbuf](./csp.channel.txbuf.md) |  | <code>DCons&lt;T&gt;</code> |  |
|  [writes](./csp.channel.writes.md) |  | <code>DCons&lt;ChannelItem&lt;T&gt;&gt;</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [channel()](./csp.channel.channel.md) |  |  |
|  [close(flush)](./csp.channel.close.md) |  |  |
|  [concat(chans, close)](./csp.channel.concat.md) |  |  |
|  [constantly(x, delay)](./csp.channel.constantly.md) | <code>static</code> |  |
|  [consume(fn)](./csp.channel.consume.md) |  |  |
|  [consumeWhileReadable(fn)](./csp.channel.consumewhilereadable.md) |  |  |
|  [cycle(src, delay)](./csp.channel.cycle.md) | <code>static</code> |  |
|  [flush()](./csp.channel.flush.md) |  |  |
|  [from(src)](./csp.channel.from.md) | <code>static</code> |  |
|  [from(src, close)](./csp.channel.from_1.md) | <code>static</code> |  |
|  [from(src, tx)](./csp.channel.from_2.md) | <code>static</code> |  |
|  [from(src, tx, close)](./csp.channel.from_3.md) | <code>static</code> |  |
|  [fromPromise(p)](./csp.channel.frompromise.md) | <code>static</code> | Creates new channel with single value from given promise, then closes automatically iff promise has been resolved. |
|  [into(src, close)](./csp.channel.into.md) |  |  |
|  [isClosed()](./csp.channel.isclosed.md) |  |  |
|  [isReadable()](./csp.channel.isreadable.md) |  |  |
|  [merge(chans, out, close, named)](./csp.channel.merge.md) | <code>static</code> | Takes an array of channels to merge into new channel. Any closed channels will be automatically removed from the input selection. Once all inputs are closed, the target channel will close too (by default).<!-- -->If <code>named</code> is true, the merged channel will have tuples of: <code>[src-id, val]</code> If false (default), only received values will be forwarded. |
|  [mergeTuples(chans, out, closeOnFirst, closeOutput)](./csp.channel.mergetuples.md) | <code>static</code> | Takes an array of channels to merge into new channel of tuples. Whereas <code>Channel.merge()</code> realizes a sequential merging with no guarantees about ordering of the output, the output channel of this function will collect values from all channels and a new tuple is emitted only once a new value has been read from ALL channels. Therefore the overall throughput is dictated by the slowest of the inputs.<!-- -->Once any of the inputs closes, the process is terminated and the output channel is closed too (by default).
```
Channel.mergeTuples([
  Channel.from([1, 2, 3]),
  Channel.from([10, 20, 30]),
  Channel.from([100, 200, 300])
]).consume();

// chan-0 : [ 1, 10, 100 ]
// chan-0 : [ 2, 20, 200 ]
// chan-0 : [ 3, 30, 300 ]
// chan-0 done

Channel.mergeTuples([
  Channel.from([1, 2, 3]),
  Channel.from([10, 20, 30]),
  Channel.from([100, 200, 300])
], null, false).consume();

```
 |
|  [pipe(dest, close)](./csp.channel.pipe.md) |  |  |
|  [process()](./csp.channel.process.md) |  |  |
|  [produce(fn, close)](./csp.channel.produce.md) |  |  |
|  [range()](./csp.channel.range.md) | <code>static</code> |  |
|  [range(to)](./csp.channel.range_1.md) | <code>static</code> |  |
|  [range(from, to)](./csp.channel.range_2.md) | <code>static</code> |  |
|  [range(from, to, step)](./csp.channel.range_3.md) | <code>static</code> |  |
|  [range(from, to, step, delay)](./csp.channel.range_4.md) | <code>static</code> |  |
|  [read()](./csp.channel.read.md) |  |  |
|  [reduce(rfn, acc)](./csp.channel.reduce.md) |  |  |
|  [release()](./csp.channel.release.md) |  |  |
|  [repeatedly(fn, delay)](./csp.channel.repeatedly.md) | <code>static</code> |  |
|  [select(chans)](./csp.channel.select.md) | <code>static</code> | Takes an array of channels and blocks until any of them becomes readable (or has been closed). The returned promised resolves into an array of <code>[value, channel]</code>. Channel order is repeatedly shuffled for each read attempt. |
|  [sleep(delay)](./csp.channel.sleep.md) | <code>static</code> | Shorthand for: <code>Channel.timeout(delay).take()</code> |
|  [split(pred, truthy, falsey, close)](./csp.channel.split.md) |  |  |
|  [timeout(delay)](./csp.channel.timeout.md) | <code>static</code> | Constructs new channel which closes automatically after given period. |
|  [transduce(tx, rfn, acc)](./csp.channel.transduce.md) |  |  |
|  [tryRead(timeout)](./csp.channel.tryread.md) |  |  |
|  [write(value)](./csp.channel.write.md) |  |  |
