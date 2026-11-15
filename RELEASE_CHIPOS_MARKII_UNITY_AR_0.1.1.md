# ChipOS Mark II Unity AR 0.1.1

- Experimental Android ARM64 release build from Unity 6000.6.5f1.
- Package: `com.walkermejames.chiposmarkii`; app label: ChipOS Mark II.
- Android minimum API 31; target API 36.
- Signed with the Unity Android debug certificate for local installation.
- Bundles Sherpa ONNX native libraries, offline ASR/diarization models, and the XREAL SDK.
- Fixes microphone startup model paths to match Unity's packaged Android assets and shows actual loading/running/failure state.
- Promotes Start microphone & captions and Start spatial mapping controls; separates area list and detail views with higher contrast.
- Unity build result: succeeded with 0 errors and 44 warnings. APK v2 signature verified.

This APK has not been installed or runtime-tested on a Samsung S26 or XREAL Air 2 Ultra. Actual live transcription, speaker identity, touch/glasses input, XREAL tracking, spatial mapping, room-anchor behavior and persistence require hardware verification. XREAL native libraries report that they are not 16 KB aligned, which may affect Android 15+ compatibility.

SHA-256: `38019B1105833838BDCD8403FD01C944700705650BB5D79B8FE24A3139DF37AA`
