# Sets CMAKE version
cmake_minimum_required(VERSION 3.27)
project(main CXX)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_CXX_USE_RESPONSE_FILE_FOR_INCLUDES OFF)

add_executable(test_main
    main.cpp
)
target_compile_options(test_main
    PUBLIC -g3 -O0 -Wall -finput-charset=CP932 -fexec-charset=UTF-8
)
