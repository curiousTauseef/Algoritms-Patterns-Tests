cmake_minimum_required(VERSION 2.8)

set(PROJECT_NAME test_asio_server001)
project(${PROJECT_NAME})

set(SOURCES
    src/main.cpp
    )
add_executable(${PROJECT_NAME} ${SOURCES})

set(LIBS
    boost_system
    boost_thread
    
    pthread
    )
target_link_libraries(${PROJECT_NAME} ${LIBS})
