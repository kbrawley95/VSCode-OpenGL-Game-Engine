# VSCode OpenGL Game Engine
Repo containing the source from my OpenGL Game Engine tutorials using SDL &amp; Visual Studio Code

## Dependencies

### 1. MinGW/GNU Compiler Collection (GCC)
#### Linux: Debian & Ubuntu 14.04 and above: 

```
Sudo apt-get install g++ -y
```

**NB: This distribution of linux should have the GCC installed, provide you updated your system post-install:**

```
Sudo apt-get update && sudo apt-get upgrade -y
```

#### MacOs: 

#### Windows: 
In order to execute our code on windows, we will require GNU-like utilities. This contains numerous compilers classed as the **GNU Compiler Collection (GCC)** and their respective debuggers. Windows does not contain these tools as standard. Fortunately, we can install a minimised version of GNU called **Minimalist GNU for Windows** ([MinGW](https://sourceforge.net/projects/mingw/files/latest/download?source=files)).











### 2. SDL
#### Linux: Debian & Ubuntu 14.04 and above: 

```
Sudo apt-get install libsdl2{,-mixer,-image,-ttf}-dev
```
**Note: Ubuntu 14.04 currently has broken header file in the SDL2 package that disables people from compiling against it. It will be needed to either patch the header file or install SDL2 from source.**

#### MacOs: 

On Mac OS X, install SDL2 via Homebrew like so: brew install sdl2{,_image,_ttf,_mixer}

#### Windows: 



[SDL2 Headers](http://libsdl.org/download-2.0.php)


## Documentation
For more information on the materials provided, refer to the sources below:

* VS Portable: http://gareth.flowers/vscode-portable/
* MinGW (Minimalist GNU for Windows): http://mingw.org/
* Debugging: http://code.visualstudio.com/docs/editor/debugging
* Integrated Terminal: https://code.visualstudio.com/docs/editor/integrated-terminal
* Tasks: http://code.visualstudio.com/docs/editor/tasks
* OpenGL Documentation: https://www.opengl.org/
