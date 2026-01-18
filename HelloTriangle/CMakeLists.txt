cmake_minimum_required(VERSION 3.16)
project(HelloTriangle LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Vulkan REQUIRED)
find_package(PkgConfig REQUIRED)
pkg_check_modules(GLFW REQUIRED glfw3)
find_package(glm REQUIRED)

add_executable(HelloTriangle src/main.cpp)
target_include_directories(HelloTriangle PRIVATE ${GLFW_INCLUDE_DIRS})
target_link_libraries(HelloTriangle PRIVATE ${GLFW_LIBRARIES} glm::glm Vulkan::Vulkan)
