cmake_minimum_required(VERSION 3.20)
project("MyApp" VERSION 1.0)

set(CMAKE_CXX_STANDARD 14)

set(CMAKE_PREFIX_PATH "C:/Qt/5.15.2/mingw81_64/lib/cmake")

find_package(Qt5 COMPONENTS
        Core
        gui
        Widgets
        REQUIRED)

add_executable(MyApp main.cpp)

target_link_libraries(MyApp
        Qt5::Core
        Qt5::Gui
        Qt5::Widgets)





