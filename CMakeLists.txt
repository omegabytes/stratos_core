cmake_minimum_required(VERSION 2.8)
project(stratos_core)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

find_package(OpenCV REQUIRED)

add_executable(vcap src/vcap.cpp)

target_link_libraries(vcap ${OpenCV_LIBS})
