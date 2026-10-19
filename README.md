# ASDI Android v3.32 — Ticketing navigation removal fix

The screenshot shows the server-rendered `header.top` / `nav.nav.asdi-nav-clean` menu (Dashboard, Tickets, Ticket Management, Customers & Services, Inventory & Tracking, Tools, My Profile, Logout) above Chatroom. Earlier CSS only matched navigation as a direct child of `body`, so it missed menus wrapped in another element.

This version hides the exact shared header and navigation using descendant CSS selectors **and** removes their display via a chatroom-only JavaScript pass. It keeps Groups, Conversation and Users controls. It also expands the chatroom to the phone viewport. After authentication the WebView opens chatroom.php, not the dashboard.

## Build and install
Upload the Android project to GitHub, run the workflow in `.github/workflows/build_apk.yml`, and install the built APK. You must actually install **v3.32**; merely updating PHP does not update the APK. A replacement install needs the same signing certificate as your installed app. On some devices, uninstalling an old debug-signed app may be required and can clear app-local data.

No PHP System Upgrade is required. Server must run current ASDI Ticketing. Chat/ticket notifications continue to require the PHP endpoints included in `server/` and currently poll only while the app is active.

This ZIP is Android **source**, not a compiled APK. ZIP integrity checked; Android compilation and physical-device display are not tested.
