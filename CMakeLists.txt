cmake_minimum_required(VERSION 3.8)
project(vulkanCpp)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_C_FLAGS "-m64")
set(CMAKE_CXX_FLAGS "-m64")
set(SOURCE_FILES main.cpp)

LINK_DIRECTORIES("F:/Documents/CStuff/CExternals/glfw-3.2.1.bin.WIN64/lib-mingw-w64")
LINK_DIRECTORIES("E:/VulkanSDK/1.0.61.0/Source/lib")

add_executable(vulkanCpp ${SOURCE_FILES})

target_link_libraries(vulkanCpp "vulkan-1")
target_link_libraries(vulkanCpp "F:/Documents/CStuff/CExternals/GLFW/lib/libglfw3.a")
include_directories("F:/Documents/CStuff/CExternals/glfw-3.2.1.bin.WIN64/include")
include_directories("F:/Documents/CStuff/CExternals/glm")
include_directories("E:/VulkanSDK/1.0.61.0/Include")