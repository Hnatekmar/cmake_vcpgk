# cmake_vcpgk
Small wrapper around vcpkg for cmake

# Usage
First you need to install vcpkg and put it into your `PATH`

1. Add this as git submodule to your project
2. At the beginning of your `CMakeLists.txt` put 
```
include(cmake_vcpkg/vcpkg.cmake)

find_vcpkg()
```
This will automatically setup your cmake so it will use vcpkg.

You can also install packages via `vcpkg_install_library` like this
```
vcpkg_install_library(sfml)
```
