cmake_minimum_required(VERSION 2.8)

add_subdirectory(Adafruit-GFX-Library)

add_library(SSD1306 Adafruit_SSD1306.cpp)

target_link_libraries(SSD1306 Adafruit_GFX)

include_directories(Adafruit-GFX-Library)

