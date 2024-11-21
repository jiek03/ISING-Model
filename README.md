# ISING Model

<h4>Authors of this code:</h4>

- Javier Alejandro Pérez Garza
- Armando Adrian Pérez González

## Code Explanation
ISING model is a form of simulating continuous phase transitions. The model consists on defining $N$ magnetic dipole moments of atomic spins $\sigma$ in a mesh. The spins only can take two states in the form of $\sigma \in [-1,1]$, interacting periodically with their neighbors. The internal energy of the sysem  is given by the hamiltonian:

$$
\mathcal{H}(\vec{\sigma})=-J \sum_{i} \sum_{j=\mathbb{N}} \sigma_i \sigma_j -B \sum_{i} \sigma_i,
$$

where $\mathbb{N}$ is the set of first neighbors of spin $i$. The probability of observing a configuration $\vec{\sigma}$ is given by the Boltzmann distribution with inverse temperature:

$$
P(\vec{\sigma}) \propto e^{\frac{\mathcal{H}(\vec{\sigma})}{T}}
$$

The meshes simulated in this code are triangular and square, where each spin intteracts with its neighbors in the mesh.
