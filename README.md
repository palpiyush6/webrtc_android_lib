# WebRTC Android Library
This repository contains the WebRTC library for Android development built from the official Google WebRTC sources synced on 8-April-2023.

    Supported ABIs: armeabi-v7a, arm64-v8a, x86, x86_64

## How to use it in an Android Studio project?
1. Go to the `libs` directory of your android studio project.
2. Paste the `libwebrtc.aar` file in this directory.
3. Go to `build.gradle(module)` file and add/modify the following line inside the `dependencies{...}` scope:


       implementation fileTree(dir: "libs", includes: ["*.aar"])

4. Hit `Sync Project`.
5. Once sync is done, Go to any Kotlin/Java file and try to import WebRTC classes to check whether everything is proper or not.

       import org.webrtc.*;
