cmake_minimum_required(VERSION 3.16)
enable_language(CUDA)
project(CUDA_Introduction LANGUAGES CUDA CXX)

set(CMAKE_CUDA_STANDARD 14)

add_executable(simple_start add_cuda.cu)
set_target_properties(
        simple_start
        PROPERTIES CUDA_SEPARABLE_COMPILATION ON
)