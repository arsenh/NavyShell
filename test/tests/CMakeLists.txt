project(demo_project_tests)

add_executable(demo_project_tests tests.cpp)

add_test(NAME demo_project_tests COMMAND demo_project_tests)

target_link_libraries(demo_project_tests shell gtest gtest_main)
