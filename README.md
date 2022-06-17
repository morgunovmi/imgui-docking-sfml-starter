# imgui-docking-sfml-starter
A template starter project that you can use to start developing powerful GUI apps. The example app includes a basic dockspace setup with a simple scene rendered to an imgui window. It also shows how you can easily manipulate your SFML objects from imgui widgets.

![2022-06-17_11-56-21_screenshot](https://user-images.githubusercontent.com/48750724/174264690-48a9e0e2-62d4-41cc-a2ec-a12c935410b6.png)


## Build

### Windows
You need to have CMake and Visual Studio installed. Then run this code in a Developer PowerShell:

```
git clone --recurse-submodules -j8 https://github.com/morgunovmi/imgui-docking-sfml-starter.git
cd imgui-docking-sfml-starter
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Debug -DCMAKE_TOOLCHAIN_FILE=..\vendor\vcpkg\scripts\buildsystems\vcpkg.cmake -DVCPKG_TARGET_TRIPLET=x64-windows ..
cmake --build -j8 . --config=Debug
..\bin\Debug\App.exe
```

### Linux
You need to have CMake and a C++ compiler installed. Then run this code in the terminal:

```
git clone --recurse-submodules -j8 https://github.com/morgunovmi/imgui-docking-sfml-starter.git
cd imgui-docking-sfml-starter
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Debug -DCMAKE_TOOLCHAIN_FILE=../vendor/vcpkg/scripts/buildsystems/vcpkg.cmake -DVCPKG_TARGET_TRIPLET=x64-linux ..
cmake --build -j8 .
../bin/Debug/App
```
