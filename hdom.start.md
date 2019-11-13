<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/hdom](./hdom.md) &gt; [start](./hdom.start.md)

## start variable

Takes an hiccup tree (array, function or component object w/ life cycle methods) and an optional object of DOM update options. Starts RAF update loop, in each iteration first normalizing given tree, then computing diff to previous frame's tree and applying any changes to the real DOM. The `ctx` option can be used for passing arbitrary config data or state down into the hiccup component tree. Any embedded component function in the tree will receive this context object (shallow copy) as first argument, as will life cycle methods in component objects. If the `autoDerefKeys` option is given, attempts to auto-expand/deref the given keys in the user supplied context object (`ctx` option) prior to \*each\* tree normalization. All of these values should implement the [IDeref](./api.ideref.md) interface (e.g. atoms, cursors, views, rstreams etc.). This feature can be used to define dynamic contexts linked to the main app state, e.g. using derived views provided by .

\*\*Selective updates\*\*: No updates will be applied if the given hiccup tree is `undefined` or `null` or a root component function returns no value. This way a given root function can do some state handling of its own and implement fail-fast checks to determine no DOM updates are necessary, save effort re-creating a new hiccup tree and request skipping DOM updates via this function. In this case, the previous DOM tree is kept around until the root function returns a tree again, which then is diffed and applied against the previous tree kept as usual. Any number of frames may be skipped this way.

\*\*Important:\*\* Unless the `hydrate` option is enabled, the parent element given is assumed to have NO children at the time when `start()` is called. Since hdom does NOT track the real DOM, the resulting changes will result in potentially undefined behavior if the parent element wasn't empty. Likewise, if `hydrate` is enabled, it is assumed that an equivalent DOM (minus listeners) already exists (i.e. generated via SSR) when `start()` is called. Any other discrepancies between the pre-existing DOM and the hdom trees will cause undefined behavior.

Returns a function, which when called, immediately cancels the update loop.

<b>Signature:</b>

```typescript
start: (tree: any, opts?: Partial<HDOMOpts>, impl?: HDOMImplementation<any>) => () => boolean
```