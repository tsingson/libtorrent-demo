 # libtorrent-demo

libtorrent demo for boost.build / conan / cmake





### install conan

```
pip3 install conan
```



### install b2 ( boost.build )

check out [https://www.boost.org/build/doc/html/bbv2/installation.html](https://www.boost.org/build/doc/html/bbv2/installation.html)  or [https://github.com/bfgroup/b2](https://github.com/bfgroup/b2)



### install libtorrent with conan

```
conan install . --build missing
```



### build with b2 ( boost.build )

```
b2 release
```



### build with cmake

```
mkdir build 
cd build
conan install .. --build missing
cmake build ..
make -B 
```



### note

check out [conanfile.txt](conanfile.txt) for libtorrent library include for build 

check out [Jamfile.jam](Jamfile.jam) for b2 build config ( some hardcode , update soon for better intergrate with conan )

check out [CMakeLists.txt](CMakeLists.txt) for cmake build config



### build for 

for study only,  build pass in linux  ( centOS 8 )



2023/01/05




