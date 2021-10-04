# UniStl C17
Universal Standard Library

## Getting Started

UniStl is built and tested using the CMake build system and the Google Test framework.
(We plan to provide simple Bazel and Make integration)

With CMake:
1. Install CMake >= 3.10.0
2. Get UniStl source:
```console
git clone https://github.com/UniversalLib/UniStl.git
# or
git clone git@github.com:UniversalLib/UniStl.git
```
then `cd UniStl/C17`
3. Build UniStl and run tests (use `-DBUILD_TESTING=OFF` to skip the testing)
```console
mkdir build
cd build
cmake -GNinja ..
ninja
# or
cmake -G "Unix Makefiles" ..
make
```
4. Use in CMake-based project with:
```cmake
add_executable(target file.c)

add_subdirectory(libs/unistl/C17/)
target_link_libraries(target unistl::c17)
```

# License
UniStl is licensed under the BSD-3-Clause-Clear license