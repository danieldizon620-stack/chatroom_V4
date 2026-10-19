# ASDI Android v3.34 — Bootstrap 5 responsive mobile UI

This is an Android WebView **source project**, not a compiled APK.

- Loads Bootstrap 5.3.3 CSS from jsDelivr **only on the chatroom page**, with local responsive CSS fallback when the CDN is unavailable. An internet connection is needed to load Bootstrap itself.
- Uses Bootstrap 5 utility classes for the chatroom container and conversation. Existing server-rendered ASDI markup is retained.
- Responsive layout for OPPO Reno 15 5G and other Android screens using viewport-based widths instead of fixed physical pixels.
- Keeps Groups and Users as slide-out drawers and Chatroom full screen.
- Adjusts the keyboard resize behavior (`adjustResize`), bubble sizes, ASDI stickers, header, and message composer.
- Retains chat/ticket polling while the app is open.

Build with the included GitHub Actions workflow, then install the resulting APK. Existing app updates require the same signing certificate. This project has not been compiled or tested on a physical Android phone.

**Important:** Bootstrap cannot automatically make a PHP WebView application fully native. The mobile layout relies on targeted CSS and JS and may need adjustments if your server HTML changes.
