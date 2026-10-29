# Release testing

Version: v1.0.0-beta.1, build 10016, Apple Silicon.

- The app and DMG are Developer ID signed, notarized, and stapled. Keep Gatekeeper enabled.
- The frozen DMG was installed on a clean macOS 13.4.1 Apple Silicon VM without Homebrew or Xcode. It uses the embedded Python 3.12.13 runtime.
- A real Sparkle update from build 10013 to 10016 installed and relaunched the app. Language, interval settings, existing records, and disabled paid requests were preserved.
- Program rollback retained records created after the update. Normal Quit stopped app-owned workers; reopening retained the selected language.
- English and Simplified Chinese were checked through the real app. Selecting English, quitting normally, and reopening also switched Sparkle dialogs to English.
- The desktop copy was run on macOS 27.0.1 with a real local Codex quota reading. Messages, quota, costs, settings, and scrolling were exercised in the app.
- 70 native regression tests passed on the final source. The 364 embedded-Python tests were reused because all packaged Python scripts and reference files are unchanged from that tested input.
- Current update signatures, a damaged archive, and an incorrect signature were checked with the actual Sparkle tools. Cancellation, an unreachable update source, and a read-only installation were checked in the VM with the unchanged updater implementation. Low-space handling used boundary inputs; the test did not fill a real disk.

Paid provider generation and actual billing were not performed. Those paths used offline substitutes. No complete OS, Intel, Codex-protocol, or provider compatibility matrix is claimed. The WebKit developer console was not captured separately; the key app flows were exercised directly.

The preview image uses synthetic records. Live account screenshots, authentication files, credentials, and operating data are not published in this repository.
