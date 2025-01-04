add_library(stb OBJECT
    stb_image.h
    stb_image.cpp
)

target_include_directories(stb PUBLIC ${CMAKE_CURRENT_LIST_DIR})
