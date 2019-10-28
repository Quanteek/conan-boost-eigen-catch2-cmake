# conan-boost-eigen-cmake


## Mac OS X
    conan install . --build missing
    mkdir build
    cd build
    cmake .. -G "Unix Makefiles"
    make
    ctest .
