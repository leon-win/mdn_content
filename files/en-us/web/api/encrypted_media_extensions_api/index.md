---
title: Encrypted Media Extensions API
slug: Web/API/Encrypted_Media_Extensions_API
page-type: web-api-overview
browser-compat: api.Navigator.requestMediaKeySystemAccess
---

{{DefaultAPISidebar("Encrypted Media Extensions")}} {{securecontext_header}}

The **Encrypted Media Extensions API** provides interfaces for controlling the playback of content which is subject to a digital restrictions management scheme.

Access to this API is provided through {{domxref("Navigator.requestMediaKeySystemAccess()")}}.

## Interfaces

- {{domxref("MediaEncryptedEvent")}}
  - : Represents a specific {{domxref("HTMLMediaElement/encrypted_event", "encrypted")}} event thrown when a {{domxref('HTMLMediaElement')}} encounters some initialization data.
- {{domxref("MediaKeyMessageEvent")}}
  - : Contains the content and related data when the content decryption module (CDM) generates a message for the session.
- {{domxref("MediaKeys")}}
  - : Represents a set of keys that an associated {{domxref('HTMLMediaElement')}} can use for decryption of media data during playback.
- {{domxref("MediaKeySession")}}
  - : Represents a context for message exchange with a content decryption module (CDM).
- {{domxref("MediaKeyStatusMap")}}
  - : A read-only map of media key statuses by key IDs.
- {{domxref("MediaKeySystemAccess")}}
  - : Provides access to a key system for decryption and/or a content protection provider.

### Extensions to other interfaces

The Encrypted Media Extensions API extends the following APIs, adding the listed features.

#### HTMLMediaElement

- {{domxref("HTMLMediaElement.mediaKeys")}} {{readonlyinline}}
  - : Provides a {{domxref("MediaKeys")}} object that represents the set of keys that the element can use for decryption of media data during playback.
- {{domxref("HTMLMediaElement.setMediaKeys()")}}
  - : Sets the {{domxref("MediaKeys")}} that will be used to decrypt media during playback.
- [`encrypted` event](/en-US/docs/Web/API/HTMLMediaElement/encrypted_event)
  - : Event that is fired on a {{domxref("HTMLMediaElement")}} when initialization data is encountered in the media, indicating that it is encrypted.

#### Navigator

- {{domxref("Navigator.requestMediaKeySystemAccess()")}}
  - : Returns a {{jsxref('Promise')}} that fulfils to a {{domxref('MediaKeySystemAccess')}} object that can be used to access a particular media key system, which can in turn be used to create keys for decrypting a media stream.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
