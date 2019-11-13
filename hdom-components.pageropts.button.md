<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/hdom-components](./hdom-components.md) &gt; [PagerOpts](./hdom-components.pageropts.md) &gt; [button](./hdom-components.pageropts.button.md)

## PagerOpts.button() method

Function producing a single page nav or counter element. MUST be provided by user.

The function is called with:

- target page ID - current page ID - max pageID - page label (page number or sourced from these options here) - disabled flag as determined by the pager

If `disabled` is true, the function should return a version of the button component reflecting this state to the user. E.g. the "prev page" buttons should be disabled if the first page is currently active. Likewise, the currently selected page button will be set to disabled as well.

Page IDs are zero-based indices, whereas page number labels are one-based. The currently active page ID is only provided for special highlighting cases (optional).

<b>Signature:</b>

```typescript
button(page: number, curr: number, max: number, label: any, disabled: boolean): any;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  page | <code>number</code> |  |
|  curr | <code>number</code> |  |
|  max | <code>number</code> |  |
|  label | <code>any</code> |  |
|  disabled | <code>boolean</code> |  |

<b>Returns:</b>

`any`
