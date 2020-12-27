# SDL/SDL2 and Bazel example

It took me a bit to figure out how to set up a Bazel C++ build for SDL.


This seems to work on a Linux machine after installing `libsdl2-dev`
with `apt-get`.

```
sudo apt-get install libsdl2-dev
```

Key bit is the `linkopts = ["-lSDL2"]` directive in `cc_binary`

Hopefully this shows up for someone doing similar Google searches in the future.
