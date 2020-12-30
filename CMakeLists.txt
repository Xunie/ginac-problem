cmake_minimum_required( VERSION 3.10 )

project( problemo )

set(CLN_SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/git-submodules/cln)
# XXX: GiNaC includes CLN on its own. Eventually there will be a CLN
# submodule in GiNaC repository, so the above line won't be necessary
add_subdirectory( git-submodules/ginac )

add_executable( my_derivative
    src/derivative.cpp
)
target_link_libraries(my_derivative PRIVATE ginac::ginac)
