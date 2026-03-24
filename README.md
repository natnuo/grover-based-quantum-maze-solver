# Oracle design and complexity analysis for a Grover-based quantum maze solver

**Date Written:** December 2025

**Authors:** Advithi Baddam, Julia Pryor, Revati Tambe, and Nathan Tao (all equal contributors)

Work completed with mentorship from instructors @ MIT Beaver Works Summer Institute (Course: Quantum Software Development)

<hr/>

**Abstract**: We present the design and analysis of a quantum algorithm for solving perfect mazes using Grover's search. The algorithm operates on a superposition of all possible paths of a fixed length $L$, encoded in a quantum register. We developed a modular oracle, the <code>FitnessGate</code>, to evaluate all paths in parallel, validating them against maze walls and using a Manhattan distance-based metric to determine their fitness. Through classical simulation, the algorithm successfully solved $95.90$\% of $2 \times 2$ mazes. However, for $3 \times 3$ mazes, the solve rate dropped to 43.04\% while simulation time increased dramatically, highlighting significant scaling challenges. Our complexity analysis reveals the primary source of this challenge: the algorithm's runtime scales as $\mathcal{O}(2^L \cdot \text{Poly}(L, n))$, which is exponential in the path length $L$. This confirms that searching the state space of all possible paths does not offer a quantum advantage over efficient polynomial-time classical solvers. Our work underscores the critical importance of problem representation in quantum algorithm design and motivates the exploration of alternative methods, such as quantum walks, for future research.

<hr/>
