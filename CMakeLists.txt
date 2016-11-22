cmake_minimum_required(VERSION 3.6)
project(superpromise)

enable_testing()

set(CMAKE_CXX_FLAGS "-std=c++1z -fconcepts")

set(CMAKE_MODULE_PATH
  "${CMAKE_CURRENT_LIST_DIR}/cms/cmsfm;${CMAKE_MODULE_PATH}")

if(NOT TARGET apl)
  add_subdirectory(apl)
endif()

if(NOT TARGET dpl)
  add_subdirectory(dpl)
endif()
