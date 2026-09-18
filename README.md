# Numerically_solving_TDSE_for_different_systems
umerically solved the infinite square well, finite square well and harmonic oscillator. Discretised a spatial grid into N points and approximated the TISE as a matrix eigenvalue problem.

After discretising the grid into N points, I rewrote the time-independent Schrödinger equation by substituting the derivatives with their finite difference approximations. For each internal point you can write an individual TISE, leading to N coupled equations. This can be solved using matrices, where the eigenvalues are the energies and eigenvectors are the wavefunctions (found using np.linalg.eigh).
