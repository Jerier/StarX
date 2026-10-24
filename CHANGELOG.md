# Changelog

## 1.0.0

First public release.

### Features
- Screen color controls: saturation, vibrance, brightness, gamma, contrast,
  temperature, highlights, shadows, hue, vignette, dim and night mode, with
  presets and per-game profiles.
- NVIDIA digital vibrance, applied per display.
- Rust helper: launch options, graphics preset, FPS limit and a resolution
  switch on launch, with a target-display picker.
- Crosshair overlay with built-in shapes or your own image.
- Sound lock that caps system volume while you play.
- Color-filtered screenshots (Ctrl+Alt+S), saved to Pictures\StarX and copied
  to the clipboard. Ctrl+Alt+R resets color.
- Optional FPS boost and Windows performance tweaks, each restored when turned
  off.
- Tray icon, start with Windows, start minimized, close to tray.
- One-file installer (StarX-Setup.exe) with an uninstaller, an entry in
  Settings > Apps and the Start Menu. The uninstaller asks whether to keep your
  settings.

### Safety and recovery
- StarX remembers the original display, vibrance, power plan, volume and
  registry values and restores them on exit, on crash, and on the next start
  if a previous run was interrupted. `StarX.exe --reset` restores display state.
- Settings are written atomically, backed up, and recovered from the backup
  if the main file is damaged. Unknown or hand-typed settings keys are kept.
- Steam and Rust config edits refuse to run when the active account is
  ambiguous or Rust is running, keep a one-time backup, and verify the write.

### Installer and release
- Per-user install by default, with a Windows prompt only if you pick a
  machine-wide install.
- A failed install rolls back, and an older Setup warns before replacing a
  newer install. A running StarX is asked to exit cleanly first.
- Each release ships a SHA-256 checksum next to the download. The exe is not
  code-signed, so Windows SmartScreen may warn.

### Licensing
- Access key from the StarX Discord. A signed remote status file can disable
  StarX; an unreachable or invalid status never blocks a licensed install.
