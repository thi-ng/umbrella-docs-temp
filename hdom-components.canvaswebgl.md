<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/hdom-components](./hdom-components.md) &gt; [canvasWebGL](./hdom-components.canvaswebgl.md)

## canvasWebGL variable

Higher order WebGL canvas component delegating to user provided handlers.

<b>Signature:</b>

```typescript
canvasWebGL: (handlers: Partial<CanvasHandlers<WebGLRenderingContext>>, opts?: WebGLContextAttributes | undefined) => {
    init(_el: HTMLCanvasElement, hctx: any, ...args: any[]): void;
    render(hctx: any, ...args: any[]): any[];
    release(hctx: any, ...args: any[]): void;
}
```

## Remarks

Since this is an higher order component, if used within a non-static parent component, this function itself cannot be directly inlined into hdom tree and must be initialized prior/outside, however the returned component can be used as normal.

## Example


```ts
const glcanvas = canvasWebGL({
  render(canv, gl, hctx, time, frame, ...args) {
    const col = 0.5 + 0.5 * Math.sin(time);
    gl.clearColor(col, col, col, 1);
  }
});
...
[glcanvas, {id: "foo", width: 640, height: 480}]

```

