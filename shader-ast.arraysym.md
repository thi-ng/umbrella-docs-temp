<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast](./shader-ast.md) &gt; [arraySym](./shader-ast.arraysym.md)

## arraySym variable

Defines a new symbol with optional initial array values.

Important: Array initializers are UNSUPPORTED in GLSL ES v1 (WebGL), any code using such initializers will only work under WebGL2 or other targets.

<b>Signature:</b>

```typescript
arraySym: <T extends "bool" | "float" | "int" | "uint" | "vec2" | "vec3" | "vec4" | "ivec2" | "ivec3" | "ivec4" | "uvec2" | "uvec3" | "uvec4" | "bvec2" | "bvec3" | "bvec4" | "mat2" | "mat3" | "mat4" | "sampler2D" | "sampler3D" | "samplerCube" | "sampler2DShadow" | "samplerCubeShadow" | "isampler2D" | "isampler3D" | "isamplerCube" | "usampler2D" | "usampler3D" | "usamplerCube">(type: T, id?: string | undefined, opts?: SymOpts, init?: (Lit<T> | Sym<T>)[] | undefined) => Sym<ArrayTypeMap[T]>
```
