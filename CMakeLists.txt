cmake_minimum_required(VERSION 3.23)
project(juceCmake)

set(CMAKE_CXX_STANDARD 17)

add_subdirectory(JUCE)

add_executable(juceCmake main.cpp)

target_link_libraries(juceCmake
    juce::juce_audio_basics
    juce::juce_audio_devices
    juce::juce_audio_formats
    juce::juce_audio_processors
    juce::juce_audio_utils
    juce::juce_core
    juce::juce_data_structures
    juce::juce_events
    juce::juce_graphics
    juce::juce_gui_basics
    juce::juce_gui_extra
)