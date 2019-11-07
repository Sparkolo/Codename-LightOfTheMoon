# Codename: Light Of The Moon
Sprite-based isometric bullet hell arena boss battle game, made in SimpleRenderEngine as a student project for the Game Programming course at ITU (2019).

## Setup
[SimpleRenderEngine](https://github.com/mortennobel/SimpleRenderEngineProject) is required in order to build this project.  

To build this project in SimpleRenderEngine, first setup the engine as described in its GitHub page.  

Once done, simply clone this repository into the `SimpleRenderEngineProject/project/` folder by running the command `git clone https://github.com/Sparkolo/Codename-LightOfTheMoon.git` on your terminal.  

To correctly build the project, open the file `SimpleRenderEngineProject/projects/CMakeLists.txt` and add the following line before the last "IF": `add_subdirectory(Codename-LightOfTheMoon)`  

### Leak Detection

This project is developed on Windows 10 with [Visual Studio 2019 Community](https://visualstudio.microsoft.com/it/downloads/) as IDE. To properly run the leak detection tool, install [Visual Leak Detector](https://kinddragon.github.io/vld/) by using the installer found on the website. Make sure your installation folder is the following: `C:/Program Files (x86)/Visual Leak Detector/`  

In case you do not run the project on Windows 10 + Visual Studio, remove from the project's `CMakeLists.txt` the `# Visual Leak Detector` section and delete `vld` from the `target_link_libraries(LOTM ${all_libs} vld)` line.  
Also, in the `main.cpp` remove this line of code: `#include <vld.h>`.  
**IF YOU REMOVE VLD FROM YOUR LOCAL PROJECT, DO NOT COMMIT/PUSH THE CHANGES ABOVE!**

## Credits
* Alberto Giudice - [algi@itu.dk](algi@itu.dk)
* Francesco Frassinetti - [fraf@itu.dk](fraf@itu.dk)
* Jeppe Faber - [jepf@itu.dk](mailto:jepf@itu.dk)