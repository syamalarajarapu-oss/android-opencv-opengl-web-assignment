# 🧪 Android + OpenCV (C++) + OpenGL + TypeScript Web Viewer — RnD Intern Assessment

This project skeleton contains the minimal files and structure to help you start the assignment.
**You still need to open the project in Android Studio, provide proper Gradle files, add OpenCV SDK, and configure NDK.**

## Project structure (skeleton)
```
android-opencv-opengl-assignment/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/com/example/app/MainActivity.kt
│   │       └── java/com/example/app/NativeLib.kt
├── jni/
│   └── native-lib.cpp
├── CMakeLists.txt
├── web/
│   ├── index.html
│   ├── index.ts
│   ├── package.json
│   └── tsconfig.json
├── .gitignore
└── README.md
```

## What this ZIP includes
- Minimal Kotlin files showing how to call JNI.
- Minimal C++ native file (OpenCV calls are stubbed; include OpenCV in your CMake when available).
- A CMakeLists.txt that is a placeholder — adjust paths for OpenCV SDK on your machine.
- A tiny TypeScript web viewer skeleton.
- README with instructions and next steps.

## Important next steps (you must do these locally)
1. Open Android Studio and create a proper Android project (or import this folder into a full project).  
2. Add Gradle (`build.gradle`, `settings.gradle`) and Android manifest — not included in this skeleton.  
3. Download OpenCV Android SDK and point `CMakeLists.txt` to the OpenCV SDK path.  
4. Configure `app/build.gradle` to enable externalNativeBuild (CMake) and set the NDK version.  
5. Build and run on an Android device with USB debugging enabled.  
6. Place sample processed images into `/web` to preview the web viewer.

---
Author: Gurram Gowthami
