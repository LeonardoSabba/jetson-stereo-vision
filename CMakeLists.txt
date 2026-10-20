cmake_minimum_required(VERSION 3.16)

project(jetson_stereo_vision
    VERSION 0.1.0
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

find_package(OpenCV REQUIRED)

add_executable(stereo_vision
    src/main.cpp
)

target_link_libraries(stereo_vision
    PRIVATE
    ${OpenCV_LIBS}
)

target_include_directories(stereo_vision
    PRIVATE
    ${OpenCV_INCLUDE_DIRS}
)
