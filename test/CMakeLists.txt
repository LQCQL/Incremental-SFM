project(test)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS "-fPIC")

include_directories("../..")

set(INCREMENTAL_SFM_SOURCES
        main.cpp defines.h functions.cc functions.h)
add_executable(test ${INCREMENTAL_SFM_SOURCES})
target_link_libraries(test sfm util core features)

