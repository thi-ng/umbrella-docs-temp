<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream](./rstream.md) &gt; [fromEvent](./rstream.fromevent.md)

## fromEvent variable

Creates a [Stream](./rstream.stream.md) of events attached to given element / event target and using given event listener options (same as supported by `addEventListener()`<!-- -->, default: false).

<b>Signature:</b>

```typescript
fromEvent: (src: EventTarget, name: string, listenerOpts?: boolean | AddEventListenerOptions, streamOpts?: Partial<CommonOpts> | undefined) => Stream<Event>
```
