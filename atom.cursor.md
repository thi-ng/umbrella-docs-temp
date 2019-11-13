<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/atom](./atom.md) &gt; [Cursor](./atom.cursor.md)

## Cursor class

A cursor provides read/write access to a path location within a nested parent state (Atom or another Cursor). Cursors behave like Atoms for all practical purposes, i.e. support `deref()`<!-- -->, `reset()`<!-- -->, `swap()`<!-- -->, `addWatch()` etc. However, when updating a cursor's value, the parent state will be updated at the cursor's path as well (incl. triggering any watches and/or validators) attached to the parent. Likewise, when the parent state is modified externally, the cursor's value will automatically update as well. The update order of cursor's sharing a common parent is undefined, but can be overridden by extending this class with a custom `notifyWatches()` implementation.

If creating multiple cursors w/ a shared parent and each cursor configured with a custom ID (provided via config object to ctor), it's the user's responsibility to ensure the given IDs are unique. Cursors are implemented by attaching a watch to the parent and the ID is used to identify each watch.

When using the optional validator predicate (also specified via config object to ctor), the cursor's validator MUST NOT conflict with the one assigned to the parent or else both will go out-of-sync. Therefore, when requiring validation and updating values via cursors it's recommended to only specify validators for leaf-level cursors in the hierarchy.

<b>Signature:</b>

```typescript
export declare class Cursor<T> implements IAtom<T>, IID<string>, IRelease 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(opts)](./atom.cursor._constructor_.md) |  | Constructs a new instance of the <code>Cursor</code> class |
|  [(constructor)(parent, path)](./atom.cursor._constructor__1.md) |  | Constructs a new instance of the <code>Cursor</code> class |
|  [(constructor)(parent, lookup, update)](./atom.cursor._constructor__2.md) |  | Constructs a new instance of the <code>Cursor</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [id](./atom.cursor.id.md) |  | <code>string</code> |  |
|  [local](./atom.cursor.local.md) |  | <code>Atom&lt;T&gt;</code> |  |
|  [parent](./atom.cursor.parent.md) |  | <code>IAtom&lt;any&gt;</code> |  |
|  [selfUpdate](./atom.cursor.selfupdate.md) |  | <code>boolean</code> |  |
|  [value](./atom.cursor.value.md) |  | <code>T</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [addView(path, tx, lazy)](./atom.cursor.addview.md) |  |  |
|  [addWatch(id, fn)](./atom.cursor.addwatch.md) |  |  |
|  [deref()](./atom.cursor.deref.md) |  |  |
|  [notifyWatches(oldState, newState)](./atom.cursor.notifywatches.md) |  |  |
|  [release()](./atom.cursor.release.md) |  |  |
|  [removeWatch(id)](./atom.cursor.removewatch.md) |  |  |
|  [reset(val)](./atom.cursor.reset.md) |  |  |
|  [resetIn(path, val)](./atom.cursor.resetin.md) |  |  |
|  [swap(fn, args)](./atom.cursor.swap.md) |  |  |
|  [swapIn(path, fn, args)](./atom.cursor.swapin.md) |  |  |
