# conan-vtk

This is fully functional [conan.io](https://conan.io/) recipe for VTK 9.0.1 version.  

Still few things are missing, to become official recipe for VTK (details [here](https://github.com/conan-io/conan-center-index/pull/3280)).  
Feel free to improve it and push to [conan-center-index](https://github.com/conan-io/conan-center-index) git repo.

It was tested on Conan version `1.30.2` and successfully produced 124 different OS/options conan packages.

<details>
  <summary>List here:</summary>
  
- Windows:
  - Compilers: Visual Studio:
    - 2015 (14.0.25431.01 Update 3)
    - 2017 (15.9.19+28307.1000)
    - 2019 (16.4.4+29728.190)
  - Release (MT/MD) and Debug (MTd, MDd)
  - Architectures: x86_64
  - Build types: Release, Debug
  - Runtimes: MT/MD (Release), MTd/MDd (Debug)
  - Options: Shared, Static (option `"shared": [True, False]`)


- Linux
  - Compilers:
    - GCC versions 4.9, 5, 6, 7, 8, 9
    - Clang versions 3.9, 4.0, 5.0, 6.0, 7.0, 8, 9
  - C++ Standard Library (`libcxx`):
    - GCC compiler: `libstdc++`, `libstdc++11`
    - Clang compiler: `libstdc++`, `libc++`
  - Architectures: x86_64
  - Build types: Release, Debug
  - Options: Shared, Static (option `"shared": [True, False]`)


- MacOS
  - Compilers: Apple-clang versions 9.1, 10.0, 11.0 (three latest versions, we will rotate the older when a new compiler version is released)
  - C++ Standard Library (`libcxx`): `libc++`
  - Architectures: x86_64
  - Build types: Release, Debug
  - Options: Shared, Static (option `"shared": [True, False]`)
</details>
