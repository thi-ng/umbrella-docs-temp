<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast-js](./shader-ast-js.md)

## shader-ast-js package

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [JSBuiltinsBinary](./shader-ast-js.jsbuiltinsbinary.md) |  |
|  [JSBuiltinsCommon](./shader-ast-js.jsbuiltinscommon.md) |  |
|  [JSBuiltinsFloat](./shader-ast-js.jsbuiltinsfloat.md) |  |
|  [JSBuiltinsInt](./shader-ast-js.jsbuiltinsint.md) |  |
|  [JSBuiltinsIntVec](./shader-ast-js.jsbuiltinsintvec.md) |  |
|  [JSBuiltinsMat](./shader-ast-js.jsbuiltinsmat.md) |  |
|  [JSBuiltinsMath](./shader-ast-js.jsbuiltinsmath.md) |  |
|  [JSBuiltinsSampler](./shader-ast-js.jsbuiltinssampler.md) |  |
|  [JSBuiltinsVec](./shader-ast-js.jsbuiltinsvec.md) |  |
|  [JSBuiltinsVec3](./shader-ast-js.jsbuiltinsvec3.md) |  |
|  [JSBuiltinsVecScalar](./shader-ast-js.jsbuiltinsvecscalar.md) |  |
|  [JSEnv](./shader-ast-js.jsenv.md) |  |
|  [JSTarget](./shader-ast-js.jstarget.md) |  |

## Variables

|  Variable | Description |
|  --- | --- |
|  [canvasRenderer](./shader-ast-js.canvasrenderer.md) | Higher order function accepting an <code>HTMLCanvasElement</code> and returning a render function which accepts the following parameters:<!-- -->- <code>fn</code> - shader function (compiled via <code>targetJS().compile(ast)</code>) - <code>x</code>, <code>y</code>, <code>w</code>, <code>h</code> - optional args to define a sub-region to be updated (default to full image update) |
|  [JS\_DEFAULT\_ENV](./shader-ast-js.js_default_env.md) |  |
|  [renderBuffer](./shader-ast-js.renderbuffer.md) | Takes a [PackedBuffer](./pixel.packedbuffer.md) pixel buffer from thi.ng/pixel w/ [ABGR8888](./pixel.abgr8888.md) format, an optional buffer local region defined by <code>x</code>, <code>y</code>, <code>w</code>, <code>h</code> and applies shader function <code>fn</code> to each pixel in that region (or full buffer by default).<!-- -->In case the buffer only defines a sub-region of a larger image, <code>bufOffsetX</code>, <code>bufOffsetY</code> and <code>imgH</code> can be given to configure the location and full image height. |
|  [renderPixels](./shader-ast-js.renderpixels.md) | Low-level function used by [canvasRenderer](./shader-ast-js.canvasrenderer.md) and [renderBuffer](./shader-ast-js.renderbuffer.md)<!-- -->. Applies shader function <code>fn</code> to each pixel in the given region of the <code>u32</code> raw ABGR buffer (a <code>Uint32Array</code>). The region is defined by the top-left <code>x</code>, <code>y</code> coords and <code>w</code>, <code>h</code> dimensions. The remaining parameters <code>bufW</code>, <code>bufH</code>, <code>bufOffsetX</code>, <code>bufOffsetY</code> and <code>imgH</code> are used to define the actual location of the given buffer in the full image to be computed and to support use cases where the target array only defines a sub-region of the full image (e.g. when splitting rendering over multiple workers, each with their own buffer). |
|  [targetJS](./shader-ast-js.targetjs.md) |  |

