# WebRTC Android Library
This repository contains the WebRTC library for Android development built from the official Google WebRTC sources. Please check the release section to find the library.

    Supported ABIs: armeabi-v7a, arm64-v8a, x86, x86_64

## How to use it in an Android Studio project?
1. Go to the `libs` directory of your android studio project.
2. Paste the `libwebrtc.aar` file in this directory.
3. Go to `build.gradle (Module)` file and add/modify the following line inside the `dependencies{...}` scope:


       implementation fileTree(dir: "libs", includes: ["*.aar"])

4. Hit `Sync Now`.
5. Once the sync is done, Check whether the library is included correctly or not by importing WebRTC classes/interfaces. Paste the below line in any Kotlin/Java file to import. If the IDE doesn't show `Unresolved reference: webrtc`, You are good to go!

       import org.webrtc.*;
