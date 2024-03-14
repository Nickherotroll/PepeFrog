cmake_minimum_required(VERSION 3.8.0)
project(PepeFrog VERSION 0.1.0 LANGUAGES C CXX)

enable_testing()

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})

FIND_PACKAGE(Boost COMPONENTS REQUIRED)
INCLUDE_DIRECTORIES( ${Boost_INCLUDE_DIR} )

add_subdirectory(src)

add_subdirectory(libs/DPP)
