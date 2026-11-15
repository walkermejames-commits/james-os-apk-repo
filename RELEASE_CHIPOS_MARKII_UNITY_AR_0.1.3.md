# ChipOS Mark II Unity AR 0.1.3

- Experimental Android ARM64 APK built with Unity 6000.6.5f1.
- Android package version: `0.1.3` / version code `3`.
- APK size: 222,650,593 bytes.
- SHA-256: `45C97467882B5818974F973B8854E6E90FE9A0DC33B38F202E1462CE767F20CE`.
- Unity Android build succeeded with 0 errors and 71 warnings.
- Unity EditMode suite: 43 passed, 0 failed. Includes a startup UI check for transparent overlay, visible mapping/microphone/caption-placement buttons, and a collapsed workspace.
- APK inspection confirms package `com.walkermejames.chiposmarkii`, ARM64, min API 31, target API 36, and `CAMERA`/`RECORD_AUDIO` permissions. APK v2 signature verifies with the established experimental Android test certificate.

## Changes

- Replaced the full-screen opaque studio surface with a short, translucent bottom dock. The empty overlay area is transparent and does not intercept pointer input.
- Kept **Start spatial mapping**, **Start live captions**, and **Place captions in room** in separate visible regions on first launch. Creative area cards and note tools appear only after the user opens **Studio areas**.
- Fixed a duplicate `Image` component in the note editor that caused a `NullReferenceException` while constructing the studio.
- Microphone capture remains off until the user taps the live-caption action and grants Android microphone permission. Speech recognition and acoustic diarization run locally when the bundled engine starts.

## Verification limits

This APK has not been installed or runtime-tested on a Samsung S26 or XREAL Air 2 Ultra. No Android device was visible to ADB during this build. Button hit targets on the phone/controller, microphone permission and capture, offline model startup, live transcription, acoustic diarization, XREAL passthrough, spatial tracking, plane mapping, anchor placement/persistence, and caption readability in the glasses still require testing on that hardware. A successful Unity build and edit-mode suite do not prove those device behaviors. XREAL native-library 16 KB alignment on Android 15+ also remains unchecked.

See [SHA256SUMS.txt](SHA256SUMS.txt) for the checksum list. Direct APK downloads require the complete 212 MiB file for each sideloaded update.
