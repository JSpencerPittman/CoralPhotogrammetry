cmake_minimum_required(VERSION 3.12)

set(CMAKE_CXX_STANDARD 11)

project(CoralPhotogrammetry VERSION 1.0)
set(CoralPhotogrammetry_VERSION 1.0)

find_package(OpenMVG REQUIRED)

file(GLOB CORAL_SOURCE_FILES src/*.cpp)
file(GLOB CORAL_HEADER_FILES include/*.h)

add_executable(CoralGram ${CORAL_SOURCE_FILES})

# target_include_directories(CoralGram CORAL_HEADER_FILES)