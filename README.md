```
pip3 install conan
mkdir build && cd build
conan profile update settings.compiler.libcxx=libstdc++11 default
conan install .. ## --build=gtest
cmake .. -GNinja
ninja
```
