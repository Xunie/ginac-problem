cmake_minimum_required( VERSION 3.0 )

project( problemo )

add_subdirectory( git-submodules/cln )
add_subdirectory( git-submodules/ginac )

add_executable( main
    src/main.cpp
)
