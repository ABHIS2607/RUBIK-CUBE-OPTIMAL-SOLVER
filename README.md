# RUBIK-CUBE-OPTIMAL-SOLVER
This project implements two solving algorithms for Rubik's Cube: Richard Korf's optimal solver and Thistlethwaite's quick solver.
Algorithms
Optimal Solver (Korf's Algorithm)
Uses IDA* (Iterative Deepening A*) with pattern databases for corner and edge permutations.
Corner database: 88,179,840 states, stored in 42MB.
Converts permutations to factorial base for efficient indexing.
Quick Solver (Thistlethwaite's Algorithm)
Implements a modified Thistlethwaite algorithm with a maximum of 46 moves.
Uses pattern databases to transition between groups of simpler cube configurations.
Groups: 0 (scrambled), 1 (edge orientation fixed), 2 (corners and slice edges positioned).
Each transition uses a specific pattern database for move estimation.
Performance
Optimal Solver: Solves any cube in 20 moves or fewer, but can take longer for complex scrambles.
Quick Solver: Solves any cube in at most 46 moves, optimized for speed.

