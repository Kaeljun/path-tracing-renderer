cmake_minimum_required(VERSION 3.5.0)
project(path-tracing-renderer VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

add_executable(path-tracing-renderer src/path-tracing-renderer.cpp "src/ray.h")

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
