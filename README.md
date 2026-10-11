

# QAOA

A collection of notebooks and Python code exploring quantum optimization, including QAOA for Max-Cut and related quantum annealing experiments.

## Graph Visualization

![30 node complete graph](image/30%20node%20complete%20graphpng.png)

## Quantum Annealing on Circular and Möbius Ladder Graphs

This exploratory notebook compares circular ladder and Möbius ladder graphs using a Max-Cut formulation and D-Wave quantum annealing. Inspired by Hen and Young’s work, it investigates graph-dependent energy outcomes as a preliminary step toward studying graph distinguishability.

### Workflow

- Generate and visualize both graph families with NetworkX.
- Construct a QUBO representing a scaled negative Max-Cut objective.
- Sample the QUBO using a D-Wave QPU with automatic minor embedding.
- Compare returned energies across the graph families.
- Explore an experimental Ising Hamiltonian construction.

### Dependencies

- NumPy
- NetworkX
- Matplotlib
- D-Wave Ocean SDK (`dwave-system`)

The QPU sampling cells require configured D-Wave credentials and access to a compatible solver.

### Current Status

The notebook contains exploratory code and recorded execution errors. It does not establish a complete graph-isomorphism method.

- The energy plots compare returned samples; they do not measure evolution along an annealing schedule. The horizontal axis labeled `s` needs correction.
- The dense-Hamiltonian construction is unfinished and is not a valid Hamiltonian-to-QUBO conversion.
- Some cells contain embedding and array-shape errors.
- The proposed $Q_2$ observable is not implemented.
- Legacy NetworkX calls, including `nx.to_numpy_matrix`, need updating.
