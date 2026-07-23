# QuietBar Changelog

## 1.0 build 6 - Release Candidate

### Added

- One-click reveal and compact behavior for menu bar items.
- Application name and icon recognition with optional Accessibility access.
- Duplicate application-item grouping and live refresh.
- First-run setup guidance and settings panel.
- Launch-at-login support.
- Configurable automatic compact delay.
- `Control-Option-Q` global shortcut.
- English and Simplified Chinese interfaces.
- App Sandbox configuration for Mac App Store distribution.
- Product website, interactive browser demonstration, App Preview, privacy
  policy, support documentation, and localized store screenshots.

### Fixed

- Accessibility permission state now follows the result returned by the actual
  background scan instead of a stale UI-thread value.
- Inherited duplicate items are omitted when a directly recognized item for the
  same application is available.
- The Mac App Store configuration includes the Accessibility sandbox
  entitlement required for local app-name and icon scanning.
- Chinese product copy consistently uses the name 悄悄吧.
- Store screenshots show the correct product name and build number.

### Verified

- 24 unit tests pass.
- The signed build 6 archive contains both App Sandbox and Accessibility
  entitlements.
- The archive contains Apple silicon and Intel architectures.
- The final app bundle excludes obsolete brand candidates and generated build
  artifacts.

### Public Availability

- The notarized Developer ID package is available in the
  [v1.0-build6 GitHub Release](https://github.com/Jorgut/QuietBar-Releases/releases/tag/v1.0-build6).
- SHA-256 verification is provided as `SHA256SUMS.txt` in the release.

### Pending for Mac App Store Availability

- Install and exercise the archived Sandbox build with Accessibility disabled,
  newly granted, and revoked.
- Complete full-screen, notch, multi-display, login-start, and older macOS
  runtime checks.
- Upload build 6 and complete App Store review submission.

## 1.0 build 5 - Superseded

Build 5 was uploaded to App Store Connect on July 23, 2026. It was superseded
before review submission by build 6, which adds the required Sandbox
Accessibility entitlement.
