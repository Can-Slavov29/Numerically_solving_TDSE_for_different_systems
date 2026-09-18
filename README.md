# Numerically_solving_TDSE_for_different_systems
umerically solved the infinite square well, finite square well and harmonic oscillator. Discretised a spatial grid into N points and approximated the TISE as a matrix eigenvalue problem.

After discretising the grid into N points, I rewrote the time-independent Schrödinger equation by substituting the derivatives with their finite difference approximations. For each internal point you can write an individual TISE, leading to N coupled equations. This can be solved using matrices, where the eigenvalues are the energies and eigenvectors are the wavefunctions (found using np.linalg.eigh).

For each system I aimed to also plot a different result from the solutions. The infinite square well I plotted the wavefunctions as is. For the Harmonic oscillator I plotted the normalised wavefunctions(normalised such that the integral of the probability density over the entire domain is equal to 1). For the finite square well I plotted the probability density itself.

Infinite square well was simple as no potential within the well and 0 outside means you only need to consider the grid within the well itself. The other two required more thought about the paramaters chosen as they would affect wether or not the wavefunction decayed properly and wether the behaviour was accurately captured.
