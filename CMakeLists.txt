cmake_minimum_required(VERSION 3.0.0)
project(design_pattern VERSION 0.1.0)

include(CTest)
enable_testing()

add_executable(iterator src/iterator/iterator.cpp)

add_executable(adapter src/adapter/adapter.cpp)

add_executable(template_method src/template_method/template_method.cpp)

add_executable(factory_method src/factory_method/factory_method.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)