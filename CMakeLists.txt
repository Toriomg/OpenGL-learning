cmake_minimum_required(VERSION 3.10)
set(VCPKG_MANIFEST_MODE ON)
project(opengl-test)

#set(FMT_USE_DLL OFF)
find_package(glfw3 REQUIRED)
add_executable(Exec ./src/main.cpp)

target_link_libraries(Exec PRIVATE fmt::fmt)