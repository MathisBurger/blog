


Path:

- Used mitm.it as a http proxy on my iphone => Tracked traffic
- Decompiled the android app apk using apktool and tried to understand the code. 
- Reversed most of the code that was relevant for the API signature generation --> show m.java file and part where hash is computed
- Recompiled the APK with some debug flags set and signed it with debug key and installed it on an android emulator
- Created heap dump using android studio