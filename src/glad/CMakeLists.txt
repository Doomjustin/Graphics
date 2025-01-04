add_library(glad OBJECT
    glad/glad.h
    KHR/khrplatform.h
    glad.c
)

target_include_directories(glad PUBLIC ${CMAKE_CURRENT_LIST_DIR})

SET(OPENGL_CORE_VERSION_MAJOR 3 PARENT_SCOPE)
SET(OPENGL_CORE_VERSION_MAJOR 3 PARENT_SCOPE)