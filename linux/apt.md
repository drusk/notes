Finding out which package provides a file
-----------------------------------------
Use apt-file to search for files in APT packages.

```
sudo apt-get install apt-file
apt-file update
```

Example usage:

```
apt-file search /usr/include/GL/glut.h
freeglut3-dev: /usr/include/GL/glut.h
```