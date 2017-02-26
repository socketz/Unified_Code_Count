project(UCC)

file(GLOB FILES *.h *.cpp)
add_executable(UCC ${FILES})
include(../cmake/BuildSettings.cmake)
