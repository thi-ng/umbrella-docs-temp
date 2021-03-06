<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/webgl](./webgl.md) &gt; [ModelAttributeSpec](./webgl.modelattributespec.md)

## ModelAttributeSpec interface

Data specification of a single WebGL attribute

<b>Signature:</b>

```typescript
export interface ModelAttributeSpec 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [buffer](./webgl.modelattributespec.buffer.md) | <code>IWebGLBuffer&lt;AttribBufferData&gt;</code> | Backing [WebGLArrayBuffer](./webgl.webglarraybuffer.md) instance. Usually this will be auto-initialized by  |
|  [data](./webgl.modelattributespec.data.md) | <code>AttribBufferData</code> | Raw attribute data from which <code>buffer</code> will be initialized |
|  [divisor](./webgl.modelattributespec.divisor.md) | <code>number</code> | Only used for instanced attributes. See: [https://www.khronos.org/registry/OpenGL/extensions/ANGLE/ANGLE\_instanced\_arrays.txt](https://www.khronos.org/registry/OpenGL/extensions/ANGLE/ANGLE_instanced_arrays.txt) |
|  [normalized](./webgl.modelattributespec.normalized.md) | <code>boolean</code> | Auto-normalization flag when writing buffer data. Default: false |
|  [offset](./webgl.modelattributespec.offset.md) | <code>number</code> | Byte offset of 1st attrib component. Default: 0 |
|  [size](./webgl.modelattributespec.size.md) | <code>number</code> | Attribute element size (in component values, not bytes). Default: 3 |
|  [stride](./webgl.modelattributespec.stride.md) | <code>number</code> | Attribute stride in bytes. Default: 0 = densely packed |
|  [type](./webgl.modelattributespec.type.md) | <code>GLenum</code> | Attribute's WebGL data type. Default: gl.FLOAT |

