
include_directories(${DitheringEngine_SOURCE_DIR}/include/dither_library ${DitheringEngine_SOURCE_DIR}/include/filter_library
                    ${DitheringEngine_SOURCE_DIR}/include/path)

add_library(dithering color_space.cpp dither.cpp image_buffer.cpp palette.cpp ppm.cpp)
target_compile_options(dithering PRIVATE -ffast-math)



