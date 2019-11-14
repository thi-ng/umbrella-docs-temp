<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/simd](./simd.md) &gt; [SIMD](./simd.simd.md)

## SIMD interface

<b>Signature:</b>

```typescript
export interface SIMD 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [f32](./simd.simd.f32.md) | <code>Float32Array</code> | Float32 view of WASM memory. |
|  [f64](./simd.simd.f64.md) | <code>Float64Array</code> | Float64 view of WASM memory. |
|  [i16](./simd.simd.i16.md) | <code>Int16Array</code> | Int16 view of WASM memory. |
|  [i32](./simd.simd.i32.md) | <code>Int32Array</code> | Int32 view of WASM memory. |
|  [i8](./simd.simd.i8.md) | <code>Int8Array</code> | Int8 view of WASM memory. |
|  [memory](./simd.simd.memory.md) | <code>WebAssembly.Memory</code> | WASM memory instance given to <code>init()</code>. |
|  [u16](./simd.simd.u16.md) | <code>Uint16Array</code> | Uint16 of WASM memory. |
|  [u32](./simd.simd.u32.md) | <code>Uint32Array</code> | Uint32 view of WASM memory. |
|  [u8](./simd.simd.u8.md) | <code>Uint8Array</code> | Uint8 view of WASM memory. |

## Methods

|  Method | Description |
|  --- | --- |
|  [abs4\_f32(out, a, num, so, sa)](./simd.simd.abs4_f32.md) |  |
|  [add4\_f32(out, a, b, num, so, sa, sb)](./simd.simd.add4_f32.md) |  |
|  [addn4\_f32(out, a, n, num, so, sa)](./simd.simd.addn4_f32.md) |  |
|  [clamp4\_f32(out, a, b, c, num, so, sa, sb, sc)](./simd.simd.clamp4_f32.md) |  |
|  [clampn4\_f32(out, a, b, c, num, so, sa)](./simd.simd.clampn4_f32.md) |  |
|  [div4\_f32(out, a, b, num, so, sa, sb)](./simd.simd.div4_f32.md) |  |
|  [divn4\_f32(out, a, n, num, so, sa)](./simd.simd.divn4_f32.md) |  |
|  [dot2\_f32\_aos(out, a, b, num)](./simd.simd.dot2_f32_aos.md) | Takes two densely packed vec2 AOS buffers <code>a</code> and <code>b</code>, computes their 2D dot products and stores results in <code>out</code>. Computes two results per iteration, hence <code>num</code> must be an even number or else the last vector will not be processed.<code>a</code> &amp; <code>b</code> should be aligned to 16. |
|  [dot4\_f32\_aos(out, a, b, num, so, sa, sb)](./simd.simd.dot4_f32_aos.md) | Takes two vec4 AOS buffers, computes their dot products and stores results in <code>out</code>. <code>so</code> should be 1 for packed result buffer. <code>sa</code> and <code>sb</code> indicate the stride lengths (in floats) between each vector in each respective buffer and should be a multiple of 4. |
|  [dot4\_f32\_soa(out, a, b, num, sa, sb)](./simd.simd.dot4_f32_soa.md) | Takes two vec4 SOA buffers and computes their 4D dot products and writes results to <code>out</code>. <code>sa</code> and <code>sb</code> indicate the element stride size (in floats) of the respective vectors (should be multiple of 4). The results are always stored in a packed layout. Processes 4 vectors per iteration, hence <code>num</code> should be a multiple of 4 too. |
|  [invsqrt4\_f32(out, a, num, so, sa)](./simd.simd.invsqrt4_f32.md) | FIXME waiting for native impl of SIMD instr[SIMD.sqrt4\_f32()](./simd.simd.sqrt4_f32.md) |
|  [madd4\_f32(out, a, b, c, num, so, sa, sb, sc)](./simd.simd.madd4_f32.md) | Takes three vec4 buffers, computes componentwise <code>a * b + c</code> and stores results in <code>out</code>. Both AOS / SOA layouts are supported, as long as all buffers are using the same layout.<!-- -->All strides must by multiples of 4. All pointers should be aligned to multiples of 16. Returns <code>out</code> pointer. |
|  [maddn4\_f32(out, a, b, c, num, so, sa, sc)](./simd.simd.maddn4_f32.md) |  |
|  [mag2\_f32\_aos(out, a, num)](./simd.simd.mag2_f32_aos.md) |  |
|  [mag4\_f32\_aos(out, a, num, so, sa)](./simd.simd.mag4_f32_aos.md) |  |
|  [magsq2\_f32\_aos(out, a, num)](./simd.simd.magsq2_f32_aos.md) |  |
|  [magsq4\_f32\_aos(out, a, num, so, sa)](./simd.simd.magsq4_f32_aos.md) |  |
|  [max4\_f32(out, a, b, num, so, sa, sb)](./simd.simd.max4_f32.md) |  |
|  [min4\_f32(out, a, b, num, so, sa, sb)](./simd.simd.min4_f32.md) |  |
|  [mix4\_f32(out, a, b, t, num, so, sa, sb, st)](./simd.simd.mix4_f32.md) |  |
|  [mixn4\_f32(out, a, b, t, num, so, sa, sb)](./simd.simd.mixn4_f32.md) |  |
|  [msub4\_f32(out, a, b, c, num, so, sa, sb, sc)](./simd.simd.msub4_f32.md) |  |
|  [msubn4\_f32(out, a, b, c, num, so, sa, sc)](./simd.simd.msubn4_f32.md) |  |
|  [mul\_m22v2\_aos(out, mat, vec, num)](./simd.simd.mul_m22v2_aos.md) |  |
|  [mul\_m23v2\_aos(out, mat, vec, num)](./simd.simd.mul_m23v2_aos.md) |  |
|  [mul\_m44v4\_aos(out, mat, vec, num, so, sv)](./simd.simd.mul_m44v4_aos.md) |  |
|  [mul4\_f32(out, a, b, num, so, sa, sb)](./simd.simd.mul4_f32.md) |  |
|  [muln4\_f32(out, a, n, num, so, sa)](./simd.simd.muln4_f32.md) |  |
|  [neg4\_f32(out, a, num, so, sa)](./simd.simd.neg4_f32.md) |  |
|  [normalize2\_f32\_aos(out, a, num, norm)](./simd.simd.normalize2_f32_aos.md) |  |
|  [normalize4\_f32\_aos(out, a, num, norm, so, sa)](./simd.simd.normalize4_f32_aos.md) |  |
|  [sqrt4\_f32(out, a, num, so, sa)](./simd.simd.sqrt4_f32.md) | FIXME waiting for native impl of SIMD instr[SIMD.invsqrt4\_f32()](./simd.simd.invsqrt4_f32.md) |
|  [sub4\_f32(out, a, b, num, so, sa, sb)](./simd.simd.sub4_f32.md) |  |
|  [subn4\_f32(out, a, n, num, so, sa)](./simd.simd.subn4_f32.md) |  |
|  [sum4\_f32(a, num, sa)](./simd.simd.sum4_f32.md) |  |
