# ASDI Chatroom Android v3.39 — Edge-to-edge approved preview

Android source project for building an installable APK. The layout uses the live ASDI Ticketing v3.32+ Chrome chatroom and removes the 10px invisible border from v3.38.

- Full phone-width chatroom, no centered narrow frame
- No dashboard/tool navigation, footer or floating Chatroom shortcut
- Keeps Groups, Users, chat background, message bubbles and bottom Send bar
- After login opens chatroom.php
- Preserves existing notification polling while the app is active

## Build
1. Upload the extracted project to a GitHub repository.
2. Run **Actions > Build ASDI Chatroom v3.39 APK**.
3. Download artifact **ASDI-Chatroom-v3.39-APK** containing app-debug.apk.

Install the ASDI Ticketing v3.32 server update first. Existing Android upgrades need the same signing certificate; a fresh GitHub debug key may not match the old APK.

This is source code, not a compiled APK. Build and phone testing were not possible in this environment. The rendered preview is a design target, not a verified screenshot of the compiled app.
