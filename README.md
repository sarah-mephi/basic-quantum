# basic-quantum
# This is a file containing a simple calculation of quantum states
import numpy as np

# Pauli matrices (you know these)
sigma_x = np.array([[0, 1], [1, 0]])
sigma_y = np.array([[0, -1j], [1j, 0]])
sigma_z = np.array([[1, 0], [0, -1]])

# Quantum state (vector from linear algebra)
psi = np.array([1, 0])  # |0⟩ state

# Apply gate (matrix multiplication from linear algebra)
psi_new = sigma_x @ psi  # Now |1⟩

print(f"Initial state: {psi}")
print(f"After X gate: {psi_new}")
