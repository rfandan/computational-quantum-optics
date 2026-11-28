# Module 0: Quantum Mechanics Fundamentals & Matrix Mechanics

This module establishes the core mathematical, continuous, and discrete foundations needed for computational quantum optics. It spans continuous wavefunctions, qubits and density matrices, generalized POVM measurements, quantum harmonic oscillators, split-operator time evolution, the three dynamical pictures of quantum mechanics, composite systems and entanglement, the Schwinger boson oscillator representation of $SU(2)$, and time-dependent perturbation theory culminating in Fermi's Golden Rule.

---

### Notebook Syllabus

| # | Notebook | Core Topics & Benchmarks |
| :-: | :--- | :--- |
| **01** | [`01_quantum_states_and_wavefunctions.ipynb`](./01_quantum_states_and_wavefunctions.ipynb) | Continuous $\psi(x)$, grid discretization, Simpson/trapezoid quadrature, state normalization $\int |\psi|^2 dx = 1$, quantum superposition and spatial interference fringes, expectation values $\langle x \rangle, \langle p \rangle$, position uncertainty $\Delta x$, and introduction to two-level state vectors. |
| **02** | [`02_qubits_and_density_matrices.ipynb`](./02_qubits_and_density_matrices.ipynb) | Discrete two-level systems, Dirac notation, Pauli operators $(\hat{\sigma}_x, \hat{\sigma}_y, \hat{\sigma}_z)$, pure vs. mixed state ensembles, density matrix properties ($\hat{\rho} \ge 0, \mathrm{Tr}(\hat{\rho}) = 1$), state purity $\gamma = \mathrm{Tr}(\hat{\rho}^2)$, von Neumann entropy, and Bloch sphere coordinate vector $\vec{r}$. |
| **03** | [`03_observables_measurement_uncertainty.ipynb`](./03_observables_measurement_uncertainty.ipynb) | Differential momentum operator $\hat{p} = -i\hbar \frac{\partial}{\partial x}$, canonical commutator $[\hat{x}, \hat{p}] = i\hbar$, von Neumann projective measurement postulate and state collapse, generalized Robertson-Schrödinger uncertainty relation $\Delta A \Delta B \ge \frac{1}{2}|\langle[\hat{A}, \hat{B}]\rangle|$, and minimum uncertainty Gaussian wavepackets. |
| **04** | [`04_generalized_measurements_and_povms.ipynb`](./04_generalized_measurements_and_povms.ipynb) | Positive Operator-Valued Measures (POVMs), partition of unity $\sum \hat{E}_m = \hat{I}$, generalized Born rule $p(m) = \mathrm{Tr}(\hat{E}_m\hat{\rho})$, Kraus measurement operators and state update, symmetric Trine POVM on the Bloch equator, Unambiguous State Discrimination (USD) of non-orthogonal states achieving the Ivanovic-Dieks-Peres (IDP) zero-error limit $P_{\text{USD}} = 1 - |\langle\psi_1|\psi_2\rangle|$, and Neumark's dilation theorem embedding arbitrary POVMs into unitary rotations on $\mathcal{H}_S \otimes \mathcal{H}_A$. |
| **05** | [`05_quantum_harmonic_oscillator.ipynb`](./05_quantum_harmonic_oscillator.ipynb) | Continuous 1D finite-difference Hamiltonian diagonalization, Hermite-Gauss eigenfunctions, discrete matrix mechanics via creation and annihilation ladder operators $(\hat{a}, \hat{a}^\dagger)$, Fock number basis $|n\rangle$, zero-point ground state energy $E_0 = \frac{1}{2}\hbar\omega$, and the direct algebraic bridge to electromagnetic field quantization. |
| **06** | [`06_time_evolution_and_wavepackets.ipynb`](./06_time_evolution_and_wavepackets.ipynb) | Time-dependent Schrödinger equation $i\hbar \partial_t \psi = \hat{H}\psi$, Split-Operator Fourier Method (SOFM) using Fast Fourier Transforms (FFT) $\mathcal{O}(N\log N)$, free-particle wavepacket dispersion $\sigma(t) = \sigma_0 \sqrt{1 + (t/\tau)^2}$, and non-spreading rigid translation of coherent states in parabolic oscillator potentials. |
| **07** | [`07_quantum_pictures_and_dyson_series.ipynb`](./07_quantum_pictures_and_dyson_series.ipynb) | The three dynamical pictures of quantum mechanics: Schrödinger (state evolution), Heisenberg (operator equations of motion $\frac{d\hat{A}_H}{dt} = \frac{i}{\hbar}[\hat{H}, \hat{A}_H]$), and Interaction (rotating frame under $\hat{H}_0$), exact numerical equivalence of physical expectation values across all three pictures, time-ordering meta-operator $\mathcal{T}$, multi-dimensional Dyson series expansion up to 2nd order, and rotating-frame elimination of fast carrier frequencies. |
| **08** | [`08_composite_systems_and_entanglement.ipynb`](./08_composite_systems_and_entanglement.ipynb) | Composite quantum systems and tensor product Hilbert spaces $\mathcal{H}_A \otimes \mathcal{H}_B$, partial trace reduction to subsystems $\hat{\rho}_A = \mathrm{Tr}_B(\hat{\rho}_{AB})$, pure-state Schmidt decomposition $|\psi\rangle = \sum \sqrt{\lambda_k}|u_k\rangle|v_k\rangle$ via SVD, entanglement entropy $S(\hat{\rho}_A) = -\sum \lambda_k \ln \lambda_k$, maximally entangled Bell states ($S = \ln 2 \approx 0.693147, \gamma_A = 0.50$), and the Peres-Horodecki Positive Partial Transpose (PPT) criterion isolating the $p = 1/3$ entanglement threshold for two-qubit Werner states. |
| **09** | [`09_angular_momentum_and_schwinger_bosons.ipynb`](./09_angular_momentum_and_schwinger_bosons.ipynb) | The $SU(2)$ Lie algebra of angular momentum $[\hat{J}_i, \hat{J}_j] = i\epsilon_{ijk}\hat{J}_k$, Casimir invariant $\hat{\mathbf{J}}^2 = j(j+1)\hat{I}$, the Schwinger two-mode boson representation ($\hat{J}_+ = \hat{a}^\dagger\hat{b}, \hat{J}_z = \frac{1}{2}(\hat{n}_a - \hat{n}_b)$), conservation of total photon number $[\hat{J}_i, \hat{N}] = 0$ with $j = N/2$, exact state mapping $|j, m\rangle \leftrightarrow |n_a = j+m, n_b = j-m\rangle$, lossless optical beam splitter as an exact $SU(2)$ rotation $\hat{U}_{\text{BS}} = \exp(-i 2\theta \hat{J}_x)$, and quantum Stokes operators on the Poincaré sphere. |
| **10** | [`10_perturbation_theory_and_fermis_golden_rule.ipynb`](./10_perturbation_theory_and_fermis_golden_rule.ipynb) | Time-dependent perturbation theory (TDPT) for harmonic optical drives, first-order transition amplitude $c_f^{(1)}(t)$, sinc-squared diffraction line shape $P(t) \propto t^2 \mathrm{sinc}^2((\omega_{fi}-\omega)t/2)$, continuum density of states $\rho(E)$, exact microphysical derivation of Fermi's Golden Rule decay rate $\Gamma = \frac{2\pi}{\hbar}|V_{fi}|^2 \rho(E_f)$, numerical validation of irreversible continuum exponential decay $e^{-\Gamma t}$ matching analytical predictions within $0.11\%$, short-time Quantum Zeno effect ($dP/dt|_{t=0} = 0$), and second-order virtual state transitions scaling as $1/\Delta_k^2$. |

---

### Key Formulas & Physical Principles

* **POVM Partition of Unity & Born Rule:**
  $$\sum_m \hat{E}_m = \hat{I}, \quad \hat{E}_m \ge 0, \quad p(m) = \mathrm{Tr}(\hat{E}_m\hat{\rho})$$

* **Unambiguous State Discrimination (IDP Bound):**
  $$P_{\text{USD}} = 1 - |\langle\psi_1|\psi_2\rangle|$$

* **Heisenberg Equation of Motion & Interaction Picture:**
  $$\frac{d\hat{A}_H}{dt} = \frac{i}{\hbar}[\hat{H}_H, \hat{A}_H] + \left(\frac{\partial \hat{A}}{\partial t}\right)_H, \quad \hat{V}_I(t) = e^{i\hat{H}_0 t/\hbar}\hat{V}(t)e^{-i\hat{H}_0 t/\hbar}$$

* **Dyson Series Expansion:**
  $$\hat{U}_I(t) = \mathcal{T} \exp\left( -\frac{i}{\hbar}\int_0^t \hat{V}_I(t') dt' \right) = \hat{I} - \frac{i}{\hbar}\int_0^t dt_1 \hat{V}_I(t_1) - \frac{1}{\hbar^2}\int_0^t dt_1 \hat{V}_I(t_1)\int_0^{t_1} dt_2 \hat{V}_I(t_2) + \dots$$

* **Schmidt Decomposition & Entanglement Entropy:**
  $$|\psi_{AB}\rangle = \sum_{k=1}^K \sqrt{\lambda_k}|u_k\rangle_A |v_k\rangle_B, \quad E(|\psi\rangle) = S(\hat{\rho}_A) = -\sum_{k=1}^K \lambda_k \ln \lambda_k$$

* **Peres-Horodecki (PPT) Criterion & Logarithmic Negativity:**
  $$\hat{\rho}_{AB}^{T_B} \ge 0 \iff \text{Separable (for } 2\times 2, 2\times 3\text{)}, \quad E_N(\hat{\rho}) = \log_2 \|\hat{\rho}^{T_B}\|_1$$

* **Schwinger Two-Mode Boson Operators:**
  $$\hat{J}_x = \frac{\hat{a}^\dagger\hat{b} + \hat{b}^\dagger\hat{a}}{2}, \quad \hat{J}_y = \frac{\hat{a}^\dagger\hat{b} - \hat{b}^\dagger\hat{a}}{2i}, \quad \hat{J}_z = \frac{\hat{a}^\dagger\hat{a} - \hat{b}^\dagger\hat{b}}{2}, \quad j = \frac{n_a + n_b}{2}$$
  $$\hat{U}_{\text{BS}}(\theta) = \exp(-i 2\theta \hat{J}_x) \quad (\text{Beam Splitter as } SU(2) \text{ Rotation})$$

* **Fermi's Golden Rule:**
  $$\Gamma_{i \to f} = \frac{2\pi}{\hbar} |\langle f | \hat{V} | i \rangle|^2 \rho(E_f)$$
