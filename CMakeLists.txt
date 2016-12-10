cmake_minimum_required(VERSION 3.5)
project(NewProject)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    Builds/LinuxMakefile/Makefile
    Builds/MacOSX/build/Debug/NewProject.component/Contents/MacOS/NewProject
    Builds/MacOSX/build/Debug/NewProject.component/Contents/Resources/NewProject.rsrc
    Builds/MacOSX/build/Debug/NewProject.component/Contents/Resources/RecentFilesMenuTemplate.nib
    Builds/MacOSX/build/Debug/NewProject.component/Contents/Info.plist
    Builds/MacOSX/build/Debug/NewProject.component/Contents/PkgInfo
    Builds/MacOSX/build/Debug/NewProject.vst/Contents/MacOS/NewProject
    Builds/MacOSX/build/Debug/NewProject.vst/Contents/Resources/RecentFilesMenuTemplate.nib
    Builds/MacOSX/build/Debug/NewProject.vst/Contents/Info.plist
    Builds/MacOSX/build/Debug/NewProject.vst/Contents/PkgInfo
    Builds/MacOSX/build/Debug/libNewProject.a
    Builds/MacOSX/halabae.xcodeproj/project.xcworkspace/xcuserdata/zacharyhalaby.xcuserdatad/UserInterfaceState.xcuserstate
    Builds/MacOSX/halabae.xcodeproj/project.xcworkspace/xcuserdata/zacharyhalaby.xcuserdatad/WorkspaceSettings.xcsettings
    Builds/MacOSX/halabae.xcodeproj/project.xcworkspace/contents.xcworkspacedata
    "Builds/MacOSX/halabae.xcodeproj/xcuserdata/zacharyhalaby.xcuserdatad/xcschemes/halabae (All).xcscheme"
    "Builds/MacOSX/halabae.xcodeproj/xcuserdata/zacharyhalaby.xcuserdatad/xcschemes/halabae (AU).xcscheme"
    "Builds/MacOSX/halabae.xcodeproj/xcuserdata/zacharyhalaby.xcuserdatad/xcschemes/halabae (Shared Code).xcscheme"
    "Builds/MacOSX/halabae.xcodeproj/xcuserdata/zacharyhalaby.xcuserdatad/xcschemes/halabae (VST).xcscheme"
    Builds/MacOSX/halabae.xcodeproj/xcuserdata/zacharyhalaby.xcuserdatad/xcschemes/xcschememanagement.plist
    Builds/MacOSX/halabae.xcodeproj/project.pbxproj
    Builds/MacOSX/NewProject.xcodeproj/project.xcworkspace/xcuserdata/zacharyhalaby.xcuserdatad/UserInterfaceState.xcuserstate
    Builds/MacOSX/NewProject.xcodeproj/project.xcworkspace/contents.xcworkspacedata
    "Builds/MacOSX/NewProject.xcodeproj/xcuserdata/zacharyhalaby.xcuserdatad/xcschemes/NewProject (All).xcscheme"
    "Builds/MacOSX/NewProject.xcodeproj/xcuserdata/zacharyhalaby.xcuserdatad/xcschemes/NewProject (AU).xcscheme"
    "Builds/MacOSX/NewProject.xcodeproj/xcuserdata/zacharyhalaby.xcuserdatad/xcschemes/NewProject (Shared Code).xcscheme"
    "Builds/MacOSX/NewProject.xcodeproj/xcuserdata/zacharyhalaby.xcuserdatad/xcschemes/NewProject (VST).xcscheme"
    Builds/MacOSX/NewProject.xcodeproj/xcuserdata/zacharyhalaby.xcuserdatad/xcschemes/xcschememanagement.plist
    Builds/MacOSX/NewProject.xcodeproj/project.pbxproj
    Builds/MacOSX/halabae.entitlements
    Builds/MacOSX/Info-AU.plist
    Builds/MacOSX/Info-VST.plist
    Builds/MacOSX/NewProject.entitlements
    Builds/MacOSX/RecentFilesMenuTemplate.nib
    JuceLibraryCode/AppConfig.h
    JuceLibraryCode/juce_audio_basics.cpp
    JuceLibraryCode/juce_audio_basics.mm
    JuceLibraryCode/juce_audio_devices.cpp
    JuceLibraryCode/juce_audio_devices.mm
    JuceLibraryCode/juce_audio_formats.cpp
    JuceLibraryCode/juce_audio_formats.mm
    JuceLibraryCode/juce_audio_plugin_client_AAX.cpp
    JuceLibraryCode/juce_audio_plugin_client_AAX.mm
    JuceLibraryCode/juce_audio_plugin_client_AU_1.mm
    JuceLibraryCode/juce_audio_plugin_client_AU_2.mm
    JuceLibraryCode/juce_audio_plugin_client_AUv3.mm
    JuceLibraryCode/juce_audio_plugin_client_RTAS_1.cpp
    JuceLibraryCode/juce_audio_plugin_client_RTAS_2.cpp
    JuceLibraryCode/juce_audio_plugin_client_RTAS_3.cpp
    JuceLibraryCode/juce_audio_plugin_client_RTAS_4.cpp
    JuceLibraryCode/juce_audio_plugin_client_RTAS_utils.cpp
    JuceLibraryCode/juce_audio_plugin_client_Standalone.cpp
    JuceLibraryCode/juce_audio_plugin_client_utils.cpp
    JuceLibraryCode/juce_audio_plugin_client_VST2.cpp
    JuceLibraryCode/juce_audio_plugin_client_VST3.cpp
    JuceLibraryCode/juce_audio_plugin_client_VST_utils.mm
    JuceLibraryCode/juce_audio_processors.cpp
    JuceLibraryCode/juce_audio_processors.mm
    JuceLibraryCode/juce_core.cpp
    JuceLibraryCode/juce_core.mm
    JuceLibraryCode/juce_cryptography.cpp
    JuceLibraryCode/juce_cryptography.mm
    JuceLibraryCode/juce_data_structures.cpp
    JuceLibraryCode/juce_data_structures.mm
    JuceLibraryCode/juce_events.cpp
    JuceLibraryCode/juce_events.mm
    JuceLibraryCode/juce_graphics.cpp
    JuceLibraryCode/juce_graphics.mm
    JuceLibraryCode/juce_gui_basics.cpp
    JuceLibraryCode/juce_gui_basics.mm
    JuceLibraryCode/juce_gui_extra.cpp
    JuceLibraryCode/juce_gui_extra.mm
    JuceLibraryCode/juce_opengl.cpp
    JuceLibraryCode/juce_opengl.mm
    JuceLibraryCode/juce_video.cpp
    JuceLibraryCode/juce_video.mm
    JuceLibraryCode/JuceHeader.h
    JuceLibraryCode/ReadMe.txt
    Source/PluginEditor.cpp
    Source/PluginEditor.h
    Source/PluginProcessor.cpp
    Source/PluginProcessor.h
    NewProject.jucer)

add_executable(NewProject ${SOURCE_FILES})