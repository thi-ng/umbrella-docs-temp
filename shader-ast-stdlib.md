<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast-stdlib](./shader-ast-stdlib.md)

## shader-ast-stdlib package

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [RaymarchOpts](./shader-ast-stdlib.raymarchopts.md) |  |

## Variables

|  Variable | Description |
|  --- | --- |
|  [A](./shader-ast-stdlib.a.md) |  |
|  [additive](./shader-ast-stdlib.additive.md) | Higher order function. Takes an AST type ID, a single-arg scalar function <code>fn</code>, number of octaves (default: 4) and an optional function name. Returns a new function which computes the summed value of <code>fn</code> over the given number octaves and accepts 3 args:<!-- -->- position (float) - octave shift (float) - octave decay (usually 0.5)<!-- -->For each octave <code>i</code> \[0..oct), the function is (in principle) evaluated as:<!-- -->n += decay / exp2(i) \* fn(pos \* exp2(i) + i \* shift) |
|  [aspectCorrectedUV](./shader-ast-stdlib.aspectcorrecteduv.md) | Takes <code>pos</code>, a screen coord (e.g. gl\_FragCoord) and viewport resolution <code>res</code>, returns aspect corrected uv, with uv.y in \[-1..1\] interval. |
|  [B](./shader-ast-stdlib.b.md) |  |
|  [blendDestAtop](./shader-ast-stdlib.blenddestatop.md) |  |
|  [blendDestIn](./shader-ast-stdlib.blenddestin.md) |  |
|  [blendDestOut](./shader-ast-stdlib.blenddestout.md) |  |
|  [blendDestOver](./shader-ast-stdlib.blenddestover.md) |  |
|  [blendPlus](./shader-ast-stdlib.blendplus.md) |  |
|  [blendSrcAtop](./shader-ast-stdlib.blendsrcatop.md) |  |
|  [blendSrcIn](./shader-ast-stdlib.blendsrcin.md) |  |
|  [blendSrcOut](./shader-ast-stdlib.blendsrcout.md) |  |
|  [blendSrcOver](./shader-ast-stdlib.blendsrcover.md) |  |
|  [blendXor](./shader-ast-stdlib.blendxor.md) |  |
|  [blur13](./shader-ast-stdlib.blur13.md) | 13x13 gaussian blur texture lookup, optimized, but based on:<!-- -->- [http://rastergrid.com/blog/2010/09/efficient-gaussian-blur-with-linear-sampling/](http://rastergrid.com/blog/2010/09/efficient-gaussian-blur-with-linear-sampling/) - [https://github.com/Jam3/glsl-fast-gaussian-blur](https://github.com/Jam3/glsl-fast-gaussian-blur) |
|  [blur5](./shader-ast-stdlib.blur5.md) | 5x5 gaussian blur texture lookup, optimized, but based on:<!-- -->- [http://rastergrid.com/blog/2010/09/efficient-gaussian-blur-with-linear-sampling/](http://rastergrid.com/blog/2010/09/efficient-gaussian-blur-with-linear-sampling/) - [https://github.com/Jam3/glsl-fast-gaussian-blur](https://github.com/Jam3/glsl-fast-gaussian-blur) |
|  [blur9](./shader-ast-stdlib.blur9.md) | 9x9 gaussian blur texture lookup, optimized, but based on:<!-- -->- [http://rastergrid.com/blog/2010/09/efficient-gaussian-blur-with-linear-sampling/](http://rastergrid.com/blog/2010/09/efficient-gaussian-blur-with-linear-sampling/) - [https://github.com/Jam3/glsl-fast-gaussian-blur](https://github.com/Jam3/glsl-fast-gaussian-blur) |
|  [cartesian2](./shader-ast-stdlib.cartesian2.md) | Converts 2D polar vector <code>v</code>, i.e. <code>[r,θ]</code> (angle in radians) to cartesian coordinates. See [polar2](./shader-ast-stdlib.polar2.md) for reverse operation. |
|  [cartesian3](./shader-ast-stdlib.cartesian3.md) | Converts 3D polar/spherical vector <code>v</code>, i.e. <code>[r,θ,ϕ]</code> (angles in radians) to cartesian coordinates. See [polar3](./shader-ast-stdlib.polar3.md) for reverse operation. |
|  [clamp01](./shader-ast-stdlib.clamp01.md) | Inline function, expands to equivalent of <code>clamp(x, 0, 1)</code>. |
|  [clamp11](./shader-ast-stdlib.clamp11.md) | Inline function, expands to equivalent of <code>clamp(x, -1, 1)</code>. |
|  [coordToIndex](./shader-ast-stdlib.coordtoindex.md) | Inline function. Reverse op to [indexToCoord](./shader-ast-stdlib.indextocoord.md)<!-- -->. Not compatible with WebGL1. |
|  [cossin](./shader-ast-stdlib.cossin.md) | Inline function. Returns vec2(cos(x), sin(x)). |
|  [cross2](./shader-ast-stdlib.cross2.md) | Inline function. Computes 2D cross product of given vectors.[crossC2](./shader-ast-stdlib.crossc2.md) |
|  [crossC2](./shader-ast-stdlib.crossc2.md) | Inline function. Computes 2D cross product of given individual components: ax \* by - ay \* bx |
|  [curlNoise3](./shader-ast-stdlib.curlnoise3.md) |  |
|  [diffuseLighting](./shader-ast-stdlib.diffuselighting.md) | Inline function. Computes:<!-- -->col = lambert \* lightCol \* diffuseCol + ambientCol |
|  [distChebyshev2](./shader-ast-stdlib.distchebyshev2.md) |  |
|  [distChebyshev3](./shader-ast-stdlib.distchebyshev3.md) |  |
|  [distChebyshev4](./shader-ast-stdlib.distchebyshev4.md) |  |
|  [distManhattan2](./shader-ast-stdlib.distmanhattan2.md) |  |
|  [distManhattan3](./shader-ast-stdlib.distmanhattan3.md) |  |
|  [distManhattan4](./shader-ast-stdlib.distmanhattan4.md) |  |
|  [fit01](./shader-ast-stdlib.fit01.md) | Inline function. Fits value <code>a</code> in \[0..1\] interval to new interval \[b..c\]. No clamping performed. Same as <code>mix(b, c, a)</code> |
|  [fit0111](./shader-ast-stdlib.fit0111.md) | Inline function. Fits value <code>x</code> in \[0..1\] interval to \[-1..+1\] interval. No clamping performed. |
|  [fit1101](./shader-ast-stdlib.fit1101.md) | Inline function. Fits value <code>x</code> in \[-1..+1\] interval to \[0..1\] interval. No clamping performed. |
|  [fitNorm1](./shader-ast-stdlib.fitnorm1.md) | Returns normalized value of <code>x</code> WRT to interval \[a,b\]. Returns 0, if <code>a</code> equals <code>b</code>. |
|  [fogExp](./shader-ast-stdlib.fogexp.md) | Computes exponential fog factor \[0..1\], based on given fully saturated fog distance and density. |
|  [fogExp2](./shader-ast-stdlib.fogexp2.md) | Similar to [fogExp](./shader-ast-stdlib.fogexp.md)<!-- -->. Computes exponential fog factor \[0..1\], based on given fully saturated fog distance and density. Uses [exp2](./shader-ast.exp2.md) internally. |
|  [fogLinear](./shader-ast-stdlib.foglinear.md) | Computes linear fog factor \[0..1\], based on given fog min/max distances. |
|  [fragUV](./shader-ast-stdlib.fraguv.md) | Computes UV coord in \[0..1\] interval from given <code>fragCoord</code> and screen <code>res</code>. |
|  [halfLambert](./shader-ast-stdlib.halflambert.md) | Inline function. Computes Half-Lambertian term. Both vectors must be pre-normalized.[https://developer.valvesoftware.com/wiki/Half\_Lambert](https://developer.valvesoftware.com/wiki/Half_Lambert) |
|  [hash11](./shader-ast-stdlib.hash11.md) | 1D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash12](./shader-ast-stdlib.hash12.md) | 2D -<!-- -->&gt; 1D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash13](./shader-ast-stdlib.hash13.md) | 3D -<!-- -->&gt; 1D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash2](./shader-ast-stdlib.hash2.md) | iq's hash PRNG producing 2D results. |
|  [hash21](./shader-ast-stdlib.hash21.md) | 1D -<!-- -->&gt; 2D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash22](./shader-ast-stdlib.hash22.md) | 2D -<!-- -->&gt; 2D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash23](./shader-ast-stdlib.hash23.md) | 3D -<!-- -->&gt; 2D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash3](./shader-ast-stdlib.hash3.md) | iq's hash PRNG producing 3D results. |
|  [hash31](./shader-ast-stdlib.hash31.md) | 1D -<!-- -->&gt; 3D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash32](./shader-ast-stdlib.hash32.md) | 2D -<!-- -->&gt; 3D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash33](./shader-ast-stdlib.hash33.md) | 3D -<!-- -->&gt; 3D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash41](./shader-ast-stdlib.hash41.md) | 1D -<!-- -->&gt; 4D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash42](./shader-ast-stdlib.hash42.md) | 2D -<!-- -->&gt; 4D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash43](./shader-ast-stdlib.hash43.md) | 3D -<!-- -->&gt; 4D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [hash44](./shader-ast-stdlib.hash44.md) | 4D -<!-- -->&gt; 4D hash.<!-- -->Dave Hoskins (https://www.shadertoy.com/view/4djSRW) |
|  [indexToCoord](./shader-ast-stdlib.indextocoord.md) | Inline function. Similar to [indexToUV](./shader-ast-stdlib.indextouv.md)<!-- -->, but returns uvec2 in pixel coords. Not compatible with WebGL1. |
|  [indexToUV](./shader-ast-stdlib.indextouv.md) | Converts linearized 2D index <code>i</code> into a vec2 UV coord, based on given texture <code>size</code> (in pixels). |
|  [lambert](./shader-ast-stdlib.lambert.md) | Inline function. Computes Lambert term, i.e. <code>max(dot(n, l), 0)</code>. Both vectors must be pre-normalized. |
|  [lookat](./shader-ast-stdlib.lookat.md) | Creates a mat4 view matrix from given <code>eyePos</code>, <code>target</code> and <code>up</code> vector. |
|  [luminanceRGB](./shader-ast-stdlib.luminancergb.md) | Inline function. Computes luminance of given RGB color |
|  [magSq2](./shader-ast-stdlib.magsq2.md) |  |
|  [magSq3](./shader-ast-stdlib.magsq3.md) |  |
|  [magSq4](./shader-ast-stdlib.magsq4.md) |  |
|  [maxComp2](./shader-ast-stdlib.maxcomp2.md) | Inline function. Returns max(v.x, v.y) |
|  [maxComp3](./shader-ast-stdlib.maxcomp3.md) | Inline function. Returns max(v.x, v.y, v.z) |
|  [maxComp4](./shader-ast-stdlib.maxcomp4.md) | Inline function. Returns max(v.x, v.y, v.z, v.w) |
|  [minComp2](./shader-ast-stdlib.mincomp2.md) | Inline function. Returns min(v.x, v.y) |
|  [minComp3](./shader-ast-stdlib.mincomp3.md) | Inline function. Returns min(v.x, v.y, v.z) |
|  [minComp4](./shader-ast-stdlib.mincomp4.md) | Inline function. Returns min(v.x, v.y, v.z, v.w) |
|  [ONE\_MINUS\_A](./shader-ast-stdlib.one_minus_a.md) |  |
|  [ONE\_MINUS\_B](./shader-ast-stdlib.one_minus_b.md) |  |
|  [ONE](./shader-ast-stdlib.one.md) |  |
|  [orthogonal3](./shader-ast-stdlib.orthogonal3.md) | Returns an orthogonal vector to <code>v</code>.[http://lolengine.net/blog/2013/09/21/picking-orthogonal-vector-combing-coconuts](http://lolengine.net/blog/2013/09/21/picking-orthogonal-vector-combing-coconuts) |
|  [permute](./shader-ast-stdlib.permute.md) |  |
|  [permute2](./shader-ast-stdlib.permute2.md) |  |
|  [permute3](./shader-ast-stdlib.permute3.md) |  |
|  [permute4](./shader-ast-stdlib.permute4.md) |  |
|  [perpendicularCCW](./shader-ast-stdlib.perpendicularccw.md) | Inline function. Returns counter-clockwise perpendicular vector (assuming Y-up). \[-y, x\] |
|  [perpendicularCW](./shader-ast-stdlib.perpendicularcw.md) | Inline function. Returns clockwise perpendicular vector (assuming Y-up). \[y,-x\] |
|  [polar2](./shader-ast-stdlib.polar2.md) | Converts 2D cartesian vector <code>v</code> to polar coordinates, i.e. <code>[r,θ]</code> (angle in radians). See [cartesian2](./shader-ast-stdlib.cartesian2.md) for reverse operation. |
|  [polar3](./shader-ast-stdlib.polar3.md) | Converts 3D cartesian vector <code>v</code> to spherical coordinates, i.e. <code>[r,θ,ϕ]</code> (angles in radians). See [cartesian3](./shader-ast-stdlib.cartesian3.md) for reverse operation. |
|  [porterDuff](./shader-ast-stdlib.porterduff.md) | Higher-order Porter-Duff alpha compositing operator. See [@thi.ng/porter-duff](./porter-duff.md) for reference. Returns an optimized AST function which accepts 2 RGBA colors (vec4) and returns blended &amp; clamped result (also a vec4). All built-in PD operators are defined via this HOF.<!-- -->The two given JS functions are used to extract blending coefficients for src/dest colors and are called with the alpha components of both colors.<!-- -->Optimization only happens for cases where either <code>fa</code> and/or <code>fb</code> are [ZERO](./shader-ast-stdlib.zero.md)<!-- -->. |
|  [raymarchAO](./shader-ast-stdlib.raymarchao.md) | Higher order function returning an function to compute the Ambient Occlusion term / shadow factor for given SDF scene function. The returned function takes 2 arguments: surface pos and normal. It returns a float in \[0..1\] interval (zero = fully occluded). |
|  [raymarchDir](./shader-ast-stdlib.raymarchdir.md) |  |
|  [raymarchNormal](./shader-ast-stdlib.raymarchnormal.md) | Higher order function producing a function to compute the raymarched scene normal for a given scene function and intersection position. Like [raymarchScene](./shader-ast-stdlib.raymarchscene.md)<!-- -->, this function takes an existing scene function as argument. |
|  [raymarchScene](./shader-ast-stdlib.raymarchscene.md) | Higher order function producing a function to perform a raymarch using the provided <code>scene</code> function and options to configure the raymarch process itself.<!-- -->Returns an AST function which takes 2 args: ray origin, normalized ray direction and returning a 2D vector of:<!-- -->- x = the signed distance to the <code>scene</code> defined SDF surface - y = user data provided by <code>scene</code> (e.g. material ID)<!-- -->The <code>scene</code> function itself takes a 3D point as input and returns a vec2 with the same component meaning as above. |
|  [rayPointAt](./shader-ast-stdlib.raypointat.md) | Inline function. Returns point on ray (<code>p</code>, <code>dir</code>) at distance <code>t</code>. Unless <code>norm</code> is true (default false), <code>dir</code> must be already normalized. |
|  [readIndex1](./shader-ast-stdlib.readindex1.md) | Inline function. Returns x component at index <code>i</code> in <code>tex</code>. |
|  [readIndex2](./shader-ast-stdlib.readindex2.md) | Inline function. Returns vec2 (x,y components) at index <code>i</code> in <code>tex</code>. |
|  [readIndex3](./shader-ast-stdlib.readindex3.md) | Inline function. Returns vec3 (x,y,z components) at index <code>i</code> in <code>tex</code>. |
|  [readIndex4](./shader-ast-stdlib.readindex4.md) | Inline function. Returns vec4 at index <code>i</code> in <code>tex</code>. |
|  [rotation2](./shader-ast-stdlib.rotation2.md) |  |
|  [rotationAroundAxis3](./shader-ast-stdlib.rotationaroundaxis3.md) |  |
|  [rotationAroundAxis4](./shader-ast-stdlib.rotationaroundaxis4.md) |  |
|  [rotationX3](./shader-ast-stdlib.rotationx3.md) |  |
|  [rotationX4](./shader-ast-stdlib.rotationx4.md) |  |
|  [rotationY3](./shader-ast-stdlib.rotationy3.md) |  |
|  [rotationY4](./shader-ast-stdlib.rotationy4.md) |  |
|  [rotationZ3](./shader-ast-stdlib.rotationz3.md) |  |
|  [rotationZ4](./shader-ast-stdlib.rotationz4.md) |  |
|  [sdfAnnular](./shader-ast-stdlib.sdfannular.md) | Inline function. Bi-directional offset to create ring like shapes. |
|  [sdfBox2](./shader-ast-stdlib.sdfbox2.md) | Returns signed distance from <code>p</code> to centered AABB of <code>size</code>. |
|  [sdfBox3](./shader-ast-stdlib.sdfbox3.md) | Returns signed distance from <code>p</code> to centered AABB of <code>size</code>. |
|  [sdfCircle](./shader-ast-stdlib.sdfcircle.md) | Returns signed distance from <code>p</code> to centered circle of radius <code>r</code>. |
|  [sdfCylinder](./shader-ast-stdlib.sdfcylinder.md) | Returns signed distance from <code>p</code> to cylinder centered around Y-axis with height <code>h</code> and radius <code>r</code>. |
|  [sdfIntersect](./shader-ast-stdlib.sdfintersect.md) | Inline function. SDF shape intersection (a &amp; b). |
|  [sdfLine2](./shader-ast-stdlib.sdfline2.md) | Returns signed distance from <code>p</code> to centered circle of radius <code>r</code>. |
|  [sdfLine3](./shader-ast-stdlib.sdfline3.md) |  |
|  [sdfPlane2](./shader-ast-stdlib.sdfplane2.md) | Returns signed distance from <code>p</code> to plane defined by <code>normal</code> and <code>w</code>. |
|  [sdfPlane3](./shader-ast-stdlib.sdfplane3.md) | Returns signed distance from <code>p</code> to plane defined by <code>normal</code> and <code>w</code>. |
|  [sdfRepeat2](./shader-ast-stdlib.sdfrepeat2.md) | Domain repetition by wrapping position <code>p</code> into period <code>c</code>. |
|  [sdfRepeat3](./shader-ast-stdlib.sdfrepeat3.md) | Domain repetition by wrapping position <code>p</code> into period <code>c</code>. |
|  [sdfRound](./shader-ast-stdlib.sdfround.md) | Inline function. Essentially an isoline offset to create:<!-- -->- <code>r &gt; 0</code>: rounded/thicker shapes - <code>r &lt; 0</code>: sharper/thinner shapes |
|  [sdfSmoothIntersect](./shader-ast-stdlib.sdfsmoothintersect.md) |  |
|  [sdfSmoothSubtract](./shader-ast-stdlib.sdfsmoothsubtract.md) |  |
|  [sdfSmoothUnion](./shader-ast-stdlib.sdfsmoothunion.md) |  |
|  [sdfSphere](./shader-ast-stdlib.sdfsphere.md) | Returns signed distance from <code>p</code> to centered sphere of radius <code>r</code>. |
|  [sdfTorus](./shader-ast-stdlib.sdftorus.md) | Returns signed distance from <code>p</code> to torus centered around Y-axis with radii <code>r1</code>, <code>r2</code>. |
|  [sdfTriangle2](./shader-ast-stdlib.sdftriangle2.md) |  |
|  [sdfUnion](./shader-ast-stdlib.sdfunion.md) | Inline function. SDF shape union (a \|\| b). |
|  [sincos](./shader-ast-stdlib.sincos.md) | Inline function. Returns vec2(sin(x), cos(x)). |
|  [snoise2](./shader-ast-stdlib.snoise2.md) | Array and textureless GLSL 2D simplex noise function. Ported from original GLSL implementation by Ian McEwan &amp; Ashima Arts.[https://github.com/ashima/webgl-noise](https://github.com/ashima/webgl-noise) |
|  [snoise3](./shader-ast-stdlib.snoise3.md) |  |
|  [snoiseVec3](./shader-ast-stdlib.snoisevec3.md) |  |
|  [surfaceNormal](./shader-ast-stdlib.surfacenormal.md) | Inline function. Multiplies <code>normal</code> with given 4x4 normal matrix (e.g. transpose inverse of view \* model). |
|  [toLinear](./shader-ast-stdlib.tolinear.md) | Inline function. Converts sRGB color term (1D-4D) to linear space via <code>pow(rgb, GAMMA)</code>, where gamma is hardcoded to 2.2. For vec4 args, the <code>w</code> component (alpha) remains unchanged. |
|  [toSRGB](./shader-ast-stdlib.tosrgb.md) | Inline function. Converts linear color term (1D-4D) to sRGB via <code>pow(rgb, 1.0 / GAMMA)</code>, where gamma is hardcoded to 2.2. For vec4 args, the <code>w</code> component (alpha) remains unchanged. |
|  [transformMVP](./shader-ast-stdlib.transformmvp.md) | Inline function. Multiplies <code>pos</code> with given model, view &amp; projection matrices (in order). <code>p</code> is extended to a vec4. |
|  [trilight](./shader-ast-stdlib.trilight.md) | Tom Forsyth's Trilight lighting model. |
|  [uvToIndex](./shader-ast-stdlib.uvtoindex.md) | Inverse operation of [indexToUV](./shader-ast-stdlib.indextouv.md)<!-- -->. Converts vec2 UV coord into linearized 2D index, based on given texture <code>width</code> (in pixels). |
|  [voronoise2](./shader-ast-stdlib.voronoise2.md) | IQ's parametric 2D voronoise. Depending on <code>u</code> and <code>v</code>, this function produces 4 different noise types<!-- -->- cell noise (0,0) - voronoi (1,0) - perlin noise (0,1) - voronoise (1,1)[http://www.iquilezles.org/www/articles/voronoise/voronoise.htm](http://www.iquilezles.org/www/articles/voronoise/voronoise.htm)<!-- -->Note: This implementation uses the improved [hash32](./shader-ast-stdlib.hash32.md) by Dave Hoskins instead of iq's original [hash3](./shader-ast-stdlib.hash3.md)<!-- -->. |
|  [worley2](./shader-ast-stdlib.worley2.md) | Higher order function. Computes 2D Worley noise using provided distance function. The returned function takes 2 args: position and jitter amount, the latter in \[0..1\] interval. Returns noise components as vec2, with the x component containing the distance from closest simplex center and y the noise value. The vector components can be used individually or combined (e.g. <code>noise.y - noise.x</code>)...<!-- -->Based on implementation by Stefan Gustavson: [http://webstaff.itn.liu.se/\~stegu/GLSL-cellular/GLSL-cellular-notes.pdf](http://webstaff.itn.liu.se/~stegu/GLSL-cellular/GLSL-cellular-notes.pdf) |
|  [worleyDist](./shader-ast-stdlib.worleydist.md) |  |
|  [worleyDistManhattan](./shader-ast-stdlib.worleydistmanhattan.md) |  |
|  [ZERO](./shader-ast-stdlib.zero.md) |  |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [RaymarchScene](./shader-ast-stdlib.raymarchscene.md) |  |

