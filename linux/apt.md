# Finding out which package provides a file

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

# Purging packages

To find out what package a file belongs to:

```
dpkg -S /path/to/file
```

Then to remove everything including config files (except config or data 
files in user's home directory):

```
sudo apt-get purge packagename
```

Note this will not remove dependencies installed when the package was
installed. To get rid of orphaned packages use:

```
sudo apt-get autoremove
```

