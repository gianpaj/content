---
title: Firefox 97 for developers
slug: Mozilla/Firefox/Releases/97
tags:
  - '97'
  - Firefox
  - Mozilla
  - Release
---
{{FirefoxSidebar}}{{draft}}

This article provides information about the changes in Firefox 97 that will affect developers. Firefox 97 is the current [Beta version of Firefox](https://www.mozilla.org/en-US/firefox/channel/desktop/#beta), and will ship on [February 8, 2022](https://wiki.mozilla.org/RapidRelease/Calendar#Future_branch_dates).

## Changes for web developers

### Developer Tools

### HTML

#### Removals

### CSS

#### Removals

### JavaScript

#### Removals

### HTTP

#### Removals

### Security

#### Removals

### APIs

#### DOM

- The reason for an abort signal can now be set using {{domxref("AbortController.abort()")}} (or {{domxref("AbortSignal.abort()")}}), and will be available in the {{domxref("AbortSignal.reason")}} property.
  This reason defaults to being an "AbortError" {{domxref("DOMException")}}.
  The reason can be thrown or handled via promise rejection as appropriate.
  ({{bug(1737771)}}).
- The convenience method {{domxref("AbortSignal.throwIfAborted()")}} can be used to check if a signal has been aborted, and if so throw the {{domxref("AbortSignal.reason()")}}.
  This makes it easier for developers to handle abort signals in code where you can't simply pass the signal to an abortable method. ({{bug(1745372)}}).

#### Media, WebRTC, and Web Audio

#### Removals

### WebAssembly

#### Removals

### WebDriver conformance (Marionette)

#### Removals

## Changes for add-on developers

- `cookieStoreId` in {{WebExtAPIRef("tabs.query")}} supports an array of strings. This enables queries to match tabs against more than one cookie store ID ({{bug(1730931)}}).
- `cookieStoreId` added to {{WebExtAPIRef("contentScripts.register")}}. This enables extensions to register container-specific content scripts ({{bug(1470651)}}).

#### Removals

### Other

## Older versions

{{Firefox_for_developers(96)}}
