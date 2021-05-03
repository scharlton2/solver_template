cmake_minimum_required (VERSION 3.9)

project (hello Fortran)

include(GNUInstallDirs)

add_executable(hello src/Hello.f90)

install (TARGETS hello DESTINATION "${CMAKE_INSTALL_BINDIR}")

include(CTest)

add_test(TestRun hello)


