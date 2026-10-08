cmake_minimum_required(VERSION 3.16)

project(donstu_os_cpp_scheduler LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(donstu_os_cpp_scheduler main.cpp)

include(GNUInstallDirs)
install(TARGETS donstu_os_cpp_scheduler
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
