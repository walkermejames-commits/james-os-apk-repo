# ChipOS Mark II Unity AR 0.1.21

- Experimental Android ARM64 APK built with Unity 6000.6.5f1.
- Android package: `com.walkermejames.chiposmarkii`.
- Android version: `0.1.21`, version code `21`.
- APK size: 225,338,124 bytes.
- SHA-256: `A8B370AF33827C604482581579DEF4CB816DC97863D4127174249FC80AE7DFA3`.
- Unity Android build succeeded with 0 errors and 75 warnings. APK v2 signature verification passed.
- Installed and exercised on the Samsung S26 API 36 x86_64 emulator. The startup dock was visible; tapping camera mapping displayed the emulator limitation; tapping live captions displayed that the bundled speech runtime is unavailable for x86_64. No crash was observed in these interactions.

## Changes

- Extended the acoustic diarization analysis window to 12 seconds and associate speaker segments with the full finalized caption interval.
- Added a software microphone gain control for quiet input routes.
- Kept the phone studio layout visible and gave spatial and speech failures explicit status messages.

## Verification limits

The emulator test verifies visible controls and their unsupported-device status paths only. It does not verify microphone capture, recognition accuracy, acoustic speaker diarization, camera mapping, room-anchored captions, XREAL see-through rendering, or Air 2 Ultra controller/hand input. The APK is ARM64-only; the emulator's x86_64 image cannot run the bundled offline speech runtime. Those features remain unverified on the physical S26 with Air 2 Ultra. The room around the emulator is not available to the app, so a dark phone display there is expected.

This release is experimental and should not be treated as confirmation that spatial mapping or live speech works on the target hardware. Direct sideloaded updates require downloading the complete APK.
