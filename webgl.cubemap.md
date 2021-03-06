<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/webgl](./webgl.md) &gt; [cubeMap](./webgl.cubemap.md)

## cubeMap variable

Creates cube map texture from given 6 `face` texture sources. The given options are shared by each each side/face of the cube map. The following options are applied to the cube map directly:

- `filter` - `mipmap`

The following options are ignored entirely:

- `target` - `image`

<b>Signature:</b>

```typescript
cubeMap: (gl: WebGLRenderingContext, faces: (ArrayBufferView | HTMLCanvasElement | HTMLImageElement | HTMLVideoElement | ImageBitmap | OffscreenCanvas | ImageData)[], opts?: Partial<TextureOpts>) => Texture
```
