# zlib-minimal
The code in this repository is in no way, shape or form mine. The code is copied from the [zlib GitHub repo](https://github.com/madler/zlib) to make a very minimal library that can be included into a project as a library. 

## Why?
I had a lot of issues linking zlib to a project of my own, where zlib would take over my project with a main function that was run somewhere (probably from an example). I decided to make it easy for myself and copy the essential files for (de)compressing a gzipped file.

## How can I use this easily?
The easiest would be using the `FetchContent` directive in CMake. To include this project, you should only have to add the following to your CMakeLists.txt:
```cmake
include(FetchContent)

FetchContent_Declare(
        zlib-minimal
        GIT_REPOSITORY https://github.com/camielverdult/zlib-minimal.git
        GIT_TAG        main
)

FetchContent_MakeAvailable(zlib-minimal)

target_link_libraries(your_project zlib-minimal)
```