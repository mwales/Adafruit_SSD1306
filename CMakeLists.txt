cmake_minimum_required(VERSION 2.8)

add_library(SSD1306 Adafruit_SSD1306.cpp)

include_directories(Adafruit-GFX-Library ArduinoForLinux)

add_subdirectory(Adafruit-GFX-Library ArduinoForLinux)

target_link_libraries(SSD1306 Adafruit_GFX arduino)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} --std=c++11 -Wall")

set(CMAKE_CXX_COMPILER "clang++")

