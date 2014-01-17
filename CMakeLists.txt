cmake_minimum_required( VERSION 2.8 )

project( framework )

add_definitions( -g `sdl2-config --cflags` )
add_executable( framework main.cpp gameengine.cpp imagehandler.cpp playstate.cpp )
target_link_libraries( framework -lSDL2 -lSDL2_image )