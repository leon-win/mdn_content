---
title: "CSSTransformComponent: toMatrix() method"
short-title: toMatrix()
slug: Web/API/CSSTransformComponent/toMatrix
page-type: web-api-instance-method
browser-compat: api.CSSTransformComponent.toMatrix
---

{{APIRef("CSS Typed OM")}}

The **`toMatrix()`** method of the
{{domxref("CSSTransformComponent")}} interface returns a {{domxref('DOMMatrix')}}
object.

All transform functions can be represented mathematically as a 4x4 transformation matrix.

> [!NOTE]
> The `is2D` property affects what transform, and therefore type of matrix that will be returned. CSS 2D and 3D transforms are different for legacy reasons. A brief explanation of 2D vs. 3D transforms can be found in [Using CSS transforms](/en-US/docs/Web/CSS/CSS_transforms/Using_CSS_transforms).

## Syntax

```js-nolint
toMatrix()
```

### Parameters

None.

### Return value

A {{domxref('DOMMatrix')}} object

### Exceptions

- {{jsxref("TypeError")}}
  - : Raised if any lengths involved in generating the matrix are not compatible units
    with px (such as relative lengths or percentages).

## Examples

To Do

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
