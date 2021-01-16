# OpenGL Game Engine Development in Visual Studio Code

This repo contains the source from my OpenGL Game Engine tutorials using SDL &amp; Visual Studio Code. Tailored at those who are new to graphics programming, and possess knowledge of object-orientated development/C++, I have done my best to explain everything I've included, but cited further sources which will explain on these topics in greater detail.

# Table of Contents
1. [Required Tools](#tools)
2. [Application Dependencies](#dependencies)
    1. [MinGW/GCC](#gcc)
    2. [SDL2](#sdl)
    3. [OpenGL](#opengl)
    4. [GLEW](#glew)
    5. [GLM](#glm)
    6. [OpenAL](#openal)
    7. [Bullet](#bullet)
3. [Documentation](#documentation)

# Required Tools <a name="tools"></a>

1. [Visual Studio Code](https://code.visualstudio.com/)
2. [Git/Github](https://desktop.github.com/)
3. (Optional) [Vmware Player Virtual Machine](https://www.vmware.com/products/player/playerpro-evaluation.html) for testing your code on different operating systems.
4. (Optional) [Windows (VM Image)](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/)
5. (Optional) [Linux (Ubuntu VM Image)](https://www.ubuntu.com/download/desktop)

https://github.com/kbrawley95/VSCode-OpenGL-Game-Engine
# Application Dependencies <a name="dependencies"></a>

## 1. MinGW/GNU Compiler Collection (GCC) <a name="gcc"></a>

In order to execute our code, we will require GNU utilities. This contains numerous compilers for various languages (e.g. Fortran, C++ etc.) classified as the **GNU Compiler Collection (GCC)**, and their respective debuggers.

### Linux: Debian & Ubuntu 14.04 and above: 

```
Sudo apt-get install g++ -y
```

**NB: This distribution of linux should have the GCC installed, provided you updated your system post-install:**

```
Sudo apt-get update && sudo apt-get upgrade -y
```

### MacOs: 
My knowledge of MacOS/OSX is limited. However, this github repo detailing an installer for the GCC (incorporating xcode) appears to be a good place to [start](https://github.com/kennethreitz/osx-gcc-installer).

### Windows: 
Windows does not contain these tools as standard. Fortunately, we can install a minimised version of GNU called **Minimalist GNU for Windows** ([MinGW](https://sourceforge.net/projects/mingw/files/latest/download?source=files)). This will supply all the dependecies, and tools to simulate a GNU-like environment, add these tools to your system path, and execute them through the **Comand Line Interface (CLI)** as you would on linux.



## 2. SDL <a name ="sdl"></a>
### Linux: Debian & Ubuntu 14.04 and above: 

```
sudo apt-get install libsdl2{,-mixer,-image,-ttf}-dev
```

**NB:** Further dependencies for each of these libraries can be installed by changing the above command with following:




### MacOs: 

On Mac OS X, install SDL2 via Homebrew like so: brew install sdl2{,_image,_ttf,_mixer}

### Windows: 

The [SDL2 Headers](http://libsdl.org/download-2.0.php) can be fetched directly from the SDL website. 



## 3. OPENGL <a name ="opengl"></a>

The **Open Graphics Library (OpenGL)** is a specification of various operations (functions) that facilite the rendering and manipulation of images, and other graphical niceties on our displays. The functions and the specification as a whole is maintain by the Khronos Group; a body of various industry experts, GPU manufactors, and related companies that collaborate to continually improve upon the capabilties of OpenGL -and the core requirements that supporting hardware should implement. The key word there is 'should'. 

As OpenGL is **NOT** actually set of classes/libaries or **Application Programming Interface (API)**, it falls upon the Graphics Card Manufactors to implement the defined requirements i.e. they create the libraries, and classes that help you to run your favourite games via software called drivers. Installing these drivers will allow you to access core OpenGL functuality, and any further extensions to the specification which were supported by your Graphics card at the time of release. 

### Linux: Debian & Ubuntu 14.04 and above: 

Linux distributions utilise the an open-source implementation of OpenGL called Mesa. Mesa provides drivers that will enable you to utilise the core OpenGL features supported by your gpu: 

```
sudo apt-get install libgl1-mesa-dri:i386, libgl1-mesa-glx:i386, libc6:i386
```

**NB:**: Your properity drivers downloaded during your installation of your given Linux distro maybe enough to start using OpenGL operation in your code. But I'd advice installing these drivers to save further complication down the road.




### MacOs: ?


### Windows:

On Windows the setup is much easily. Simply install the latest graphics drivers supported by your current graphics card/GPU. Clicking the relevant manufactor below will take your to the necessary download pages:

1. [AMD](https://www.amd.com/en/support)
2. [Intel](https://www.intel.com/content/www/us/en/support/articles/000005629/graphics.html)
3. [Nvidia](https://developer.nvidia.com/opengl)


## 4. GLEW <a name ="glm"></a>

The OpenGL Extension Wrangler Library

[Download](http://glew.sourceforge.net/install.html)

## 5. GLM <a name ="glm"></a>

GLSL + Optional features = OpenGL Mathematics (GLM)
A C++ mathematics library for graphics programming. 

[Download](http://glm.g-truc.net/0.9.5/index.html)

## 6. OPENAL <a name ="openal"></a>

OpenAL is a cross-platform 3D audio API appropriate for use with gaming applications and many other types of audio applications.

The library models a collection of audio sources moving in a 3D space that are heard by a single listener somewhere in that space. The basic OpenAL objects are a Listener, a Source, and a Buffer. There can be a large number of Buffers, which contain audio data. Each buffer can be attached to one or more Sources, which represent points in 3D space which are emitting audio. There is always one Listener object (per audio context), which represents the position where the sources are heard -- rendering is done from the perspective of the Listener.

[Download](http://www.openal.org/)

## 7. BULLET <a name ="bullet"></a>

Bullet Physics SDK: real-time collision detection and multi-physics simulation for VR, games, visual effects, robotics, machine learning etc.

[Download](https://github.com/bulletphysics/bullet3/releases)


# Documentation <a name="documentation"></a>
For more information on the materials provided, refer to the sources below:

### Minimalist GNU for Windows
* [MinGW](http://mingw.org/)

### OpenGL & Related Libraries
* [Bullet Physics Documentation](https://github.com/bulletphysics/bullet3)
* [GLEW](https://github.com/nigels-com/glew#authors)
* [GLM](http://glm.g-truc.net/0.9.5/api/index.html)
* [OpenAL](http://www.openal.org/documentation/)
* [OpenGL](https://www.opengl.org/)
* [SDL2](http://wiki.libsdl.org/FrontPage)

### Visual Studio Code
* [VS Portable](http://gareth.flowers/vscode-portable/)
* [Debugging](http://code.visualstudio.com/docs/editor/debugging)
* [Integrated Terminal](https://code.visualstudio.com/docs/editor/integrated-terminal)
* [Tasks](http://code.visualstudio.com/docs/editor/tasks)
