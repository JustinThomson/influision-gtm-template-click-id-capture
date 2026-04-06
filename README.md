# Influise - Click ID Capture

This Google Tag Manager template reads the `clid` URL parameter from any page view and stores it in a 1-year persistent cookie named `influise_clid`. This enables influencer tracking and last-click attribution for conversions.

## Features

- Reads `clid` query parameter from the URL.
- Stores in cookie valid for 1 year (`SameSite=Lax`).
- Automatically overwrites old cookie on new tracking links.
- Works across all pages; no per-influencer setup required.

## Installation

1. Import this template into your GTM container.
2. Add the tag **“Influise - Click ID Capture”** with trigger **All Pages**.
3. Save and publish.

## Example

Visitor lands on:

https://example.com/?clid=1234

The tag will store a cookie:

Name: influise_clid
Value: 1234
Path: /
Max-age: 31536000
SameSite: Lax

No further configuration is required.

## License

Apache License 2.0  
http://www.apache.org/licenses/