# Copyright 2009-2021 Intel Corporation
# SPDX-License-Identifier: Apache-2.0

cmake_minimum_required(VERSION 3.0)

project(HelloEmbree LANGUAGES CXX)

add_executable(hello_embree hello_embree.cpp)

find_package(embree 3.0)
target_link_libraries(hello_embree embree)