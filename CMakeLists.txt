cmake_minimum_required(VERSION 3.6)
project(superpromise)

enable_testing()

# TODO: We should instead be using the 'CXX_STANDARD' and
# 'CXX_STANDARD_REQUIRED' target attributes. For the concepts part, I think we
# need to verify that the compiler is GNU and add this flag to the target which
# requires it somehow.
set(CMAKE_CXX_FLAGS "-std=c++1z -fconcepts")

# Bootstrap cms
add_subdirectory(cms)
get_target_property(cms_modulePath cms CMAKE_MODULE_PATH)
set(CMAKE_MODULE_PATH "${cms_modulePath};${CMAKE_MODULE_PATH}")

include(cmsi_import)

cmsi_import(apl)
cmsi_import(cms)
cmsi_import(dpl)
