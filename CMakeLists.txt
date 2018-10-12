cmake_minimum_required(VERSION 3.12)
project(VulkanGraphics)

set(CMAKE_CXX_STANDARD 17)

find_package(glfw3 3.3 REQUIRED)

add_executable(VulkanGraphics main.cpp)
target_link_libraries(VulkanGraphics glfw)
