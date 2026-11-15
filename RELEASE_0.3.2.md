# ChipOS Studio 0.3.2

Experimental, ARM64-only Android APK. It combines the native creative studio, private editable project cards, offline English speech captions, acoustic speaker labels, floating caption overlay and phone-controlled external-display caption window.

**Glasses output is view-fixed.** It is not room-anchored AR and does not use the camera, LiDAR or depth sensing. The Unity/XREAL spatial prototype remains separate and uses simulated captions. Check this app on the S26 and Air 2 Ultra before relying on external display behavior.

## Build checks

- Android debug and release builds completed.
- Android instrumentation test APK compiled.
- Android lint completed.
- Instrumentation tests were not executed on this machine because no Android device or emulator was online after restart.
- APK signature verified with the established Android debug/test certificate. Certificate SHA-256: 49dd995914a6582eaa33c76fa0c128bd801d43d564a205ba45295d1f9b3a44f2.
- APK is ARM64 and 16 KB zip aligned.
- APK permissions include microphone and floating-window access; no Internet or camera permission is present.

APK SHA-256: 8a359d2a61901bcdab7a2c8e555d4ae44d7f68e4fb9ea9084ded38116c44023e
