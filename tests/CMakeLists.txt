enable_testing()
include_directories(${GTEST_INCLUDE_DIRS})
add_executable(jamspell_tests test_perfect_hash.cpp)
target_link_libraries(jamspell_tests jamspell_lib ${GTEST_BOTH_LIBRARIES} pthread)
add_test(jamspell_tests jamspell_tests)
