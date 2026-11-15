# ChipOS Mark II Unity AR 0.1.2

- Experimental Android ARM64 APK built with Unity 6000.6.5f1.
- Package: `com.walkermejames.chiposmarkii`.
- Android version name/code: `0.1.2` / `2`.
- Android minimum API 31; target API 36.
- Adds an independent high-order studio overlay canvas so the studio does not inherit a hidden legacy HUD's alpha or raycast state.
- Requests Android camera permission only after the user taps **Start spatial mapping**. Denial leaves mapping off and reports that phone controls remain available.
- Keeps microphone capture behind the explicit **Start microphone & captions** action and requests microphone permission through Android.
- APK build succeeded with 0 errors and 72 warnings. APK v2 signature verified; ARM64 package and `CAMERA`/`RECORD_AUDIO` permissions confirmed.
- Unity edit-mode checks: 42 passed, 0 failed.
- SHA-256: `97AC06FCD6CDA53E4E1DBA4D41F4380890880477675DCCA934973E4AA51EEABC`.

This APK has not been installed or runtime-tested on a Samsung S26 or XREAL Air 2 Ultra. The APK was copied to the attached S26's `Download` folder, but it has not been installed. Button visibility/touch, live microphone capture, offline transcription, acoustic speaker identification, XREAL tracking, camera-based plane mapping, room-anchor placement and persistence, glasses controls, and 16 KB native-library compatibility remain unverified. The XREAL native-library alignment warning from 0.1.1 remains applicable until checked against this build and device.
