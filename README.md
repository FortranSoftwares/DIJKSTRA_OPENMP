# DIJKSTRA_OPENMP

## Dijkstra Graph Distance Algorith using OpenMP

DIJKSTRA_OPENMP is a FORTRAN77 program which illustrates the use of the OpenMP application program interface by implementing Dijkstra's minimum graph distance algorithm.

The program is an interesting example, because it does not involve parallelization of a loop. Instead, a parallel region is defined, and the nodes of the graph are divided up among the threads. The resulting parallel algorithm naturally requires some of the more advanced OpenMP directives, including critical, single and barrier, in order to work correctly.

The actual graph that is analyzed is very small (6 nodes), but of course the same algorithm would work for larger graphs. The point is rather to see how the OpenMP directives can be put together correctly.

## Licensing:
The computer code and data files described and made available on this web page are distributed under the MIT License

## Reference:

- Peter Arbenz, Wesley Petersen,
Introduction to Parallel Computing - A practical guide with examples in C,
Oxford University Press,
ISBN: 0-19-851576-6,
LC: QA76.58.P47.

- Rohit Chandra, Leonardo Dagum, Dave Kohr, Dror Maydan, Jeff McDonald, Ramesh Menon,
Parallel Programming in OpenMP,
Morgan Kaufmann, 2001,
ISBN: 1-55860-671-8,
LC: QA76.642.P32.

- Barbara Chapman, Gabriele Jost, Ruud vanderPas, David Kuck,
Using OpenMP: Portable Shared Memory Parallel Processing,
MIT Press, 2007,
ISBN13: 978-0262533027,
LC: QA76.642.C49.
The OpenMP web site
OpenMP Architecture Review Board,
OpenMP Application Program Interface,
Version 3.0,
May 2008.

## Source code:
dijkstra_openmp.f, the source code;

## Examples and Tests:

### DIJKSTRA_LOCAL_GFORTRAN compiles, links, loads and runs the program using 1, 2 and 4 threads, the local interactive environment, and the GNU GFORTRAN compiler.

- dijkstra_local_gfortran.sh, BASH commands.
- dijkstra_local_gfortran_output.txt, the output file;

### DIJKSTRA_LOCAL_IFORT compiles, links, loads and runs the program using 1, 2 and 4 threads, the local interactive environment, and the Intel IFORT compiler.

- dijkstra_local_ifort.sh, BASH commands.
- dijkstra_local_ifort_output.txt, the output file;

### DIJKSTRA_ITHACA_GFORTRAN compiles, links, loads and runs the program using 1, 2 and 4 threads, using the PBS queueing system on Virginia Tech's Ithaca cluster, and the GNU GFORTRAN compiler.

- dijkstra_ithaca_gfortran.sh, BASH commands.
- dijkstra_ithaca_gfortran_output.txt, the output file;

### DIJKSTRA_ITHACA_IFORT compiles, links, loads and runs the program using 1, 2 and 4 threads, using the PBS queueing system on Virginia Tech's Ithaca cluster, and the Intel IFORT compiler.

- dijkstra_ithaca_ifort.sh, BASH commands.
- dijkstra_ithaca_ifort_output.txt, the output file;
