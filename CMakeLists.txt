cmake_minimum_required(VERSION 3.0.0)
project(path-tracing-renderer VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

add_executable(path-tracing-renderer path-tracing-renderer.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
