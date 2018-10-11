cmake_minimum_required(VERSION 3.12)
project(VulkanGraphics)

set(CMAKE_CXX_STANDARD 17)

find_package(glfw3 3.3 REQUIRED)
if(glfw3_FOUND)
    message(STATUS ${glfw3_INCLUDE_DIRS})
    include_directories(${glfw3_INCLUDE_DIRS})
endif(glfw3_FOUND)

add_executable(VulkanGraphics main.cpp)
target_link_libraries(VulkanGraphics ${glfw3_LIBRARIES})