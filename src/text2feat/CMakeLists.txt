add_library(text2feat SHARED text2feat.cpp)
INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR}/../../build/crfsuite/installed/include)
LINK_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR}/../../build//crfsuite/installed/lib ${CMAKE_CURRENT_SOURCE_DIR}/../../build/liblbfgs-1.10/installed/lib)
target_link_libraries(text2feat text_util)
target_include_directories (text2feat PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
