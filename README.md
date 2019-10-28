# conan-boost-eigen-catch2-cmake


## Mac OS X
    conan remote add conan-community https://api.bintray.com/conan/conan-community/conan
    conan remote add catchorg https://api.bintray.com/conan/catchorg/Catch2
    conan install . --build missing
    mkdir build
    cd build
    cmake .. -G "Unix Makefiles"
    make
    bin/test_catch
    bin/test_boost
