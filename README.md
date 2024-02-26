A useless and broken Android mfoc port
======================================

This was the result of me trying to port the mfoc tool to Android, by simply running the C code using NDK, under a small wrapper that provides the libc and libnfc calls.

Status
------

Don't be so excited: all this code can do is to (poorly) probe for default keys. I don't know if it's completely working, as it didn't get much testing.

It **can't** run the actual cracking code, because it depends on the ability of disabling parity check and sending/receiving raw parity bits, and this doesn't seem to be possible using the Android API.


APK
---

If you still want to see it running, you can get an APK at:
https://github.com/downloads/ehabkost/nfc-tools/AndroidMfoc.apk


=================
- EDIT:
APK located in link isn't active but used that link in archive.org which lead to an archive of that APK at=

https://web.archive.org/web/20201122173142/https://github.s3.amazonaws.com/downloads/ehabkost/nfc-tools/AndroidMfoc.apk?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAISTNZFOVBIJMK3TQ%2F20201122%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20201122T173142Z&X-Amz-Expires=300&X-Amz-SignedHeaders=host&X-Amz-Signature=7ec1012c2a09792dc636a67ee5e17366a827637166bb23d08cea4d64a41399a1
