---
title: "Location: host property"
short-title: host
slug: Web/API/Location/host
page-type: web-api-instance-property
browser-compat: api.Location.host
---

{{ApiRef("Location")}}

The **`host`** property of the {{domxref("Location")}} interface is a string containing the host, which is the {{domxref("Location.hostname", "hostname")}}, and then, if the {{glossary("port")}} of the URL is nonempty, a `":"`, followed by the {{domxref("Location.port", "port")}} of the URL. If the URL does not have a `hostname`, this property contains an empty string, `""`.

See {{domxref("URL.host")}} for more information.

## Value

A string.

## Examples

```js
const anchor = document.createElement("a");

anchor.href = "https://developer.mozilla.org/en-US/Location.host";
console.log(anchor.host === "developer.mozilla.org");

anchor.href = "https://developer.mozilla.org:443/en-US/Location.host";
console.log(anchor.host === "developer.mozilla.org");
// The port number is not included because 443 is the scheme's default port

anchor.href = "https://developer.mozilla.org:4097/en-US/Location.host";
console.log(anchor.host === "developer.mozilla.org:4097");
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
