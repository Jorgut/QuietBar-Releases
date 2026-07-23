# QuietBar Support

## The QuietBar Icon Does Not Appear

1. Confirm QuietBar is running.
2. Open **System Settings > Control Center > Menu Bar Only** and verify macOS
   allows QuietBar to appear.
3. Quit and reopen QuietBar.
4. If the problem continues, include your macOS version, Mac model, and a
   privacy-safe screenshot in a GitHub Issue.

## Items Do Not Compact

Reveal QuietBar first. Hold `Command`, then drag the items you want to compact
to the left of the QuietBar divider. Fixed system items such as the clock remain
visible.

## Names or Application Icons Are Missing

Open **System Settings > Privacy & Security > Accessibility** and enable
QuietBar, then return to QuietBar and refresh.

If QuietBar was already enabled:

1. Disable or remove QuietBar from the Accessibility list.
2. Quit QuietBar.
3. Reopen it and grant access again.
4. Refresh the panel.

Some system helpers and third-party apps do not provide enough metadata for a
stable name or icon. QuietBar may show a fallback icon or omit an unstable
duplicate. Basic reveal and compact behavior does not require this metadata.

## The Global Shortcut Does Not Work

Confirm the global shortcut is enabled in QuietBar settings, then press
`Control-Option-Q` (`⌃⌥Q`). If another app uses the same shortcut, mention that
app in your report.

## Launch at Login Does Not Work

Open **System Settings > General > Login Items & Extensions** and confirm
QuietBar is allowed to open at login. macOS may require a second confirmation
there.

## Restore the Full Menu Bar Temporarily

Quit QuietBar. Its divider is removed by macOS, so it no longer occupies menu
bar space.

## Reporting a Problem

Create a GitHub Issue and include:

- QuietBar version and build number;
- full macOS version;
- Mac model and processor;
- number and arrangement of displays;
- whether a notch or full-screen Space is involved;
- reproducible steps, expected result, and actual result;
- screenshots or recordings with private content removed.

Do not upload passwords, private notifications, personal documents, crash logs
containing private paths, or other sensitive information.

For privacy or store questions, email [honaler@gmail.com](mailto:honaler@gmail.com).
