set(CMAKE_SYSTEM_NAME Generic)
set(CMAKE_C_COMPILER_WORKS 1)
set(CMAKE_CXX_COMPILER_WORKS 1)

find_package(eosio.cdt)

cmake_minimum_required(VERSION 3.5)
project(eospetgameio VERSION 0.0.0.1)

add_contract(eospetgameio eospetgameio src/eospetgameio.cpp)

target_include_directories(eospetgameio.wasm PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)