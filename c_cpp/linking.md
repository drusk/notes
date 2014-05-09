Order
-----
Order is important when linking.  Put dependent libraries first.  That is, if A depends on B then do:
```
gcc prog.o -lA -lB -o prog
```

Third party libraries
---------------------
Here is an example of finding requirements of a third party library (GLFW)

```
pkg-config --libs --cflags --print-requires-private glfw3
```

Output:
```
x11
xrandr
xi
xxf86vm
gl
-I/usr/local/include -I/usr/include/libdrm  -L/usr/local/lib -lglfw3
```

So when linking make sure to include these using ```-lX11 -lXrandr ...```