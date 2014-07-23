Ubuntu Install
--------------
```
sudo apt-get install valgrind
```

Memory Leaks
------------
```
valgrind --leak-check=yes <executable>
```

Profiling
---------
```
valgrind --tool=callgrind <executable>
```

When it finishes it will output a file called callgrind.out.xxx where xxx is some
number.  These results can be visualized using kcachegrind.
```
sudo apt-get install kcachegrind
```

then:
```
kcachegrind callgrind.out.xxx
```