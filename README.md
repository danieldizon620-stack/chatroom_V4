# ASDI Android v3.33 — Mobile Messenger UI

This source project adapts the existing ASDI Chatroom to the supplied phone messenger screenshot:
- A single full-width conversation (no compressed three-column grid).
- Compact white conversation header and floating Groups/Users buttons.
- Groups and Users slide in as drawers; chat remains readable on narrow screens.
- Smaller message bubbles, spacing and rounded input composer.
- Ticketing navigation remains hidden by the v3.32 logic.
- Retains existing ticket/chat notification polling while app is active.

## Build and install
Build the Android APK using the GitHub Actions workflow in `.github/workflows/build_apk.yml`.
The ZIP is Android source, not a compiled APK. An update over an existing app requires the same signing certificate.

**Limitations:** Screenshot-inspired layout is implemented as WebView-injected CSS and JavaScript. This is not a native redesign. Not compiled or tested on a physical device. Colors and sizing may vary depending on the server's live HTML and CSS.
