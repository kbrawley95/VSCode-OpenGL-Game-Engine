# OpenGL Game Engine Development in Visual Studio Code

## Overview

This repo contains the source from my OpenGL Game Engine tutorials using SDL &amp; Visual Studio Code. Tailored at those who are new to graphics programming, and possess knowledge of object-orientated development/C++, I have done my best to explain everything I've included, but cited further sources which will explain on these topics in greater detail.

# Table of Contents
1. [Required Tools](#tools)
2. [Application Dependencies](#dependencies)
    1. [MinGW/GCC](#gcc)
    2. [SDL2](#sdl)
    3. [OpenGL])(#opengl)
3. [Documentation](#documentation)

## Required Tools <a name="tools"></a>

1. [Visual Studio Code](https://code.visualstudio.com/)
2. [Git/Github](https://desktop.github.com/)
3. (Optional) [Vmware Player Virtual Machine](https://www.vmware.com/products/player/playerpro-evaluation.html) for testing your code on different operating systems.
### Virtual Machines Images
4. [Windows](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/)
4. [Linux (Ubuntu)](https://www.ubuntu.com/download/desktop)


## Application Dependencies <a name="dependencies"></a>

### 1. MinGW/GNU Compiler Collection (GCC) <a name="gcc"></a>

In order to execute our code, we will require GNU utilities. This contains numerous compilers for various languages (e.g. Fortran, C++ etc.) classified as the **GNU Compiler Collection (GCC)**, and their respective debuggers.

#### Linux: Debian & Ubuntu 14.04 and above: 

```
Sudo apt-get install g++ -y
```

**NB: This distribution of linux should have the GCC installed, provided you updated your system post-install:**

```
Sudo apt-get update && sudo apt-get upgrade -y
```

#### MacOs: 
My knowledge of MacOS/OSX is limited. However, this github repo detailing an installer for the GCC (incorporating xcode) appears to be a good place to [start](https://github.com/kennethreitz/osx-gcc-installer).

#### Windows: 
Windows does not contain these tools as standard. Fortunately, we can install a minimised version of GNU called **Minimalist GNU for Windows** ([MinGW](https://sourceforge.net/projects/mingw/files/latest/download?source=files)). This will supply all the dependecies, and tools to simulate a GNU-like environment, add these tools to your system path, and execute them through the **Comand Line Interface (CLI)** as you would on linux.











### 2. SDL <a name ="sdl"></a>
#### Linux: Debian & Ubuntu 14.04 and above: 

```
sudo apt-get install libsdl2{,-mixer,-image,-ttf}-dev
```

**NB:** Further dependencies for each of these libraries can be installed by changing the above command with following:




#### MacOs: 

On Mac OS X, install SDL2 via Homebrew like so: brew install sdl2{,_image,_ttf,_mixer}

#### Windows: 



[SDL2 Headers](http://libsdl.org/download-2.0.php)



### 3. OPENGL <a name ="opengl"></a>

The **Open Graphics Library (OpenGL)** is a specification of various operations (functions) that facilite the rendering and manipulation of images, and other graphical niceties on our displays. The functions and the specification as a whole is maintain by the Khronos Group; a body of various industry experts, GPU manufactors, and related companies that collaborate to continually improve upon the capabilties of OpenGL -and the core requirements that supporting hardware should implement. The key word there is 'should'. 

As OpenGL is **NOT** actually set of classes/libaries or **Application Programming Interface (API)**, it falls upon the Graphics Card Manufactors to implement the defined requirements i.e. they create the libraries, and classes that help you to run your favourite games via software called drivers. Installing these drivers will allow you to access core OpenGL functuality, and any further extensions to the specification which were supported by your Graphics card at the time of release. 

#### Linux: Debian & Ubuntu 14.04 and above: 

Linux distributions utilise the an open-source implementation of OpenGL called Mesa. Mesa provides drivers that will enable you to utilise the core OpenGL features supported by your gpu: 

```
sudo apt-get install libgl1-mesa-dri:i386, libgl1-mesa-glx:i386, libc6:i386
```

**NB:**: Your properity drivers downloaded during your installation of your given Linux distro maybe enough to start using OpenGL operation in your code. But I'd advice installing these drivers to save further complication down the road.




#### MacOs: ?


#### Windows:

On Windows the setup is much easily. Simply install the latest graphics drivers supported by your current graphics card/GPU. Clicking the relevant manufactor below will take your to the necessary download pages:

1. [AMD]()
2. [Intel)()
3. [Nvidia]()






## Documentation <a name="documentation"></a>
For more information on the materials provided, refer to the sources below:

* VS Portable: http://gareth.flowers/vscode-portable/
* MinGW (Minimalist GNU for Windows): http://mingw.org/
* Debugging: http://code.visualstudio.com/docs/editor/debugging
* Integrated Terminal: https://code.visualstudio.com/docs/editor/integrated-terminal
* Tasks: http://code.visualstudio.com/docs/editor/tasks
* OpenGL Documentation: https://www.opengl.org/
