# OpenGL_CLion_Linux_Setup
Simple Step by step setup for OpenGL (GLFW) using CMake and CLion on linux. Simple CMake Template and Test Code included

//// The setup ////

Download GLFW from here, https://www.glfw.org/

Next install dependancies via

sudo apt-get install cmake xorg-dev libglu1-mesa-dev

Next make, open the directory where you extracted GLFW.(Version)

Type:
cmake -G "Unix Makefiles"
(Note install cmake if you dont have)

Type:
sudo make

Type:
sudo make install

You should now be set up to create your generic CMakefile and start using OpenGL and the GLFW library.

CMake template made for CLion and testable OpenGL file in repo.

To add GLEW libraries (Reccomended) open terminal,

Type:
sudo apt-get install libglew-dev

To add GLEW to your CMake file simply follow the same steps that can be seen for GLFW,

Ie add:
find_package (GLEW REQUIRED)

include_directories(${GLEW_INCLUDE_DIRS})

Then in the target libraries, include ${GLEW_LIBRARY}
