add_executable(bt_get
        bt-get.cpp)
target_link_libraries(bt_get ${CONAN_LIBS})

add_executable(bt_get3
        bt-get3.cpp)
target_link_libraries(bt_get3 ${CONAN_LIBS})

add_executable(example1
        example1.cpp)
target_link_libraries(example1 ${CONAN_LIBS})
#add_executable(dump_torrent
#        dump_torrent.cpp)
#target_link_libraries(dump_torrent ${CONAN_LIBS})

#add_executable(maglink2torrent maglink2torrent.cpp)
#target_link_libraries(maglink2torrent ${CONAN_LIBS})
