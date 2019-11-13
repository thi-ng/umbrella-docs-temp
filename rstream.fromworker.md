<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [fromWorker](./rstream.fromworker.md)

## fromWorker variable

Returns a new `Stream` instance which adds "message" and "error" event listeners to given `worker` and then passes received values downstream. If `terminate` is true (default), the worker will be terminated when the stream is being closed (either directly or indirectly, i.e. if the user called `.done()` on the stream or the last child subscription has unsubscribed).

As with `postWorker()`<!-- -->, the `worker` can be an existing `Worker` instance, a JS source code `Blob` or an URL string. In the latter two cases, a worker is created automatically using `utils/makeWorker()`<!-- -->.

```


```

<b>Signature:</b>

```typescript
fromWorker: <T>(worker: string | Blob | Worker, terminate?: boolean, id?: string | undefined) => Stream<T>
```