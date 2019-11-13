<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/errors](./errors.md) &gt; [IllegalStateError](./errors.illegalstateerror.md)

## IllegalStateError variable

<b>Signature:</b>

```typescript
IllegalStateError: {
    new (msg?: any): {
        name: string;
        message: string;
        stack?: string | undefined;
    };
    captureStackTrace(targetObject: Object, constructorOpt?: Function | undefined): void;
    prepareStackTrace?: ((err: Error, stackTraces: NodeJS.CallSite[]) => any) | undefined;
    stackTraceLimit: number;
}
```