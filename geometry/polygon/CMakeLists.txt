add_library(polygon polygon.cpp)
target_link_libraries(polygon geometry_base)

add_gmock_test(polygon_unittest polygon_test.cpp)
target_link_libraries(polygon_unittest polygon geometry_base)