 # libtorrent-demo

libtorrent demo for boost.build / conan / cmake


**==== cpp code copy from libtorrent/examples ====**


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

check out [Jamfile.jam](Jamfile.jam) for b2 build config ( issues )

check out [CMakeLists.txt](CMakeLists.txt) for cmake build config



### issues

for study only,  build pass in linux  ( centOS 8 )

1. some hardcode in [Jamfile.jam](Jamfile.jam) like <include> <library>  
2. b2 build static fail, it not like cmake that build static one file 



2023/01/05




