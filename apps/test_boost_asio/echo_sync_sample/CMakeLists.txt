cmake_minimum_required(VERSION 2.8)

add_executable(client client.cpp)
target_link_libraries(client ${Boost_LIBRARIES} pthread)

add_executable(server server.cpp)
target_link_libraries(server ${Boost_LIBRARIES} pthread)
