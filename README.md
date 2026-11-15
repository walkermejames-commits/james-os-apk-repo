# James OS APK repository

Direct downloads (APK files are Android application packages; install only if you trust the build):

| App / build | Download |
| --- | --- |
| ChipOS Studio 0.3.2 (experimental ARM64; consolidated studio, offline captions + acoustic speaker labels, phone controls + separate glasses caption display) | [Download APK](https://github.com/walkermejames-commits/james-os-apk-repo/releases/download/chipos-studio-0.3.2/chipos-studio-0.3.2-arm64.apk) |
| ChipOS Studio 0.3.1 (experimental ARM64; phone controls + separate glasses caption display) | [Download APK](https://github.com/walkermejames-commits/james-os-apk-repo/releases/download/chipos-studio-0.3.1/chipos-studio-0.3.1-arm64.apk) |
| ChipOS Studio 0.3.0 (superseded by 0.3.1; phone studio and floating captions) | [Download APK](https://github.com/walkermejames-commits/james-os-apk-repo/releases/download/chipos-studio-0.3.0/chipos-studio-0.3.0-arm64.apk) |
| ChipOS Mark II Unity first build (OLD KEYBOARD DEMO; simulated captions, not the studio; do not install for glasses use) | [Archived prototype](https://raw.githubusercontent.com/walkermejames-commits/james-os-apk-repo/main/chipos-markii-unity-first-build-arm64.apk) |
| ChipOS AR Caption Lens 0.2.4 (experimental, arm64) | [Download APK](https://github.com/walkermejames-commits/james-os-apk-repo/releases/download/chipos-ar-0.2.4-caption-lens/chipos-ar-0.2.4-caption-lens-arm64.apk) |
| ChipOS AR Caption Lens 0.2.3 (experimental, arm64) | [Download APK](https://github.com/walkermejames-commits/james-os-apk-repo/releases/download/chipos-ar-0.2.3-caption-lens/chipos-ar-0.2.3-caption-lens-arm64.apk) |
| ChipOS AR Caption Lens 0.2.2 (experimental, arm64 debug) | [Download APK](https://github.com/walkermejames-commits/james-os-apk-repo/releases/download/chipos-ar-0.2.2-caption-lens/chipos-ar-0.2.2-caption-lens-debug.apk) |
| ChipOS AR Caption Lens 0.2.1 (experimental, arm64 debug) | [Download APK](https://github.com/walkermejames-commits/james-os-apk-repo/releases/download/chipos-ar-0.2.1-caption-lens/chipos-ar-0.2.1-caption-lens-debug.apk) |
| ChipOS AR Caption Lens 0.2.0 (experimental, arm64 debug) | [Download APK](https://github.com/walkermejames-commits/james-os-apk-repo/releases/download/chipos-ar-0.2.0-caption-lens/chipos-ar-0.2.0-caption-lens-debug.apk) |
| Scrying RF 0.4.1 (debug) | [Download APK](https://raw.githubusercontent.com/walkermejames-commits/james-os-apk-repo/main/scrying-0.4.1-debug.apk) |
| Scrying RF 0.4.0 (debug) | [Download APK](https://raw.githubusercontent.com/walkermejames-commits/james-os-apk-repo/main/scrying-0.4.0-debug.apk) |
| Scrying RF 0.3.1 (debug) | [Download APK](https://raw.githubusercontent.com/walkermejames-commits/james-os-apk-repo/main/scrying-0.3.1-debug.apk) |
| Scrying RF 0.3.0 (debug) | [Download APK](https://raw.githubusercontent.com/walkermejames-commits/james-os-apk-repo/main/scrying-0.3.0-debug.apk) |
| Scrying RF 0.2.0 (debug) | [Download APK](https://raw.githubusercontent.com/walkermejames-commits/james-os-apk-repo/main/scrying-0.2.0-debug.apk) |
| Scrying RF current build (debug) | [Download APK](https://raw.githubusercontent.com/walkermejames-commits/james-os-apk-repo/main/app-debug.apk) |
| TWK Driver ARM64 (debug) | [Download APK](https://raw.githubusercontent.com/walkermejames-commits/james-os-apk-repo/main/twk-driver-arm64-debug.apk) |
| Doorin Driver ARM64 (debug) | [Download APK](https://raw.githubusercontent.com/walkermejames-commits/james-os-apk-repo/main/doorin-driver-arm64-debug.apk) |

ChipOS Studio 0.3.2 packages the native creative studio, offline speech and acoustic diarization, floating subtitles, and phone controls for an external glasses caption display. The glasses output is **view-fixed**; this APK has no tracked 6DoF anchors, room scan or LiDAR support. S26/XREAL hardware testing is still required. The APK is signed with the existing experimental Android test certificate. See [0.3.2 build notes](RELEASE_0.3.2.md) and [SHA-256 checksum](SHA256SUMS.txt).

The native Android project is the installable Studio and speech source. The separate Unity/XREAL prototype contains spatial tracking experiments but simulated captions, so it is not included as a working Studio APK. See the source audit in the Android source repository.

**Do not install the archived ChipOS Mark II keyboard demo for glasses use.** It shows simulated placeholder captions such as “Caption frame received”; they are not speech recognition.
