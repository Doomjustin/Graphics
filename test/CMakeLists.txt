list(APPEND CMAKE_MODULE_PATH ${catch2_SOURCE_DIR}/extras)
include(CTest)
include(Catch)

function(graphics_add_test target)
    add_executable(${target} ${target}.cpp)

    target_link_libraries(${target}
        PRIVATE
            Catch2::Catch2WithMain
    )

    catch_discover_tests(${target})
endfunction()
