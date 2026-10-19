# ASDI Android v3.36 — Composer and Attachment Menu Fix

Android source project (not a compiled APK).

- Replaces the previous 90%-zoom / 111%-width workaround that could cause horizontal overflow.
- Fits the entire composer on one row: Attach, Emoji, Message field, **Send**.
- Keeps messages scrollable in the remaining space; one mobile chat layout.
- Closes attachment menu when tapping outside, focusing message input, opening emojis, submitting, or pressing Escape.
- Preserves the existing server's send-message handler, photo/file picker, and ASDI chat features.
- Retains dashboard navigation hiding and active-app notifications.

Build with the included GitHub Actions workflow; install the resulting APK. Existing app upgrades require the same signing certificate.

ZIP integrity checked; Android compilation and phone testing not performed. The server's current markup and styles can affect final behavior.
