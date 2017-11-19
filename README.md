# Mandelbrot-Set

This is a code taken from this url: https://rosettacode.org/wiki/Mandelbrot_set#C to make a Mandelbrot Fractal and used to parallelize it using MPI.

I'm using Ubuntu 16.04 to make this program. 
The version of MPI that I'm using is 3.2.

This program is only tested in Ubuntu 16.04

np = number of processors you want to use.

# How to compile Set.c
Compile the program using the command:
- mpicc set.c -o set

or using:
- gcc set.c -o set


# How to run Set.c
After compiling Set.c you need to run the program using the command:
- mpirun -np 2 ./set

or using:
- ./set

After running the program you'll have a image call "mandelbrotSet.ppm"

# How to compile ParallelFractal.c
Compile the program using the command:
- mpicc ParallelFractal.c -o fractal

# How to run ParallelFractal.c
After compiling ParallelFractal.c you need to run the program using the command:
- mpirun -np 2 ./fractal

After running the program you'll have a image call "mandelbrotSet.ppm"
