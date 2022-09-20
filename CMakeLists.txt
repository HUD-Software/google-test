cmake_minimum_required(VERSION 3.18)

project(GoogleTest)

set(GOOGLETEST_VERSION 1.12.1)
add_subdirectory(src)

set_target_properties(gtest PROPERTIES ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/target/${CMAKE_SYSTEM_NAME}_${CMAKE_CXX_COMPILER_ID}_${CMAKE_SYSTEM_PROCESSOR}/${CMAKE_BUILD_TYPE})