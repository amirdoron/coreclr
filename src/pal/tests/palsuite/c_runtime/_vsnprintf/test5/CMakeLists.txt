cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test5.c
)

add_executable(paltest_vsnprintf_test5
  ${SOURCES}
)

add_dependencies(paltest_vsnprintf_test5 CoreClrPal)

target_link_libraries(paltest_vsnprintf_test5
  pthread
  m
  CoreClrPal
)
