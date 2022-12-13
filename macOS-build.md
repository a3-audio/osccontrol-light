The following instructions can help to build the OSCLight Plugins on macOS.

This has been testet on the following system:

- macOS Ventura 13.0.1
- xcode Version 14.1 (14B47b)
- juce-7.0.3-osx
- cmake version 3.25.1

brew install cmake
arch -arm64 brew install cmake

gh repo clone a3-audio/osccontrol-light

export JUCE_DIR=/Users/YOURNAME/local/juce/lib/cmake/JUCE-7.0.3/

 brew install yaml-cpp

./build_plugins.sh -v -j16 iem-encoder-ch1 iem-encoder-ch2 iem-encoder-ch3 iem-encoder-ch4

brew install liblo

oscdump 2352