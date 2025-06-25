# BLACK X [Injecter]

A high-performance Android injector combining Java and C++ for Unity (il2cpp) games.  
Designed for real-time modding, memory patching, and custom UI overlays. for real-time modding, memory patching, and custom UI overlays.

---

## 📄 Description

A professional-grade Android injector leveraging native C++ and Java layers to inject code, patch memory, and deploy real-time game modifications.  
Optimized for Unity il2cpp games, it supports floating UI, native hooking, and 64-bit compatibility with minimal performance overhead.

---

## ✨ Features

- Java + C++ hybrid injector architecture
- Unity il2cpp memory patching
- Native library (.so) injection
- Dobby or KittyMemory support
- Floating mod menu with ImGui
- Support for Aimbot, ESP, FOV, and more
- 64-bit game compatibility

---

## 📁 Folder Structure
AndroidInjector/
├── app/                        # Java Android app source
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/           # Java package (UI, Service)
│   │   │   ├── res/            # UI resources (layouts, icons)
│   │   │   └── AndroidManifest.xml
│   └── build.gradle
│
├── jni/                        # Native C++ injector code
│   ├── main.cpp                # Entry point for native injector
│   ├── Injector.hpp/.cpp       # Memory patching, native methods
│   ├── Dobby/                  # Optional: Hooking library
│   ├── KittyMemory/            # Optional: Memory patching lib
│   ├── imgui/                  # ImGui floating UI
│   ├── UnityOffsets.hpp        # Offsets for il2cpp structures
│   └── config.h                # Custom feature toggles
│
├── libs/                       # Precompiled .so libraries
│   └── arm64-v8a/
│       └── libmodmenu.so
│
├── CMakeLists.txt              # CMake config for JNI build
├── Android.mk                  # (Optional) Android NDK makefile
├── build.gradle                # Project-level Gradle file
├── settings.gradle
└── README.md                   # Project documentation
