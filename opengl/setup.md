Technologies
------------
* C++
* OpenGL
* GLFW (configures OpenGL context)
* GLEW (dynamically link available OpenGL functions)
* GLM (vectors and matrices library)

Install GLFW
------------
* Download source from http://www.glfw.org/
* Unizp
* Install dependencies:

```
sudo apt-get install cmake xorg-dev libglu1-mesa-dev
```

* Build and install

```
cmake -G "Unix Makefiles"
make
sudo make install
```

Install GLEW
------------
Download source from http://glew.sourceforge.net/

Untar, make, make install

Install GLM
-----------
```
sudo apt-get install libglm-dev
```
