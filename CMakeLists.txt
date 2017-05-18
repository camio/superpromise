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

# ----------------------------------------------------------------------------
# Copyright 2017 Bloomberg Finance L.P.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
