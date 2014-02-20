cmake_minimum_required( VERSION 2.8 )

project( framework )
set( CMAKE_CXX_FLAGS_DEBUG )
set( CMAKE_C_FLAGS_DEBUG )
add_executable( framework main.cpp gameengine.cpp graphics.cpp playstate.cpp )
target_link_libraries( framework -lSDL2 -lSDL2_image -lSDL2_ttf )