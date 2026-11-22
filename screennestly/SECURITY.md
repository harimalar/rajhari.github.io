# ScreenNestly Security Policy

Updated November 21, 2026 · Maintainer: Hari Rajagopalan

## Report privately

Send suspected vulnerabilities to **[rajhari@gmail.com](mailto:rajhari@gmail.com?subject=ScreenNestly%20security%20report)** with the subject "ScreenNestly security report." Do not post exploitable details or sensitive screenshots in a public GitHub issue.

Include the app and macOS versions, a clear description, impact, and minimal steps to reproduce using synthetic content. Do not attach passwords, access tokens, real customer records, or someone else's private files. Contact us first if a report needs sensitive material; ordinary email is not a secure file vault.

Reports are reviewed and coordinated privately. No fixed response deadline, bounty, or legal immunity is promised. Test only devices and files you own or are authorized to test, avoid destructive tests, and allow time for a fix before public disclosure. The latest released version is the primary maintenance target; older versions are not guaranteed separate patches.

## Security model and limits

ScreenNestly uses the macOS app sandbox, user-selected folder access, and system-managed capture, optional microphone, and optional Accessibility permissions. OCR runs on the device. The app has no account, cloud service, remote-control endpoint, advertising, analytics, or automatic capture upload.

The local library includes MP4 recordings (and enabled audio), original images and recognized text as well as edited renders. Audio options start off for every recording. Failed recordings may remain locally for recovery. It is not a separately encrypted or password-protected vault. Protect your Mac account and backups; use macOS security features such as FileVault where appropriate. Solid Redact affects the shared render, while the original remains locally editable.

Sharing through the clipboard, drag-and-drop, exports, email, or folders managed by another service moves copies outside the app's control. Keep settings backups private: they can contain paths and folder-access bookmarks. See the [Privacy Policy](PRIVACY.md) for storage, temporary copies, retention, and deletion details.

## Dependency and release checks

ScreenNestly uses Apple's system frameworks and the pinned KeyboardShortcuts package. Its MIT notice is included in the app. Release checks cover image persistence, file-operation rollback, redaction output, transfer snapshots, scrolling alignment, and recording persistence and lifecycle behavior. Passing those checks does not eliminate all security risks. Distribution signing and App Store review must be completed before a public App Store release.
