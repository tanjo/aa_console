cmake_minimum_required(VERSION 2.8)

project(AAConsole CXX)

set(serial "1.0.0")
set(soserial "1")

set(src
  ${CMAKE_CURRENT_SOURCE_DIR}/aa_console.cc
)

set(headers
  ${CMAKE_CURRENT_SOURCE_DIR}/aa_console.hh
)

add_library(aa_console SHARED ${src} ${headers})

set_target_properties(aa_console PROPERTIES VERSION ${serial} SOVERSION ${soserial})

# install(TARGETS aa_console LIBRARY DESTINATION lib)
# install(FILES aa_console.h DESTINATION include)
