cmake_minimum_required(VERSION 3.10)
project(DaytimeProject)


find_package(Boost REQUIRED COMPONENTS system)

add_executable(myserver server.cpp)
target_link_libraries(myserver Boost::system)
add_executable(myclient client.cpp)
target_link_libraries(myclient Boost::system)
