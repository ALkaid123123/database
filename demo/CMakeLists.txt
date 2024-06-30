cmake_minimum_required(VERSION 3.9)
# Keep the version below in sync with the one in db.h
project(testdb VERSION 1.23.0 LANGUAGES C CXX)
include_directories(../include)

add_executable(demo1 test.cpp)
target_link_libraries(demo1 /home/zhe/leveldb/demo/lib/libleveldb.a)
target_link_libraries(demo1 -lpthread)