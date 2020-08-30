add_executable(wine main.c)

if(HAVE_LIBM)
    target_link_libraries(wine m)
endif()

if(HAVE_LIBDL)
    target_link_libraries(wine dl)
endif()