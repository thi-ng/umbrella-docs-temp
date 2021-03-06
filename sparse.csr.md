<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/sparse](./sparse.md) &gt; [CSR](./sparse.csr.md)

## CSR class

<b>Signature:</b>

```typescript
export declare class CSR extends ASparseMatrix 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(m, n, data, rows, cols)](./sparse.csr._constructor_.md) |  | Constructs a new instance of the <code>CSR</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [cols](./sparse.csr.cols.md) |  | <code>number[]</code> | Column indices for values in A |
|  [data](./sparse.csr.data.md) |  | <code>number[]</code> | Non-zero matrix values |
|  [rows](./sparse.csr.rows.md) |  | <code>number[]</code> | Row start indices into A |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [add(mat)](./sparse.csr.add.md) |  |  |
|  [at(m, n, safe)](./sparse.csr.at.md) |  |  |
|  [copy()](./sparse.csr.copy.md) |  |  |
|  [denseCol(n)](./sparse.csr.densecol.md) |  |  |
|  [denseRow(m)](./sparse.csr.denserow.md) |  |  |
|  [diag(vals)](./sparse.csr.diag.md) | <code>static</code> |  |
|  [empty(m, n)](./sparse.csr.empty.md) | <code>static</code> |  |
|  [extract(m, n, rows, cols)](./sparse.csr.extract.md) |  |  |
|  [fromDense(m, n, dense)](./sparse.csr.fromdense.md) | <code>static</code> | Constructs CSR from dense row-major matrix values. |
|  [identity(size)](./sparse.csr.identity.md) | <code>static</code> |  |
|  [mul(mat)](./sparse.csr.mul.md) |  |  |
|  [mulN(n)](./sparse.csr.muln.md) |  |  |
|  [mulV(vec)](./sparse.csr.mulv.md) |  |  |
|  [nnz()](./sparse.csr.nnz.md) |  |  |
|  [nnzCol(n)](./sparse.csr.nnzcol.md) |  |  |
|  [nnzRow(m)](./sparse.csr.nnzrow.md) |  |  |
|  [nzColRows(n)](./sparse.csr.nzcolrows.md) |  |  |
|  [nzColVals(n)](./sparse.csr.nzcolvals.md) |  |  |
|  [nzEntries()](./sparse.csr.nzentries.md) |  |  |
|  [nzRowCols(m)](./sparse.csr.nzrowcols.md) |  |  |
|  [nzRowVals(m)](./sparse.csr.nzrowvals.md) |  |  |
|  [reshape(m, n)](./sparse.csr.reshape.md) |  |  |
|  [setAt(m, n, x, safe, compact)](./sparse.csr.setat.md) |  |  |
|  [sub(mat)](./sparse.csr.sub.md) |  |  |
|  [toDense()](./sparse.csr.todense.md) |  |  |
|  [toString()](./sparse.csr.tostring.md) |  |  |
|  [transpose()](./sparse.csr.transpose.md) |  |  |
|  [zero()](./sparse.csr.zero.md) |  |  |

