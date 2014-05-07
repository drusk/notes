Typical Makefile structure
--------------------------
```
CC      = g++
CFLAGS  = -g -Wall
LDFLAGS = -lm -lpthreads

all: hello clean

hello: hello.o
	$(CC) -o $@ $^ $(LDFLAGS)

hello.o: hello.cpp hello.h
	$(CC) -c $(CFLAGS) $<

.PHONY: clean cleanest

clean:
	rm *.o

cleanest: clean
	rm hello
```

Special Symbols
---------------
```$@``` the name of the target

```$^``` list of prerequisites with duplicates removed

```$<``` the first prerequisite

Formatting
----------
Note that tabs are **REQUIRED**.  Spaces for indenting will result in errors.