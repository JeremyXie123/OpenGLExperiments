cmake_minimum_required(VERSION 3.0.0)
project(OpenGLExperiments VERSION 0.1.0)

include(CTest)
enable_testing()

add_library(OpenGLExperiments OpenGLExperiments.cpp)
add_subdirectory (glad-master)
add_subdirectory (glfw-3.3.4)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
