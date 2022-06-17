# imgui-docking-sfml-starter
A template starter project that you can use to start developing powerful GUI apps. The example app includes a basic dockspace setup with a simple scene rendered to an imgui window. It also shows how you can easily manipulate your SFML objects from imgui widgets.

![2022-06-17_11-37-29_screenshot](https://user-images.githubusercontent.com/48750724/174261509-4db781c6-4aee-415f-a4b9-a51ab13b9762.png)

## Build

### Windows
You need to have CMake and Visual Studio installed. Then run this code in a Developer PowerShell:

```
git clone --recurse-submodules -j8 https://github.com/morgunovmi/imgui-docking-sfml-starter.git
cd imgui-docking-sfml-starter
mkdir build
cd build
cmake -DCMAKE_TOOLCHAIN_FILE=../vendor/vcpkg/scripts/buildsystems/vcpkg.cmake -DCMAKE_BUILD_TYPE=Debug ..
cmake --build . --config=Debug
../bin/Debug/App.exe
```

### Linux
You need to have CMake and a C++ compiler installed. Then run this code in the terminal:

```
git clone --recurse-submodules -j8 https://github.com/morgunovmi/imgui-docking-sfml-starter.git
cd imgui-docking-sfml-starter
mkdir build
cd build
cmake -DCMAKE_TOOLCHAIN_FILE=../vendor/vcpkg/scripts/buildsystems/vcpkg.cmake -DCMAKE_BUILD_TYPE=Debug ..
cmake --build .
../bin/Debug/App
```
