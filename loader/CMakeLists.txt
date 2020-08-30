add_executable(wine main.c)

if(HAVE_LIBM)
    target_link_libraries(wine m)
endif()