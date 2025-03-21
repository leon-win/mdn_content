---
title: "DOMPointReadOnly: y property"
short-title: y
slug: Web/API/DOMPointReadOnly/y
page-type: web-api-instance-property
browser-compat: api.DOMPointReadOnly.y
---

{{APIRef("Geometry Interfaces")}}{{AvailableInWorkers}}

The **`DOMPointReadOnly`** interface's
**`y`** property holds the vertical coordinate, y, for a
read-only point in space.

If your script needs to be able to change the value
of this property, you should instead use the {{domxref("DOMPoint")}} object.

In general, positive values of `y` mean downward, and negative values of
`y` mean upward, assuming no transforms have resulted in a reversal.

## Value

A double-precision floating-point value indicating the y coordinate's value for the
point. This value is **unrestricted**, meaning that it is allowed to be
infinite or invalid (that is, its value may be {{jsxref("NaN")}} or {{jsxref("Infinity", "±Infinity")}}).

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The other coordinate properties: {{domxref("DOMPointReadOnly.x", "x")}},
  {{domxref("DOMPointReadOnly.z", "z")}}, and the perspective value,
  {{domxref("DOMPointReadOnly.w", "w")}}.
