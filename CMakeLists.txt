cmake_minimum_required(VERSION 3.15)

project(vsfreezetest)
enable_testing()

add_subdirectory(${CMAKE_SOURCE_DIR}/googletest-release-1.11.0)
add_executable(vsft main.cpp)
target_link_libraries(vsft gtest_main gmock_main)
add_test(NAME vsft COMMAND $<TARGET_FILE:vsft>)

