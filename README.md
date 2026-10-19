# ASDI Chatroom Android v3.37 — Chrome layout parity

This is an Android **source project**, not a compiled APK.

- Requires ASDI Ticketing server **v3.32 or newer** for the Chrome layout, hidden floating Chatroom button, and hidden footer.
- Uses the server's responsive chatroom design without injecting Bootstrap or overriding chat bubbles, attachments, or Send bar.
- Hides the website's ticketing navigation; opens chatroom after login.
- Keeps chat/ticket notifications while app is active (requires the existing mobile notification PHP endpoints on the server).
- Keeps existing app ID `com.asdi.chatroom`, versionCode 337.

## Build APK using GitHub Actions
Upload the project contents (including `.github/workflows/build_apk.yml`) to a GitHub repository. Under Actions, run **Build ASDI Chatroom v3.37 APK**. Download artifact **ASDI-Chatroom-v3.37-APK**, containing `app-debug.apk`.

The build environment here lacks the Android SDK/Gradle, so an installable APK cannot be produced or tested here. Installing over an existing app requires the same signing certificate. Debug APKs built on different runners may not share the same certificate.
