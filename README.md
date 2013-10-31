EMFlow
======
Compute the drainage network on digital elevation models stored in external memory.

Compilation
-----------
To compile, run **make** or use:

    g++ -O3 -o EMFlow hydrogEmFillFlow.cpp lz4.c

Running
-------
To run, need set up the amount of memory available (line 77) and tiled block size (line 76) on code hydrogEmFillFlow.cpp and need set up the amount of memory available (line 44) and tiled block size (line 43) on code flow.cpp.

    ./EMFlow nrows terrain_name.hgt

About the Script
----------------
.creat folder tiles to store temporary tiles, the tiles folder is necessary for the program operation
.creat folder tempos to store the running time
.Run the program for several instances and stores the runtime

Output
------
As a result it is given a file named flow.hgt containing the accumulated flow with 2 bytes.
