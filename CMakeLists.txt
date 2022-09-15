cmake_minimum_required(VERSION 3.18)

project(GoogleTest)

add_subdirectory(src)

set_target_properties(gtest PROPERTIES ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/target/${CMAKE_SYSTEM_NAME}_${CMAKE_CXX_COMPILER_ID}_${CMAKE_SYSTEM_PROCESSOR}/${CMAKE_BUILD_TYPE})