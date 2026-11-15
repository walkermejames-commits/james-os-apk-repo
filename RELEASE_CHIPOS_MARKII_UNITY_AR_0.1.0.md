# ChipOS Mark II Unity AR 0.1.0

- Experimental Android ARM64 release build from Unity 6000.6.5f1.
- Package: `com.walkermejames.chiposmarkii`.
- Android minimum API 31; target API 36.
- Signed with the Unity Android debug certificate for local installation.
- Bundles Sherpa ONNX native libraries, offline ASR/diarization models, and the XREAL SDK.
- Unity build result: succeeded with 0 errors and 44 warnings. APK v2 signature verified.

This APK has not been installed or runtime-tested on a Samsung S26 or XREAL Air 2 Ultra. Actual live transcription, speaker identity, touch/glasses input, XREAL tracking, spatial mapping, room-anchor behavior and persistence require hardware verification. The XREAL ARM64 native plugin reports it is not 16 KB aligned, which may affect Android 15+ compatibility.

SHA-256: `E7E63AF264DAE1B686CAEE6CBB5DB5380E51E731A3378662AA3359CEE19C3D9C`
