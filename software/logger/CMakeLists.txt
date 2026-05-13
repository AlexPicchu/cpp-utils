add_library(logger
    src/logger.cc
)   

target_include_directories(logger
    PUBLIC
$<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
        $<INSTALL_INTERFACE:include>
)

target_compile_options(logger PRIVATE -Wall -Wextra
-Wpedantic)ß