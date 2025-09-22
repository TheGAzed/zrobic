set(CERPEC_INCLUDE_TEST OFF)
add_subdirectory(cerpec)

add_subdirectory(sdl)

set(CLAY_INCLUDE_ALL_EXAMPLES OFF)
add_subdirectory(clay)

add_library(EXTERNAL INTERFACE)
target_link_libraries(EXTERNAL INTERFACE SDL3:SDL3 CERPEC clay)
