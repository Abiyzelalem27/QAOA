

# Max-Cut Optimization on Ladder Graphs

Explore Max-Cut optimization on circular ladder and Möbiusladder graphs using Quadratic Unconstrained Binary Optimization(QUBO) and Ising formulations.
 
### Workflow

- Generate and visualize both graph families with NetworkX.
- Construct a QUBO representing a scaled negative Max-Cut objective.
- Compare sampled energies and cut sizes across the graph families.
- Explore the relationship between Max-Cut and Ising Hamiltonians.

### Planned Extension: Quantum Approximate Optimization Algorithm(QAOA)

Implement the QAOA using a parameterized quantum circuit and a classical
optimizer, then compare its results with the annealing methods.