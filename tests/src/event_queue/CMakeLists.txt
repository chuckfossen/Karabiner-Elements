cmake_minimum_required (VERSION 3.9)

include (../../tests.cmake)

project (karabiner_test)

add_executable(
  karabiner_test
  event_queue_test.cpp
  event_queue_event_time_stamp_test.cpp
  event_queue_utility_test.cpp
  test.cpp
)

target_link_libraries(
  karabiner_test
  test_runner
)
