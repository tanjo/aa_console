cmake_minimum_required(VERSION 2.8)

project(AAConsole CXX)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/../aa_console)
add_executable(sample_aa_console ${CMAKE_CURRENT_SOURCE_DIR}/sample_aa_console.cc)
target_link_libraries(sample_aa_console aa_console)
