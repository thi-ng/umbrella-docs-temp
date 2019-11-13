<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/matrices](./matrices.md)

## matrices package

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [MultiMatOp1](./matrices.multimatop1.md) |  |
|  [MultiMatOpM](./matrices.multimatopm.md) |  |
|  [MultiMatOpMM](./matrices.multimatopmm.md) |  |
|  [MultiMatOpMN](./matrices.multimatopmn.md) |  |
|  [MultiMatOpMU](./matrices.multimatopmu.md) |  |
|  [MultiMatOpMV](./matrices.multimatopmv.md) |  |
|  [MultiMatOpN](./matrices.multimatopn.md) |  |
|  [MultiVecOpM](./matrices.multivecopm.md) |  |
|  [MultiVecOpMN](./matrices.multivecopmn.md) |  |

## Variables

|  Variable | Description |
|  --- | --- |
|  [add](./matrices.add.md) | Componentwise matrix addition. If <code>out</code> is not given, writes result in <code>a</code>.<!-- -->out = a + b |
|  [add22](./matrices.add22.md) |  |
|  [add23](./matrices.add23.md) |  |
|  [add33](./matrices.add33.md) |  |
|  [add44](./matrices.add44.md) |  |
|  [addN](./matrices.addn.md) | Adds single scalar componentwise to matrix. If <code>out</code> is not given, writes result in <code>mat</code>.<!-- -->out = mat + n |
|  [addN22](./matrices.addn22.md) |  |
|  [addN23](./matrices.addn23.md) |  |
|  [addN33](./matrices.addn33.md) |  |
|  [addN44](./matrices.addn44.md) |  |
|  [alignmentQuat](./matrices.alignmentquat.md) | Returns quaternion describing the rotation from direction vector <code>from</code> -<!-- -->&gt; <code>to</code>. If <code>normalize</code> is true (default), first normalizes the vectors (not modifying original). |
|  [column](./matrices.column.md) | Extracts column vector from given matrix and writes result to <code>out</code>. If <code>out</code> is null, creates new vector. |
|  [column22](./matrices.column22.md) |  |
|  [column23](./matrices.column23.md) |  |
|  [column33](./matrices.column33.md) |  |
|  [column44](./matrices.column44.md) |  |
|  [concat](./matrices.concat.md) | Concatenates / multiplies given matrices in left-to-right order. A minimum of 2 input matrices must be given. If <code>out</code> is null, writes result into <code>a</code>. |
|  [conjugateQ](./matrices.conjugateq.md) |  |
|  [defMath](./matrices.defmath.md) |  |
|  [defMathN](./matrices.defmathn.md) |  |
|  [det22](./matrices.det22.md) |  |
|  [det23](./matrices.det23.md) |  |
|  [det33](./matrices.det33.md) |  |
|  [det44](./matrices.det44.md) |  |
|  [det44FromCoeffs](./matrices.det44fromcoeffs.md) |  |
|  [detCoeffs44](./matrices.detcoeffs44.md) |  |
|  [diag](./matrices.diag.md) | Extracts matrix diagonal into <code>out</code>. |
|  [diag22](./matrices.diag22.md) |  |
|  [diag23](./matrices.diag23.md) |  |
|  [diag33](./matrices.diag33.md) |  |
|  [diag44](./matrices.diag44.md) |  |
|  [div](./matrices.div.md) | Componentwise matrix division. If <code>out</code> is not given, writes result in <code>a</code>.<!-- -->out = a / b |
|  [div22](./matrices.div22.md) |  |
|  [div23](./matrices.div23.md) |  |
|  [div33](./matrices.div33.md) |  |
|  [div44](./matrices.div44.md) |  |
|  [divN](./matrices.divn.md) | Componentwise matrix division by single scalar. If <code>out</code> is not given, writes result in <code>mat</code>.<!-- -->out = mat / n |
|  [divN22](./matrices.divn22.md) |  |
|  [divN23](./matrices.divn23.md) |  |
|  [divN33](./matrices.divn33.md) |  |
|  [divN44](./matrices.divn44.md) |  |
|  [frustum](./matrices.frustum.md) | Constructs a 4x4 matrix representing the given view frustum. Creates new matrix if <code>out</code> is <code>null</code>. |
|  [frustumBounds](./matrices.frustumbounds.md) |  |
|  [IDENT22](./matrices.ident22.md) |  |
|  [IDENT23](./matrices.ident23.md) |  |
|  [IDENT33](./matrices.ident33.md) |  |
|  [IDENT44](./matrices.ident44.md) |  |
|  [identity](./matrices.identity.md) | Writes identity matrix into given matrix. |
|  [identity22](./matrices.identity22.md) |  |
|  [identity23](./matrices.identity23.md) |  |
|  [identity33](./matrices.identity33.md) |  |
|  [identity44](./matrices.identity44.md) |  |
|  [invert](./matrices.invert.md) | Matrix inversion. Returns <code>undefined</code> if matrix is not invertible. Mutates <code>mat</code> if <code>out</code> is <code>null</code>. |
|  [invert22](./matrices.invert22.md) |  |
|  [invert23](./matrices.invert23.md) |  |
|  [invert33](./matrices.invert33.md) |  |
|  [invert44](./matrices.invert44.md) |  |
|  [invertQ](./matrices.invertq.md) |  |
|  [isOrthagonal](./matrices.isorthagonal.md) | Returns true, if given square matrix of size <code>n</code> is orthagonal, i.e. check if <code>A * AT = I</code>.[https://en.wikipedia.org/wiki/Orthogonal\_matrix](https://en.wikipedia.org/wiki/Orthogonal_matrix) |
|  [lookAt](./matrices.lookat.md) | Constructs a 4x4 camera matrix for given <code>eye</code> position, look-at <code>target</code> (both in world space) and normalized <code>up</code> vector. Creates new matrix if <code>out</code> is <code>null</code>. |
|  [mat22n](./matrices.mat22n.md) |  |
|  [mat22to23](./matrices.mat22to23.md) | Converts 2x2 to 2x3 matrix and writes result to <code>out</code>. Creates new matrix if <code>out</code> is <code>null</code>. |
|  [mat22v](./matrices.mat22v.md) | Initializes 2x2 matrix from 2D column vectors. |
|  [mat23n](./matrices.mat23n.md) |  |
|  [mat23to22](./matrices.mat23to22.md) | Converts 2x3 to 2x2 matrix and writes result to <code>out</code>. Creates new matrix if <code>out</code> is <code>null</code>. |
|  [mat23to44](./matrices.mat23to44.md) | Converts 2x3 to 4x4 matrix and writes result to <code>out</code>. Creates new matrix if <code>out</code> is <code>null</code>. |
|  [mat23v](./matrices.mat23v.md) | Initializes 2x3 matrix (affine transform) from 2D column vectors. |
|  [mat33n](./matrices.mat33n.md) |  |
|  [mat33to44](./matrices.mat33to44.md) | Converts 3x3 to 4x4 matrix and writes result to <code>out</code>. Creates new matrix if <code>out</code> is <code>null</code>. |
|  [mat33v](./matrices.mat33v.md) | Initializes 3x3 matrix from 3D column vectors. |
|  [mat44n](./matrices.mat44n.md) |  |
|  [mat44to33](./matrices.mat44to33.md) | Converts 4x4 to 3x3 matrix and writes result to <code>out</code>. Creates new matrix if <code>out</code> is <code>null</code>. |
|  [mat44v](./matrices.mat44v.md) | Initializes 4x4 matrix from 4D column vectors. |
|  [mixQ](./matrices.mixq.md) | Interpolates quaternion <code>a</code> to <code>b</code> by given amount <code>t</code> \[0...1\], using SLERP. Writes result to <code>out</code>. The optional <code>eps</code> (default 1e-3) is used to switch to linear interpolation if the angular difference is very small. |
|  [mul](./matrices.mul.md) | Componentwise matrix addition. Use <code>mulM</code> for actual matrix-matrix multiplication. If <code>out</code> is not given, writes result in <code>a</code>.<!-- -->out = a \* b |
|  [mul22](./matrices.mul22.md) |  |
|  [mul23](./matrices.mul23.md) |  |
|  [mul33](./matrices.mul33.md) |  |
|  [mul44](./matrices.mul44.md) |  |
|  [mulM](./matrices.mulm.md) | Multi-method. Performs matrix-matrix multiplication. If <code>out</code> is not given, writes result in <code>a</code>. |
|  [mulM22](./matrices.mulm22.md) | 2x2 matrix-matrix multiplication. If <code>out</code> is not given, writes result in <code>a</code>. |
|  [mulM23](./matrices.mulm23.md) | 2x3 matrix-matrix multiplication. If <code>out</code> is not given, writes result in <code>a</code>. |
|  [mulM33](./matrices.mulm33.md) | 3x3 matrix-matrix multiplication. If <code>out</code> is not given, writes result in <code>a</code>. |
|  [mulM44](./matrices.mulm44.md) | 4x4 matrix-matrix multiplication. If <code>out</code> is not given, writes result in <code>a</code>. |
|  [mulN](./matrices.muln.md) | Multiplies matrix componentwise with single scalar. If <code>out</code> is not given, writes result in <code>mat</code>.<!-- -->out = mat \* n |
|  [mulN22](./matrices.muln22.md) |  |
|  [mulN23](./matrices.muln23.md) |  |
|  [mulN33](./matrices.muln33.md) |  |
|  [mulN44](./matrices.muln44.md) |  |
|  [mulQ](./matrices.mulq.md) | Performs quaternion multiplication of <code>a</code> and <code>b</code> and writes result to <code>out</code>. If <code>out</code> is null, writes result into <code>a</code>. |
|  [mulV](./matrices.mulv.md) | Matrix-vector multiplication. Supports in-place modification, i.e. if <code>out === v</code>. |
|  [mulV22](./matrices.mulv22.md) | Multiplies 2x2 matrix <code>m</code> with 2D vector <code>v</code>. Supports in-place modification, i.e. if <code>out === v</code>. |
|  [mulV23](./matrices.mulv23.md) | Multiplies 2x3 matrix <code>m</code> with 2D vector <code>v</code>. Supports in-place modification, i.e. if <code>out === v</code>. |
|  [mulV33](./matrices.mulv33.md) | Multiplies 3x3 matrix <code>m</code> with 3D vector <code>v</code>. Supports in-place modification, i.e. if <code>out === v</code>. |
|  [mulV344](./matrices.mulv344.md) | Multiplies 4x4 matrix <code>m</code> with 3D vector <code>v</code> and assumes <code>w=1</code>, i.e. the vector is interpreted as <code>[x,y,z,1]</code>. After transformation applies perspective divide of the resulting XYZ components. |
|  [mulV44](./matrices.mulv44.md) | Multiplies 4x4 matrix <code>m</code> with 4D vector <code>v</code>. Supports in-place modification, i.e. if <code>out === v</code>. |
|  [mulVM22](./matrices.mulvm22.md) | Same as:
```ts
out[0] = dot(v, column(m, 0))
out[1] = dot(v, column(m, 1))

```
 |
|  [mulVM23](./matrices.mulvm23.md) |  |
|  [mulVM33](./matrices.mulvm33.md) | Same as:
```ts
out[0] = dot(v, column(m, 0))
out[1] = dot(v, column(m, 1))
out[2] = dot(v, column(m, 2))

```
 |
|  [mulVM44](./matrices.mulvm44.md) | Same as:
```ts
out[0] = dot(v, column(m, 0))
out[1] = dot(v, column(m, 1))
out[2] = dot(v, column(m, 2))
out[3] = dot(v, column(m, 3))

```
 |
|  [mulVQ](./matrices.mulvq.md) | Multiplies quaternion <code>q</code> with 3D vector <code>v</code>. Returns transformed vector or modifies in-place if <code>out</code> is null or <code>v</code>. |
|  [normal33](./matrices.normal33.md) | Converts given 4x4 matrix to a 3x3 normal matrix, i.e. the transposed inverse of its upper-left 3x3 region. If <code>out</code> is null a new result matrix will be created. Returns <code>undefined</code> if matrix inversion failed. |
|  [normal44](./matrices.normal44.md) | Converts given 4x4 matrix to a 4x4 matrix normal matrix, i.e. the transposed inverse. Writes results to <code>m</code> if <code>out</code> is null. Returns <code>undefined</code> if matrix inversion failed. |
|  [ortho](./matrices.ortho.md) | Creates a 4x4 matrix orthographic projection matrix and writes result to <code>out</code>. |
|  [outerProduct](./matrices.outerproduct.md) | Computes outer/tensor product of vectors <code>u</code> and <code>v</code>. Returns square matrix of same dimensions as vectors, e.g. 3x3 matrix for 3D vectors.[https://en.wikipedia.org/wiki/Outer\_product](https://en.wikipedia.org/wiki/Outer_product) |
|  [outerProduct2](./matrices.outerproduct2.md) |  |
|  [outerProduct3](./matrices.outerproduct3.md) |  |
|  [outerProduct4](./matrices.outerproduct4.md) |  |
|  [perspective](./matrices.perspective.md) | Creates a 4x4 matrix perspective projection matrix and writes result to <code>out</code>. |
|  [project](./matrices.project.md) | Transforms given point <code>p</code> (4D, homogeneous coordinates) with 4x4 matrix <code>mvp</code>, applies perspective divide and then transforms XY components with 2x3 matrix <code>view</code> matrix. Returns 3D vector. The result Z component can be used for depth sorting. |
|  [quatFromAxisAngle](./matrices.quatfromaxisangle.md) | Computes a quaternion representing the rotation <code>theta</code> around <code>axis</code>. |
|  [quatFromEuler](./matrices.quatfromeuler.md) | Constructs a quaternion from given rotation angles in specified <code>order</code>. |
|  [quatToAxisAngle](./matrices.quattoaxisangle.md) | Decomposes quaternion into <code>[axis, theta]</code> tuple. |
|  [quatToMat33](./matrices.quattomat33.md) | Converts quaternion into 3x3 matrix and writes result to <code>out</code>. |
|  [quatToMat44](./matrices.quattomat44.md) | Converts quaternion into 4x4 matrix with optional translation offset <code>t</code>, then writes result to <code>out</code>. |
|  [rotation22](./matrices.rotation22.md) | Constructs a 2x2 matrix rotation matrix for given <code>theta</code>. |
|  [rotation23](./matrices.rotation23.md) | Constructs a 2x3 matrix rotation matrix for given <code>theta</code>. |
|  [rotationAroundAxis33](./matrices.rotationaroundaxis33.md) | Constructs a 3x3 matrix representing a rotation of <code>theta</code> around <code>axis</code> and writes result to <code>out</code>. If <code>normalize</code> is true (default false), non-destructively first normalizes axis vector. |
|  [rotationAroundAxis44](./matrices.rotationaroundaxis44.md) | Constructs a 4x4 matrix representing a rotation of <code>theta</code> around <code>axis</code> and writes result to <code>out</code>. If <code>normalize</code> is true (default false), non-destructively first normalizes axis vector. |
|  [rotationX33](./matrices.rotationx33.md) | Constructs a 3x3 matrix X rotation matrix for given <code>theta</code>. |
|  [rotationX44](./matrices.rotationx44.md) | Constructs a 4x4 matrix X rotation matrix for given <code>theta</code>. |
|  [rotationY33](./matrices.rotationy33.md) | Constructs a 3x3 matrix Y rotation matrix for given <code>theta</code>. |
|  [rotationY44](./matrices.rotationy44.md) | Constructs a 4x4 matrix Y rotation matrix for given <code>theta</code>. |
|  [rotationZ33](./matrices.rotationz33.md) | Constructs a 3x3 matrix Z rotation matrix for given <code>theta</code>. |
|  [rotationZ44](./matrices.rotationz44.md) | Constructs a 4x4 matrix Z rotation matrix for given <code>theta</code>. |
|  [row](./matrices.row.md) | Extracts row vector from given matrix and writes result to <code>out</code>. If <code>out</code> is null, creates new vector. |
|  [row22](./matrices.row22.md) |  |
|  [row23](./matrices.row23.md) |  |
|  [row33](./matrices.row33.md) |  |
|  [row44](./matrices.row44.md) |  |
|  [scale22](./matrices.scale22.md) | Computes 2x2 matrix scale matrix and writes result to <code>out</code>. If <code>s</code> is a number, scaling will be uniform. |
|  [scale23](./matrices.scale23.md) | Computes 2x3 matrix scale matrix and writes result to <code>out</code>. If <code>s</code> is a number, scaling will be uniform. |
|  [scale33](./matrices.scale33.md) | Computes 3x3 matrix scale matrix and writes result to <code>out</code>. If <code>s</code> is a number, scaling will be uniform. |
|  [scale44](./matrices.scale44.md) | Computes 4x4 matrix scale matrix and writes result to <code>out</code>. If <code>s</code> is a number, scaling will be uniform. |
|  [scaleWithCenter23](./matrices.scalewithcenter23.md) | Computes a 2x3 matrix representing a scale operation with origin <code>p</code> and writes result to <code>out</code>. |
|  [scaleWithCenter44](./matrices.scalewithcenter44.md) | Computes a 4x4 matrix representing a scale operation with origin <code>p</code> and writes result to <code>out</code>. |
|  [set](./matrices.set.md) |  |
|  [set22](./matrices.set22.md) |  |
|  [set23](./matrices.set23.md) |  |
|  [set33](./matrices.set33.md) |  |
|  [set44](./matrices.set44.md) |  |
|  [shearX22](./matrices.shearx22.md) |  |
|  [shearX23](./matrices.shearx23.md) |  |
|  [shearXY33](./matrices.shearxy33.md) |  |
|  [shearXY44](./matrices.shearxy44.md) |  |
|  [shearXZ33](./matrices.shearxz33.md) |  |
|  [shearXZ44](./matrices.shearxz44.md) |  |
|  [shearY22](./matrices.sheary22.md) |  |
|  [shearY23](./matrices.sheary23.md) |  |
|  [shearYX33](./matrices.shearyx33.md) |  |
|  [shearYX44](./matrices.shearyx44.md) |  |
|  [shearYZ33](./matrices.shearyz33.md) |  |
|  [shearYZ44](./matrices.shearyz44.md) |  |
|  [shearZX33](./matrices.shearzx33.md) |  |
|  [shearZX44](./matrices.shearzx44.md) |  |
|  [shearZY33](./matrices.shearzy33.md) |  |
|  [shearZY44](./matrices.shearzy44.md) |  |
|  [skewX22](./matrices.skewx22.md) |  |
|  [skewX23](./matrices.skewx23.md) |  |
|  [skewXY33](./matrices.skewxy33.md) |  |
|  [skewXY44](./matrices.skewxy44.md) |  |
|  [skewXZ33](./matrices.skewxz33.md) |  |
|  [skewXZ44](./matrices.skewxz44.md) |  |
|  [skewY22](./matrices.skewy22.md) |  |
|  [skewY23](./matrices.skewy23.md) |  |
|  [skewYX33](./matrices.skewyx33.md) |  |
|  [skewYX44](./matrices.skewyx44.md) |  |
|  [skewYZ33](./matrices.skewyz33.md) |  |
|  [skewYZ44](./matrices.skewyz44.md) |  |
|  [skewZX33](./matrices.skewzx33.md) |  |
|  [skewZX44](./matrices.skewzx44.md) |  |
|  [skewZY33](./matrices.skewzy33.md) |  |
|  [skewZY44](./matrices.skewzy44.md) |  |
|  [sub](./matrices.sub.md) | Componentwise matrix subtraction. If <code>out</code> is not given, writes result in <code>a</code>.<!-- -->out = a - b |
|  [sub22](./matrices.sub22.md) |  |
|  [sub23](./matrices.sub23.md) |  |
|  [sub33](./matrices.sub33.md) |  |
|  [sub44](./matrices.sub44.md) |  |
|  [subN](./matrices.subn.md) | Subtracts matrix componentwise with single scalar. If <code>out</code> is not given, writes result in <code>mat</code>.<!-- -->out = mat - n |
|  [subN22](./matrices.subn22.md) |  |
|  [subN23](./matrices.subn23.md) |  |
|  [subN33](./matrices.subn33.md) |  |
|  [subN44](./matrices.subn44.md) |  |
|  [trace](./matrices.trace.md) | Returns matrix trace of <code>m</code>, i.e. component sum of <code>diag(m)</code>. |
|  [transform23](./matrices.transform23.md) | Creates 2x3 TRS transformation matrix from given translation vector, rotation angle and scale factor/vector. |
|  [transform44](./matrices.transform44.md) | Creates 4x4 TRS transformation matrix from given translation vector, rotation angles (given as 3D vector) and scale factor/vector. Internally, uses a quaternion for constructing the rotation matrix part. The quaternion is created via <code>quatFromEuler()</code> with ZYX ordering. |
|  [translation23](./matrices.translation23.md) | Constructs a 2x3 translation matrix. |
|  [translation44](./matrices.translation44.md) | Constructs a 4x4 translation matrix. |
|  [transpose22](./matrices.transpose22.md) | Writes transposition of 2x2 matrix <code>m</code> to <code>out</code>. Creates new matrix if <code>out</code> is <code>null</code> |
|  [transpose33](./matrices.transpose33.md) | Writes transposition of 3x3 matrix <code>m</code> to <code>out</code>. Creates new matrix if <code>out</code> is <code>null</code> |
|  [transpose44](./matrices.transpose44.md) | Writes transposition of 4x4 matrix <code>m</code> to <code>out</code>. Creates new matrix if <code>out</code> is <code>null</code> |
|  [unproject](./matrices.unproject.md) | Reverse operation of <code>project()</code>. If <code>invert</code> is true (default: false), both <code>mvp</code> and <code>view</code> matrices will be inverted first (non-destructively), else they're both assumed to be inverted already. |
|  [viewport](./matrices.viewport.md) | Produces a 2x3 viewport matrix to transform projected coordinates to screen space. |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [IMatrix](./matrices.imatrix.md) |  |
|  [Mat](./matrices.mat.md) |  |
|  [Mat22Like](./matrices.mat22like.md) |  |
|  [Mat23Like](./matrices.mat23like.md) |  |
|  [Mat33Like](./matrices.mat33like.md) |  |
|  [Mat44Like](./matrices.mat44like.md) |  |
|  [MatOp1](./matrices.matop1.md) |  |
|  [MatOpM](./matrices.matopm.md) |  |
|  [MatOpMM](./matrices.matopmm.md) |  |
|  [MatOpMN](./matrices.matopmn.md) |  |
|  [MatOpMU](./matrices.matopmu.md) |  |
|  [MatOpMV](./matrices.matopmv.md) |  |
|  [MatOpN](./matrices.matopn.md) |  |
|  [MultiMatOp](./matrices.multimatop.md) |  |
|  [ReadonlyMat](./matrices.readonlymat.md) |  |
|  [VecOpM](./matrices.vecopm.md) |  |
|  [VecOpMN](./matrices.vecopmn.md) |  |
