cmake_minimum_required (VERSION 2.6)
project (ExeFile)
set(SOURCES ExeFile.cpp )
include ("${CLR_INTEROP_TEST_ROOT}/Interop.cmake") 

# add the executable
add_executable (ExeFile ${SOURCES})
target_link_libraries(ExeFile ${LINK_LIBRARIES_ADDITIONAL}) 

# add the install targets
install (TARGETS ExeFile DESTINATION bin)
