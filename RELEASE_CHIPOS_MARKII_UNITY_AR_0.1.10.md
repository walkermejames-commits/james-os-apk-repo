# ChipOS Mark II Unity AR 0.1.10

- Experimental Android ARM64 APK built with Unity 6000.6.5f1.
- Android package: `com.walkermejames.chiposmarkii`.
- Android version: `0.1.10`, version code `10`.
- APK size: 225,291,117 bytes.
- SHA-256: `D15137A98ECB564B4E6627488A1C1505CA3D649BB22F3A9CDE0D48D2D08056A0`.
- Unity Android build succeeded with 0 errors and 72 warnings.
- Installed and exercised on the Samsung S26 API 36 x86_64 emulator. The startup dock was visible; tapping captions requested microphone permission and then reported that the emulator cannot run the bundled ARM64 speech/diarization engine. Tapping spatial mapping requested camera permission and then reported AR tracking unsupported. The app remained open and the dock stayed visible.

## Changes

- Rebuilt the Unity speech bridge AAR from source so the packaged code rejects unsupported emulator ABI before Sherpa/ONNX native initialization. This avoids the prior native crash on the x86_64 emulator.
- Kept the transparent studio dock visible while spatial initialization is pending. Phone camera background only activates after AR tracking is confirmed; XREAL uses a transparent scene background for see-through displays.
- Added a tracking startup timeout and an explicit unsupported state so mapping does not remain at “starting” indefinitely.
- Gave the status and caption text a dedicated left column so it does not sit underneath the action buttons.
- Microphone capture remains off until the user taps the caption action and grants Android microphone permission. Audio recognition and acoustic diarization use bundled local models on supported ARM64 hardware; no captions or diarization were verified in this emulator run.

## Verification limits

The emulator has no functional AR tracking provider and runs this ARM64 app under translation on an x86_64 image. The emulator check does not verify live speech recognition, acoustic speaker diarization, S26 camera mapping, room-anchored caption placement, persistent room anchors, XREAL optical see-through rendering, or Air 2 Ultra input. Those still need testing on the Samsung S26 with the Air 2 Ultra connected. The Unity EditMode test command was attempted, but Unity exited without generating its requested test-results XML; no EditMode pass count is claimed for this release.

See [SHA256SUMS.txt](SHA256SUMS.txt) for the checksum list. Direct sideloaded APK updates still require downloading the complete APK.
