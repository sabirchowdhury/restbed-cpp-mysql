# restbed-cpp

playground for c++ restbed to create an API

Windows:

Install restbed (using vcpkg)
Install CMAKE

remove any build directories:

```
rmdir build
```

build the project and add any required dependencies:

```
cmake -Bbuild -S . -DCMAKE_TOOLCHAIN_FILE={LOCATION_TO_VCPKG}/vcpkg/scripts/buildsystems/vcpkg.cmake

cmake --build build --target ALL_BUILD --config Release

```

Use microsoft visual studio's "MSbuild.exe" to build the solution:

```
MSbuild.exe build/CalculatorAPI.sln
```

This will create an executable in build/Debug/restbedcpp.exe that will run the program

---

Ensure all files and any dependencies are accounted for in the CMakeLists.txt file
