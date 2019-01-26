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

