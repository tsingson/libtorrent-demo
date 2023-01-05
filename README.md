# libtorrent-demo

libtorrent demo for boost.build / conan / cmake



install libtorrent with conan

```
conan install . --build missing
```



build with b2 ( boost.build )

```
b2 release
```



build with cmake

```
mkdir build 
cd build
conan install .. --build missing
cmake build ..
make -B 
```



check out [conanfile.txt](conanfile.txt) for libtorrent library include for build 

check out [Jamfile.jam](Jamfile.jam) for b2 build config

check out [CMakeLists.txt](CMakeLists.txt) for cmake build config



